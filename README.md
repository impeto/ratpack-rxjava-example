# ratpack-rxjava-example
[![Build Status](https://travis-ci.org/gregwhitaker/ratpack-rxjava-example.svg?branch=master)](https://travis-ci.org/gregwhitaker/ratpack-rxjava-example)

An example of using [RxJava](https://github.com/ReactiveX/RxJava) with [Ratpack](https://ratpack.io/).

This example starts a Ratpack application that allows the user to upload and download files.

## Running the Example
The example can be run using the following Gradle command:

    $ ./gradlew run

Once the application has started you may upload a file to the service using the following curl command:

    $ curl -i -X POST -H "Content-Type: image/jpeg" -F "data=@demo/cat1.jpeg" http://localhost:5050/files

Now, you may download the file you just uploaded using the following curl command:

    $ curl -i http://localhost:5050/files/{file id here}

## Bugs and Feedback
For bugs, questions and discussions please use the [Github Issues](https://github.com/gregwhitaker/ratpack-rxjava-example/issues).

## License
MIT License

Copyright (c) 2017 Greg Whitaker

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
