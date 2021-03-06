# sample_dagger2_android_graphs

Just converting [android-activity-graphs](https://github
.com/google/dagger/tree/master/examples/android-activity-graphs)
 exmple to Android Studio.

Example: Android Activity Graphs
================================

Building on top of the simple Android example, this example demonstrates how it is possible to
create child graphs for each activity which extend from the global graph.

Some of the advantages of the activity scope:

 * Provides the ability to inject objects which require the activity to be constructed.
 * Allows for the use of singletons on a per-activity basis. This is a great way to manage a
   resource that is shared by a bunch of fragments in an activity.
 * Keeps the global object graph clear of things that can be used only by activities.

While this example only shows the presence of an activity scope, you should be able to see the
potential for other useful scopes that can be used. For example, having a dedicated object graph
for the current user session is a great way to manage data that is tied to the currently logged-in
user.

_Note: The app does not actually do anything when it is run. It is only to show how you can
 structure Dagger within an Android app_

_Note: The app is in transition to Dagger 2 and may not reflect recommended patterns.  Before
 we release Dagger 2.0 it will, but until this note is removed, please do not rely on this
 example as a strong recommendation._
