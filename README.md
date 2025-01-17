# Module 5

**Nama** : **Jason Kent Winata** <br/>
**NPM** : **2206081313** <br/>

## Before Refactoring:
![test_plan_1](https://github.com/Fec16/exercise-profiling/assets/118716513/d32c2dca-d032-4d2f-afa0-cbeeaa407fd9)
![testresults1](https://github.com/Fec16/exercise-profiling/assets/118716513/f3eab464-5bdb-43ef-bdeb-8cca10d7154f)
![test_plan_2](https://github.com/Fec16/exercise-profiling/assets/118716513/4bd87f7a-cf4b-4166-a543-9946b66ebd03)
![testresults2](https://github.com/Fec16/exercise-profiling/assets/118716513/6388b366-d48f-4bee-ab9d-aae18d69e662)
![test_plan_3](https://github.com/Fec16/exercise-profiling/assets/118716513/8928cd85-d445-42cc-a147-83848c38ed7e)
![testresults3](https://github.com/Fec16/exercise-profiling/assets/118716513/ed6efb27-27cc-44ea-be31-aa388a4b7188)

## After Refactoring:
![test_plan_1_after](https://github.com/Fec16/exercise-profiling/assets/118716513/4a82cc1a-4cfc-4856-8761-cc9e5fe3692e)
![testresults1_after](https://github.com/Fec16/exercise-profiling/assets/118716513/b5d78cd3-84c2-41af-95cc-e6b3f69f59ae)
![test_plan_2_after](https://github.com/Fec16/exercise-profiling/assets/118716513/a42c6e77-0b16-43c7-b668-39c42d36f659)
![testresults2_after](https://github.com/Fec16/exercise-profiling/assets/118716513/ecfa1d96-1506-4029-a7c3-197afc4b6e2d)
![test_plan_3_after](https://github.com/Fec16/exercise-profiling/assets/118716513/baea4e4d-2cda-42fe-8076-a8c282487a01)
![testresults3_after](https://github.com/Fec16/exercise-profiling/assets/118716513/c5505fd0-fdb2-445d-af35-5295341a6007)


## Reflection
**Please answer the following questions:**
1. What is the difference between the approach of performance testing with JMeter and profiling with IntelliJ Profiler in the context of optimizing application performance? <br/>

    _Performance testing with JMeter and Profiling with Intellij are two different approaches used in the context of optimizing application performance. Here’s how they differ:_

    - Performance testing happens at the system level, under varying types of load. It ensures your system lives up to its Service Level Agreements (SLAs). This type of testing is typically used to understand how an application behaves under specific conditions, such as under heavy load or with many concurrent users.
    - Profiling is what you do when your performance testing shows a problem. It helps you identify those parts of your system that contribute the most to the performance problem and shows you where to concentrate your efforts. IntelliJ IDEA provides integration with profilers like Java Flight Recorder and Async Profiler. These profilers collect valuable information about your Java code’s behavior at runtime, determine where the hot spots are, and help understand how a framework operates under the hood. IntelliJ Profiler uses sampling, so the overhead is very low – close to running the program without the profiler. <br/>
   
    _In summary, Profiling allows you to drill down into the code level to identify and address specific performance bottlenecks. Both profiling and Performance testing are essential tools in the process of optimizing application performance. They complement each other and are often used together during the performance optimization process._<br/>


2. How does the profiling process help you in identifying and understanding the weak points in your application? <br/>

   _Profiling helps me identify which part of the program is hampering the overall performance of the application. Thus, I only need to optimize those parts so that the overall application will improve its performance better without the need to fix too many parts of the application._


3. Do you think IntelliJ Profiler is effective in assisting you to analyze and identify bottlenecks in your application code? <br/>

   _Yeah, through Intellij profiler, I find out that the part of the program that takes the longest time is the findStudentWithHighestGpa method. I can even find out which line in the method is hampering the performance of the method. Because I get the information on the duration of time needed to operate the function calls, I can easily detect which part of the program is a bottleneck for the whole program._
    

4. What are the main challenges you face when conducting performance testing and profiling, and how do you overcome these challenges? <br/>

   _One of the most challenging thing is understanding the relevant output results and identifying which parts of the program are bottlenecks in the application. The way to overcome this is to examine the output of JMeter or the profiler carefully and slowly, and it may take some time to get used to this new technology in order to obtain important information more easily._   


5. What are the main benefits you gain from using IntelliJ Profiler for profiling your application code? <br/>

   _IntelliJ's profiler allows Users to identify the bottleneck parts of the program, knowing how long it takes to execute a method call, and how often the method is called. With this information, we can adjust the parts of the program that need optimization and ignore the unnecessary ones. It is important to remember that unnecessary optimization efforts will only reduce the readability of our code._


6. How do you handle situations where the results from profiling with IntelliJ Profiler are not entirely consistent with findings from performance testing using JMeter? <br/>

   _From some literatures and forums I have read, JMeter performance is affected by various factors such as operating system, JVM version, and others. These variations can result in differences in JMeter testing between one device and another. The way around this is to use containers like Docker instead of .jmx files, and also pay attention to think time. By doing so, it is expected that the JMeter test results will be more consistent and will not fluctuate from one machine to another. It is important to keep in mind that the test results from Profiler and JMeter may differ due to different ways of working, where JMeter focuses on testing the application's persistence._


7. What strategies do you implement in optimizing application code after analyzing results from performance testing and profiling? How do you ensure the changes you make do not affect the application's functionality? <br/>

   _To improve the performance of the code after the testing and profiling process is done is to check the duration taken by the program to respond requests using JMeter. If the response is too slow, I then use the profiler to find the bottleneck part of the code and find ways to improve its performance. After making the changes, I made sure that the output remained the same as before to ensure the correctness of the code._
