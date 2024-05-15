# bloc_course_tutorials
Why Bloc?
Bloc makes it easy to separate presentation from business logic, making your code fast, easy to test, and reusable.

When building production quality applications, managing state becomes critical.

As developers we want to:

. know what state our application is in at any point in time.
. easily test every case to make sure our app is responding appropriately.
. record every single user interaction in our application so that we can make data-driven decisions.
. work as efficiently as possible and reuse components both within our application and across other applications.
. have many developers seamlessly working within a single code base following the same patterns and conventions.
develop fast and reactive apps.

Bloc was designed with three core values in mind:

.Simple: Easy to understand & can be used by developers with varying skill levels.
.Powerful: Help make amazing, complex applications by composing them of smaller components.
. Testable: Easily test every aspect of an application so that we can iterate with confidence.

Overall, Bloc attempts to make state changes predictable by regulating when a state change can occur and enforcing a single way to change state throughout an entire application.

Streams
A stream is a sequence of asynchronous data.

In order to use the bloc library, it is critical to have a basic understanding of Streams and how they work
If you’re unfamiliar with Streams just think of a pipe with water flowing through it. The pipe is the Stream and the water is the asynchronous data.


We can create a Stream in Dart by writing an async* (async generator) function.

count_stream.dart

Stream<int> countStream(int max) async* {
    for (int i = 0; i < max; i++) {
        yield i;
    }
}
