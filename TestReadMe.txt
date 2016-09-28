Q1) Let me Explain the comparison between the two.
1) Abstract class can have abstract and non-abstract methods whereas Interface can have only abstract methods.
2) Abstract class doesn't support multiple inheritance whereas Interface supports multiple inheritance.
3) Abstract class can have final, non-final, static and non-static variables whereas Interface has only static and final variables.
4) Abstract class can have static methods, main method and constructor whereas Interface can't have static methods, main method or constructor.
5) Abstract class can provide the implementation of interface whereas Interface can't provide the implementation of abstract class.
6) The abstract keyword is used to declare abstract class and  interface keyword is used to declare interface.

Q2)

I dont have much details about this,I have used java 7 and i don't see any problem related to class inheritance.

Q3) 

- An Activity is an application component that provides a screen, with which users can interact in order to do something. 
- An Activity may contain 0 or multiple number of fragments based on the screen size.
- An activity can contain multiple fragments.
- A Fragment represents a behavior or a portion of user interface in an Activity.  A fragment can be reused in multiple activities, so it acts like a reusable component in activities.
- A fragment can't exist independently. It should be always part of an activity whereas activity can exist without any fragment in it.
- A Fragment is a part of an activity, which contributes its own UI to that activity.
- A Fragment can be thought like a sub activity, where as the complete screen with which user interacts is called as activity.
- A Fragment are mostly a part of an activity.

Q4)

We can use interfaces as callbacks to do this task , i.e host activity implements interface and then passes it an argument to fragment as you can see in the sample app i have implemented.

Q5)


Yes , we can make an Entire app without Fragments. I only know few of the cases where someone absolutely have to use fragment in android App.

for Example when you are using AsyncTask for background processing and have to retain the state on onreientation chages or configuration changes.

Q6)

- I know couple of issues realated to this AsyncTask. when an orientation or configuration change happens activity is recreatd and if the AsyncTask is ruunig in bakground will have old reference to the Activity ,this will try to update the old views which are not ailable.
- This can also create memory leak issues as it is maininting the old activity references.
- we can use AsyncTask within Fragment to avoid these complications , becasue fragments can retain their states and AsyncTask will have updated reference to the view.


 