# cs661-assignment-3--particle-tracing-in-steady-flow-field-solved
**TO GET THIS SOLUTION VISIT:** [CS661 Assignment 3 -Particle Tracing in Steady Flow Field Solved](https://www.ankitcodinghub.com/product/assignment-3-cs661-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;131849&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS661 Assignment 3 -Particle Tracing in Steady Flow Field  Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
Particle Tracing in Steady Flow Field

In this assignment, you will write a particle tracing program to generate streamlines from a 3D vector field data set using Runge–Kutta 4 (RK4) integration. We have discussed the method in class.

Here is what your code should do:

1. You will load a vector field data set that has a vector array named ‘vectors.’ It is a 3D vector field data set, so vectors at each grid point will have three components.

2. Given a user-provided seed location, you will apply the RK4 integration to generate a streamline. Your Python script should take the 3D seed location as an input parameter.

3. You will perform RK4 integration in both forward and backward directions, starting from the seed location to trace forward and backward directions. Finally, you will create a single streamline and store it as a VTKPolyData file (*.vtp). To trace the particle in the backward direction, you can simply use a negative integration step size. Hence, your streamline should consist of points traced in a backward direction + seed point (at center) + points traced in the forward direction. It should be a single continuous line, as shown in Fig. 1.

4. Your code should take the 3D seed location as input from the user and output a single *.vtp file, which is the streamline traced from the input seed location.

5. You could set step size in RK4 = 0.05 and max number of steps = 1000 for testing. Note that your streamline can go out of the bounds of the data set. Therefore, you must check that your current point on the streamline is within the bounds of the vector field. You can use data.GetBounds() to query the vector field bound and compare the point location on your streamline with the XYZ bounds of the data set. If the streamline is out of bounds after an integration step, you should stop tracing and return the result.

6. To get a vector at each step, you must perform interpolation to get the vector at each location. In this assignment, you are not required to implement your interpolation routine. Instead, you will use VTKProbeFilter() to query vector location at any point in the data set. It will give you the vector at any queried location, and you can use that to perform particle tracing.

7. You are not allowed to use VTK Stream Tracer. You must implement the program on your own.

If you have implemented correctly, you should see images like the following for input seed (0,0,7):

Fig. 1: Plot of a streamline from three different views. The seed location is (0,0,7), step size is 0.05 and maximum number of steps is 1000. Both forward and backward tracing is used and results are combined into a single streamline.

Dataset for this task:

The dataset that you will use in this assignment is a 3D vector field data of a simulated tornado. The VTI file is provided with the assignment.

How to submit?

“groupnum_rollnum1_rollnum2_Assignment3.zip”.

** You must ensure you are submitting your correct submission files. If you upload wrong files, you will not be allowed to submit again. We will only grade your submitted version from HelloIITK. No submissions will be accepted after the allowed late days. **
