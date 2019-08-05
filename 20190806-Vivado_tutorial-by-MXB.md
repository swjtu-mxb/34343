## Getting Started

In this lab, you will learn about the Project mode features for project creation, source file management, design analysis, constraint definition, and synthesis and implementation run management. This could be used as a quick reference.

<br>
--------------------------------
-  **Step 1: Creating a Project**
--------------------------------
*Launching Vivado*

*Creating a New Project*

1. After Vivado opens, select **Create Project** on the Getting Started page.

2. Click **Next** in the New Project wizard

3. Specify the Project Name and Location (Select “**Create project subdirectory**” to create a folder for your project) 

4. Click **Next**.

5. Select **RTL Project** as the **Project Type** and click **Next**.(Select **Do not specify sources at this time** and add your files soon afterwards)

   *(The Vivado Design Suite allows for different design entry points depending on your source file types and design tasks. You can choose the suitable type of project.)*

6. Select the **xc7s15ftgb196-1** part for project, and click Next, as shown in figure 1.

![img](https://i.screenshot.net/03j6ot5)

<center> Figure 1. </center>
The Vivado IDE opens project_tutorial in the default layout, as shown in figure 2.

![img](https://i.screenshot.net/55kmphv)

<center> Figure 2. </center>
The **Flow Navigator** shows the basic design process clearly.

The **Sources** is made up of **Constraints**, **Simulation** **Sources** and **Utility** **Sources**.

The **Design Runs** creates synth_1 and impl_1 by default.

The **running status** of vivado is displayed in the upper right corner.

<br> 
---------------------------------------
-  **Step 2: Add and Create Your Files** 
---------------------------------------

1. Click **Add Sources** in the **PROJECT MANAGER** of the Flow **Navigator**

2. Select **Add or create design sources** and click Next.

3. Click the button![img](https://i.screenshot.net/0dnqqco) and select options or click the options directly to add or create files, as shown in figure 3.

![](https://i.screenshot.net/nqo47fg)

<center> Figure 3. </center>
4. Here, we add files prepared by selecting **Add Directories** , you can also select **Add Files** to do this. Remember to select **Scan and add RTL include files into project** if you have RTL include files in the folder, as shown in figure 4.

![img](https://i.screenshot.net/zm5nnt8) 

<center> Figure 4. </center>
5. Click **Finish**.

9. Click **Add Sources** in the **PROJECT MANAGER** of the Flow **Navigator** again and Select **Add or create constraints** and click Next to add the corresponding **constraints**.

10. Click **Add Files** and add your constraints.

11. Click **Finish**.

12. As above, add **simulation sources** if needed.

    Finally, the file we added will appear in the **Sources**, as shown in figure 5.

![img](https://i.screenshot.net/neqvvc9)

<center> Figure 5. </center>
<br>
----------------------------------------
-  **Step 3: Elaborating the RTL Design**
----------------------------------------

  The Vivado IDE includes an RTL analysis and IP customizing environment. There are also several RTL Design Rule Checks (DRCs) to examine ways to improve performance or power on the RTL design.

1. Select Open Elaborated Design in the Flow Navigator to elaborate the design.

2. Ensure that the Layout Selector pull down menu in the main Toolbar has Default Layout selected. The Elaborated Design enables various analysis views including an RTL Netlist, Schematic, and Graphical Hierarchy. The views have a cross-select feature, which helps you to debug and optimize the RTL.

3. Explore the logic hierarchy in the RTL Netlist window and examine the Schematic. You can traverse the schematic by double-clicking on cells to push into the hierarchy, or by using commands like the Expand Cone or Expand/Collapse from the Schematic popup menu. 

4. Select any logic instance in the Schematic and right-click to select the **Go to Source** or **Go to Definition** commands.

5. Click the Messages window at the bottom of the Vivado IDE, and examine the messages.

6. Click the **Collapse All** button in the Messages toolbar.

7. Expand the Elaborated Design and the messages, as shown in figure 6.

![img](https://i.screenshot.net/5pe00t7)

<center> Figure 6. </center>
8. Click one of the links and the Text Editor opens the RTL source file with the relevant line highlighted.
9. Close the Text Editor windows.
10. Close the Elaborated Design by clicking on the **X** on the right side of the Elaborated Design window banner, and click OK to confirm.

<br>
----------------------------------
-  **Step 4: Using the IP Catalog**
----------------------------------

  The Xilinx IP Catalog provides access to the Vivado IP configuration and generation features. You can sort and search the Catalog in a variety of ways. IP can be customized, generated, and instantiated.

1. Click the **IP Catalog** button in the Flow Navigator, under Project Manager.

2. Browse the IP Catalog to examine the various categories and IP filtering capabilities.

3. Choose the corresponding IP and perform native customization and configuration of IP within the tool and select **OK**

4. Close the IP Catalog tab by clicking on the X on the window tab.

<br>
-------------------------------------------
-  **Step 5: Running Behavioral Simulation**
-------------------------------------------

  The Vivado IDE integrates the Vivado Simulator, which enables you to add and manage simulation sources in the project. You can configure simulation options, and create and manage simulation source sets. You can run behavioral simulation on RTL sources, prior to synthesis.

1. In the Flow Navigator, under Project Manager, click the Settings command. The Settings dialog box opens with Project Settings at the top, and Tool Settings below that, as shown in figure 7.

![img](https://i.screenshot.net/0ndggi8)

<center> Figure 7. </center>
2. Examine the settings available on the  **Simulation** page, then click **Cancel** to close the dialog box.

3. Click the **Run Simulation** command in the Flow Navigator, then click the **Run Behavioral**

​       **Simulation** in the sub-menu.

4. Examine and explore the Simulation environment.

<br>
-----------------------------------------------
- **Step 6:  Reviewing Design Run Settings**
-----------------------------------------------

  Design runs are a way of configuring and storing the many options available in the different steps of the synthesis and implementation process. You can configure these options and save the configurations as strategies to be used in future runs.

1. In the Flow Navigator, under Project Manager, click the **Settings** command.

2. Select the **Synthesis** page under Project Settings. For a complete description of these options, see the *Vivado Design Suite User Guide: Synthesis*([UG901](https://www.xilinx.com/support/documentation/sw_manuals/xilinx2018_3/ug901-vivado-synthesis.pdf)).

3. Select the **Implementation** page under Project Settings. For a complete description of these options, see the *Vivado Design Suite User Guide: Implementation*([UG904](https://www.xilinx.com/support/documentation/sw_manuals/xilinx2018_3/ug904-vivado-implementation.pdf )).


<br>
----------------------------------------------------------
- **Step 7: Synthesizing and Implementing the Design**
----------------------------------------------------------

  After configuring the synthesis and implementation run options, you can **run synthesis** and **run implementation** in the **Design Runs** or click the button ![img](https://i.screenshot.net/llo40sg)  or click corresponding buttons in the **Flow Navigator** to do this. The **running status** of vivado is displayed in the upper right corner while Synthesizing and Implementing.

 

​	For this tutorial, we will run these steps in the Design Runs.

1. Right click the syth_1 and select **Launch Runs**, as shown in figure 8.

   ![1564773413803](https://i.screenshot.net/1x2kkiw)

   <center> Figure 8. </center>

2. Click ok and running status is displayed in the upper right corner, as shown in figure 9.

![img](https://i.screenshot.net/qwk7qf7)

<center> Figure 9. </center>
3. Click  **Open Synthesized Design** for further design and analysis. You can see **Report Timing Summary** , **Report Utilization** and others, as shown in figure 10.

![img](https://i.screenshot.net/xx691a3)

<center> Figure 10. </center>
4. Run Implementation in the same way, as shown in figure 11.

![img](https://i.screenshot.net/4zr88i5)

<center> Figure 11. </center>
5. Click **Open implemented Design** to see reports after implementation 

<br>
---------------------------------------------
- **Step 8: Generating a Bitstream File**
---------------------------------------------

  After **Implementing the Design,** we can see synthesis and implement Complete in the **Design Runs**,as shown in figure 12.

![img](https://i.screenshot.net/l0ge2te)

<center> Figure 12. </center>
 Click **Generate Bitstream** in the Flow Navigator.

<br>
-------------------------------
-  **Step 9: Download the file **
-------------------------------

  After **Generate Bitstream,** you have two ways to load the file to FPGA. 

  You can use the JTAG interface(on the Right-Up corner of figure 13) to load the bit file to FPGA  in vivado,
or use ESP32 to load the bit file to FPGA.

![img](https://i.screenshot.net/4l0w0i7)

<center> Figure 13. </center>
  **Follow below steps, to load bitstream to FPGA through JTAG interface**

1. Power the board and connect the downloader.

2. Click **Open Target** and **Auto Connect** in the Flow Navigator.

3. While connect to the board successfully, click **Program Device** and choose the bit file and click **Program**, as shown in figure

![img](https://i.screenshot.net/26kqqur)

4. After download the bit file, the **FPGA**_**DONE** **led** will light.

   *In this project, if you press any key or both of them,  **LED L1**  will go out.*
