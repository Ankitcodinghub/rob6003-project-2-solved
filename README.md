# rob6003-project-2-solved
**TO GET THIS SOLUTION VISIT:** [ROB6003 Project 2 Solved](https://www.ankitcodinghub.com/product/rob6003-project-2-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;101507&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;ROB6003&nbsp;Project 2 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 138px;">
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
            5/5 - (1 vote)    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
&nbsp;

1 Direct and Inverse Kinematics

Consider the SCARA manipulator depicted below. For this project only the kinematic parameters are needed. You have received a trajectory for the the manipulator end effector. The trajectory is provided in a file named kinematic traj.mat and can be read using init.m.

The manipulator parameters are

d0 =1m, a1 =a2 =0.5m

θ1min = −π/2 rad, θ1max = π/2 rad, θ2min = −π/2 rad, θ2max = π/4 rad d3min =0.25m, d3max =1m, θ4min =−2πrad, θ4max =2πrad

The frames are depicted into the figure and the DH parameters are

di αi θi ai Link1 0 0 θ1 a1 Link2 0 0 θ2 a2

Link3 d3 0 0 0 Link4 0 0 θ4 0

Table 1: Table with DH parameters.

Please not that the 0 frame is not coincident with the b frame. There is a translation from the ground

plane denoted with d0 = 1. The frame 4 is coincident with the frame 3 at the starting. Be careful on the d3 component. The range of values is always positive. When the arm is fully extended (down towards the floor) the value is 1m whereas 0.25 when retracted (away from the floor). However, when you build your matrix note that d3 moves along −z2 axis and for this reason you translation in A23 should be negative as −d3 .

Questions:

1. Implement in Matlab/Simulink a second order algorithm for kinematic inversion with jacobian inverse along the given trajectory. Adopt the Euler integration rule with integration time 1 ms. Implement a final function visualize results.m for each part including for all the 2d-plots (joint value and operational space errors). A sample function called plot outputs.m is provided for the joint errors.

</div>
</div>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
2. Suppose to relax one component in the operational space (relax the z component), implement in Matlab/Simulink the second order algorithm for kinematic inversion with Jacobian pseudo-inverse along the given trajectory maximizing the distance from an obstacle along the path. Suppose that the obstacle is a sphere centered in p = 􏰆0.4 −0.7 0.5􏰇⊤ with radius 0.2 m.

Instructions:

<ul>
<li>Make your code as a combination of matlab and simulink. The structure is already provided in the folders. You should call your initialization in a function named init.m. This function should load the trajectory and all the manipulator variables that have been previously listed. You will then define your Jacobians in another function named Jacobian.m, which will be loaded in simulink as shown during the class. The derivative of the Jacbian is Jacobian dot.m. The file init.m contains as well a call to a 3D visualization of the manipulator behavior in case you want to use it. The file direct kin.m can be used if you like to write the direct kinematics in matlab in case you do not want to write that using simulink blocks.</li>
<li>Make a different folder of each question. Once init.m runs in each folder, we should be able to automatically play the simulink environment and obtain results. Show the joint trajectories in the joint space and the errors operational space.
2 Report

You need to summarize your results in a report submitted in pdf format and generated with latex or word. Please add on top of your manuscript your name and NYU ID. The report should not be more than 8 pages including plots. In addition to the results, please include your models and any explanation you think is appropriate. Do not just write equation, but try to add your logic process and explain why and how you used the equations or models you have in your code.
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</div>
