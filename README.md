Download Link: https://assignmentchef.com/product/solved-bbm104-assignment-1-classes-object-constructor-and-getter-setter-encapsulation
<br>
<strong> Assignment 1-</strong><strong> </strong>Classes, Object, Constructor and Getter/Setter, Encapsulation

In this experiment, you are supposed to develop a simple Journal System program. The main aim of the experiment is to develop your skill of using Class, Object, Constructor, Getter/Setter, and Encapsulation with Java programming language.

<h1>2           General Information</h1>

In this section you can find some useful beginner’s level information that you will need for this project. For more information on each subject you need to do additional research and consult other resources (e.g. lecture notes, textbook, Internet resources, etc.).

Object-oriented programming (OOP) is more than just adding a few new features to programming languages. It is rather a new way of thinking about decomposing and modeling problems with less complexity and more code reuse when developing programming solutions. In OOP, a program is viewed as a collection of loosely connected objects, each of which is responsible for specific tasks. It is through the interaction of these objects that computation proceeds and the model works as a whole.

In this assignment, you will work with the concepts of OOP in order to practice them and observe their advantages. With this assignment, you will learn the concepts of relationships among classes, encapsulation.

<h2>2.1         Encapsulation</h2>

Encapsulation is one of the fundamental OOP concepts. It is a technique of wrapping (packaging) the related data (attributes) and behavior (code – methods) together into a single unit. It also provides a way to hide and control data by protecting it from misuse by the outside world. This is achieved by making data members private, and using public helper methods through which we can decide the level of access we want to provide (e.g. read-only, write-only). A fully encapsulated Java class is a class whose all variables are private.

The advantages of encapsulation include: flexibility in modifying code in case requirements change, reusability of encapsulated code throughout multiple applications if necessary, and reducing the time of maintenance (update) process.

<strong>2.1.1        Visibility Modifiers</strong>

In Java, there are four access modifiers which provide various access levels: private (visible inside of the class only), default/package (visible inside of the package), protected (visible inside the package and to all subclasses) and public (visible to everyone).

<h1>3           Problem</h1>

You will write a Journal System application. You will use the given corpus in order to list articles which belong to Authors. Also you will complete Authors’ articles by using article file.

General Rules:

<ul>

 <li>An author has maximum 5 articles.</li>

 <li>An article id’s first 3 characters equal to an author id.</li>

</ul>

Your program should read the following three files: article file, author file and command file. Java provides a rich API for input/output (I/O) operations. In this experiment you will use I/O (Input/Output) classes of Java to perform file operations.

<h1>4           Input File Format</h1>

<ul>

 <li><strong>Author File (author.txt)</strong>: Each line starts with “AUTHOR” string and author id. The others are optional. An author has 10 attributes which are id, name, university, department, email, article#1, article#2, article#3, article#4 and article#5. All attributes of the Author must be “private” Java access modifier.</li>

</ul>

Figure 1: A class structure for the ”Author” file

Figure 2: Sample Author File

<ul>

 <li><strong>Article File (article.txt)</strong>: Each line starts with “ARTICLE” string. An article has 4 attributes which are paper id, name, publisher name and year of publish. All attributes of Article must be “private” Java access modifier.</li>

</ul>

<table>

 <tbody>

  <tr>

   <td width="108"></td>

  </tr>

  <tr>

   <td></td>

   <td></td>

  </tr>

 </tbody>

</table>

Figure 3: A class structure for the ”Article” file

Figure 4: Sample Article File

<ul>

 <li><strong>Command File (command.txt): </strong>Your program should be able to process and respond to 5 different commands, which are defined below. You will take these commands from an input file (command.txt), according to commands, show the output to the output file (output.txt). The name of the input files (“author.txt” and “command.txt”) and output file (“output.txt”) will be fixed. So, please be careful about not to taking these files with a different name.</li>

</ul>

Figure 5: Sample command.txt

Now, we go through all the lines of the sample command.txt with the following commands:

<strong>COMMAND-1: </strong><em>read “articlefilename”: </em>The Journal System will read the article file and add articles to the end of the article array which stores article objects. You don’t need to print anything to the output file for this command. The output should be as shown in Figure 6 when performing line 2 (command-2: (<em>list</em>)) after line 1 (command-1: (<em>read article1.txt</em>)) from sample command.txt as shown in Figure 5.

Figure 6: Output format for <em>read article1.txt and list </em>commands

<strong>COMMAND-2: </strong><em>list: </em>The Journal System will show authors and authors’ article(s) in the following format. The outcome of this command will be printed out on output file (the name of the output file will be fixed as “output.txt”). This command always comes after the other four commands (command-1, command-3, command-4, and command-5).

Figure 7: Output format for <em>list </em>command

<strong>COMMAND-3: </strong><em>completeAll: </em>We have mentioned that an author has max 5 articles in Section 3. So, by this command, the Journal System will complete articles of the Authors, who have less than 5 articles, with considering article paper id. When performing completeall command, you will going through the article.txt file, and check the missing articles according to the article id for each author, and complete his/her articles to the 5 articles. The output should be as shown in Figure 8 when performing line 4 (command-2: (<em>list</em>)) after line 3 (command-3: (<em>completeAll</em>)) from sample command.txt as shown in Figure 5.

Figure 8: Output format for <em>completeAll and list </em>commands

<strong>COMMAND-4: </strong><em>sortedAll: </em>print articles which are sorted in ascending order according to article paper id. After performing the line 5 (command-4) and line 6 (command-2) from sample command.txt as given in Figure 5 respectively, the output for this command should be as given in figure 10.

Figure 9: Output format for <em>sortedAll and list </em>commands

<strong>COMMAND-5: </strong><em>del authorid: </em>This command deletes the corresponding author, which is given with its id, and all its attributes. This operation will be done regarding author id. “del 100” means that delete the author whose id is equal 100, and list the updated version of the array. After performing the line 7 (command-5) and line 8 (command-2) respectively from sample command.txt as shown in Figure 5, the output should be as given in Figure 10.

Figure 10: Output format for <em>del and list </em>commands

<h1>5           Output Format</h1>

The output format and an exemplar output example are given in Figure <strong>??</strong>.

<table>

 <tbody>

  <tr>

   <td width="108"></td>

  </tr>

  <tr>

   <td></td>

   <td></td>

  </tr>

 </tbody>

</table>

Figure 11: Sample output format

Output of the program will be as shown below:

——————————-List—————————————–

Author:100 Olivier_Duchenne MIT Computer_Science <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="d1bebdb8a7b4a391bcb8a5ffb4b5a4">[email protected]</a>

+1002001 A_Graph-matching_Kernel_for_Object_Categorization ICCV 2012

+1002004 From_Contours_to_3D_Object_Detection_and_Pose_Estimation ICCV 2012

+1002007 Variational_Stereo_in_Dynamic_Illumination ICCV 2012

+1002012 Source_Constrained_Clustering ICCV 2012

+1002018 Content-Based_Photo_Quality_Assessment CVPR 2013

Author:101 Ruonan_Li MIT Computer_Science <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="e092958f8e818ea08d8994ce858495">[email protected]</a>

+1002001 A_Graph-matching_Kernel_for_Object_Categorization ICCV 2012

+1002009 A_Theory_of_Coprime_Blurred_Pairs ICCV 2012

+1002004 From_Contours_to_3D_Object_Detection_and_Pose_Estimation ICCV 2012 Author:102 Horst_Bischof HUN Computer_Engineering <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="b8d0d7cacbccf8dbcb96d0d9dbddccccddc8dd96dddccd96ccca">[email protected]</a>

+1002004 From_Contours_to_3D_Object_Detection_and_Pose_Estimation ICCV 2012

Author:103 Pietro_Perona METU Computer_Science <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="cebea7abbabca18eadabe0a3abbabbe0abaabbe0babc">[email protected]</a>

+1002004 From_Contours_to_3D_Object_Detection_and_Pose_Estimation ICCV 2012

+1032019 HEAT:Iterative_Relevance_Feedback_with_One_Million_Images CVPR 2013

Author:104 Nadia_Payet METU Computer_Engineering <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="d5bbb4b1bcb495b6b0fbb8b0a1a0fbb0b1a0fba1a7">[email protected]</a>

+1002001 A_Graph-matching_Kernel_for_Object_Categorization ICCV 2012

+1042020 Unsupervised_Learning_of_a_Scene-Specific_Coarse_Gaze_Estimator CVPR 2013

+1042010 Learning_to_Predict_the_Perceived_Visual_Quality_of_Photos ICCV 2012

+1042008 Revisiting_Radiometric_Calibration_for_Color_Computer_Vision ICCV 2012

Author:105 Blake_Johnson HARVARD Computer_Science <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="6f0d030e040a2f070e1d190e1d0b410a0b1a">[email protected]</a>

————————–End—————————————

**************************CompleteAll Successful*******************

————————–List————————————–

Author:100 Olivier_Duchenne MIT Computer_Science <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="ee818287988b9cae83879ac08b8a9b">[email protected]</a>

+1002001 A_Graph-matching_Kernel_for_Object_Categorization ICCV 2012

+1002004 From_Contours_to_3D_Object_Detection_and_Pose_Estimation ICCV 2012

+1002007 Variational_Stereo_in_Dynamic_Illumination ICCV 2012

+1002012 Source_Constrained_Clustering ICCV 2012

+1002018 Content-Based_Photo_Quality_Assessment CVPR 2013

Author:101 Ruonan_Li MIT Computer_Science <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="4331362c2d222d032e2a376d262736">[email protected]</a>

+1002001 A_Graph-matching_Kernel_for_Object_Categorization ICCV 2012

+1002009 A_Theory_of_Coprime_Blurred_Pairs ICCV 2012

+1002004 From_Contours_to_3D_Object_Detection_and_Pose_Estimation ICCV 2012

+1012013 Inferring_Social_Relations_from_Visual_Concepts ICCV 2013

+1012014 Maximizing_All_Margins:Pushing_Face_Recognition_with_Kernel_Plurality CVPR 2013

Author:102 Horst_Bischof HUN Computer_Engineering <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="ddb5b2afaea99dbeaef3b5bcbeb8a9a9b8adb8f3b8b9a8f3a9af">[email protected]</a>

+1002004 From_Contours_to_3D_Object_Detection_and_Pose_Estimation ICCV 2012

+1022002 Domain_Adaptation_for_Object_Recognition:An_Unsupervised_Approach ICCV 2012

+1022005 Non-stationary_Correction_of_Optical_Aberrations ICCV 2012

+1022015 DTAM:Dense_Tracking_and_Mapping_in_Real-Time CVPR 2013

+1022016 Kernel_Non-Rigid_Structure_from_Motion CVPR 2013

Author:103 Pietro_Perona METU Computer_Science <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="72021b1706001d3211175c1f1706075c1716075c0600">[email protected]</a>

+1002004 From_Contours_to_3D_Object_Detection_and_Pose_Estimation ICCV 2012

+1032019 HEAT:Iterative_Relevance_Feedback_with_One_Million_Images CVPR 2013

+1032003 Decision_Tree_Fields ICCV 2012

+1032011 HMDB:A_Large_Video_Database_for_Human_Motion_Recognition ICCV 2012

+1032017 A_Dimensionality_Result_for_Multiple_Homography_Matrices CVPR 2013

Author:104 Nadia_Payet METU Computer_Engineering <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="a0cec1c4c9c1e0c3c58ecdc5d4d58ec5c4d58ed4d2">[email protected]</a>

+1002001 A_Graph-matching_Kernel_for_Object_Categorization ICCV 2012

+1042020 Unsupervised_Learning_of_a_Scene-Specific_Coarse_Gaze_Estimator CVPR 2013

+1042010 Learning_to_Predict_the_Perceived_Visual_Quality_of_Photos ICCV 2012

+1042008 Revisiting_Radiometric_Calibration_for_Color_Computer_Vision ICCV 2012

+1042006 Linear_stereo_matching ICCV 2012

Author:105 Blake_Johnson HARVARD Computer_Science <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="ddbfb1bcb6b89db5bcafabbcafb9f3b8b9a8">[email protected]</a> ——————————End————————————-

*****************************SortedAll Successful********************* —————————–List————————————-

Author:100 Olivier_Duchenne MIT Computer_Science <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="6e010207180b1c2e03071a400b0a1b">[email protected]</a>

+1002001 A_Graph-matching_Kernel_for_Object_Categorization ICCV 2012

+1002004 From_Contours_to_3D_Object_Detection_and_Pose_Estimation ICCV 2012

+1002007 Variational_Stereo_in_Dynamic_Illumination ICCV 2012

+1002012 Source_Constrained_Clustering ICCV 2012

+1002018 Content-Based_Photo_Quality_Assessment CVPR 2013

Author:101 Ruonan_Li MIT Computer_Science <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="6b191e04050a052b06021f450e0f1e">[email protected]</a>

+1002001 A_Graph-matching_Kernel_for_Object_Categorization ICCV 2012

+1002004 From_Contours_to_3D_Object_Detection_and_Pose_Estimation ICCV 2012

+1002009 A_Theory_of_Coprime_Blurred_Pairs ICCV 2012

+1012013 Inferring_Social_Relations_from_Visual_Concepts ICCV 2013

+1012014 Maximizing_All_Margins:Pushing_Face_Recognition_with_Kernel_Plurality CVPR 2013

Author:102 Horst_Bischof HUN Computer_Engineering <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="84ecebf6f7f0c4e7f7aaece5e7e1f0f0e1f4e1aae1e0f1aaf0f6">[email protected]</a>

+1002004 From_Contours_to_3D_Object_Detection_and_Pose_Estimation ICCV 2012

+1022002 Domain_Adaptation_for_Object_Recognition:An_Unsupervised_Approach ICCV 2012

+1022005 Non-stationary_Correction_of_Optical_Aberrations ICCV 2012

+1022015 DTAM:Dense_Tracking_and_Mapping_in_Real-Time CVPR 2013

+1022016 Kernel_Non-Rigid_Structure_from_Motion CVPR 2013

Author:103 Pietro_Perona METU Computer_Science <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="e090898594928fa08385ce8d859495ce858495ce9492">[email protected]</a>

+1002004 From_Contours_to_3D_Object_Detection_and_Pose_Estimation ICCV 2012

+1032003 Decision_Tree_Fields ICCV 2012

+1032011 HMDB:A_Large_Video_Database_for_Human_Motion_Recognition ICCV 2012

+1032017 A_Dimensionality_Result_for_Multiple_Homography_Matrices CVPR 2013

+1032019 HEAT:Iterative_Relevance_Feedback_with_One_Million_Images CVPR 2013

Author:104 Nadia_Payet METU Computer_Engineering <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="026c63666b634261672c6f6776772c6766772c7670">[email protected]</a>

+1002001 A_Graph-matching_Kernel_for_Object_Categorization ICCV 2012

+1042006 Linear_stereo_matching ICCV 2012

+1042008 Revisiting_Radiometric_Calibration_for_Color_Computer_Vision ICCV 2012

+1042010 Learning_to_Predict_the_Perceived_Visual_Quality_of_Photos ICCV 2012

+1042020 Unsupervised_Learning_of_a_Scene-Specific_Coarse_Gaze_Estimator CVPR 2013

Author:105 Blake_Johnson HARVARD Computer_Science <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="187a7479737d5870796a6e796a7c367d7c6d">[email protected]</a>

————————-End———————————————–

*************************del Successful************************************

————————-List———————————————-

Author:101 Ruonan_Li MIT Computer_Science <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="3143445e5f505f715c58451f545544">[email protected]</a>

+1002001 A_Graph-matching_Kernel_for_Object_Categorization ICCV 2012

+1002004 From_Contours_to_3D_Object_Detection_and_Pose_Estimation ICCV 2012

+1002009 A_Theory_of_Coprime_Blurred_Pairs ICCV 2012

+1012013 Inferring_Social_Relations_from_Visual_Concepts ICCV 2013

+1012014 Maximizing_All_Margins:Pushing_Face_Recognition_with_Kernel_Plurality CVPR 2013

Author:102 Horst_Bischof HUN Computer_Engineering <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="dfb7b0adacab9fbcacf1b7bebcbaababbaafbaf1babbaaf1abad">[email protected]</a>

+1002004 From_Contours_to_3D_Object_Detection_and_Pose_Estimation ICCV 2012

+1022002 Domain_Adaptation_for_Object_Recognition:An_Unsupervised_Approach ICCV 2012

+1022005 Non-stationary_Correction_of_Optical_Aberrations ICCV 2012

+1022015 DTAM:Dense_Tracking_and_Mapping_in_Real-Time CVPR 2013

+1022016 Kernel_Non-Rigid_Structure_from_Motion CVPR 2013

Author:103 Pietro_Perona METU Computer_Science <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="c5b5aca0b1b7aa85a6a0eba8a0b1b0eba0a1b0ebb1b7">[email protected]</a>

+1002004 From_Contours_to_3D_Object_Detection_and_Pose_Estimation ICCV 2012

+1032003 Decision_Tree_Fields ICCV 2012

+1032011 HMDB:A_Large_Video_Database_for_Human_Motion_Recognition ICCV 2012

+1032017 A_Dimensionality_Result_for_Multiple_Homography_Matrices CVPR 2013

+1032019 HEAT:Iterative_Relevance_Feedback_with_One_Million_Images CVPR 2013

Author:104 Nadia_Payet METU Computer_Engineering <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="bfd1dedbd6deffdcda91d2dacbca91dadbca91cbcd">[email protected]</a>

+1002001 A_Graph-matching_Kernel_for_Object_Categorization ICCV 2012

+1042006 Linear_stereo_matching ICCV 2012

+1042008 Revisiting_Radiometric_Calibration_for_Color_Computer_Vision ICCV 2012

+1042010 Learning_to_Predict_the_Perceived_Visual_Quality_of_Photos ICCV 2012

+1042020 Unsupervised_Learning_of_a_Scene-Specific_Coarse_Gaze_Estimator CVPR 2013

Author:105 Blake_Johnson HARVARD Computer_Science <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="442628252f21042c2536322536206a212031">[email protected]</a>

<h1>6           Execution and Test</h1>

The input files are going to be given as program arguments. There are text files (article.txt, author.txt, command.txt) in your working directory. In order to test your program, you should follow the following steps:

<ul>

 <li>Upload your java files to your server account (dev.cs.hacettepe.edu.tr)</li>

 <li>Compile your code (javac *.java)</li>

 <li>Run your program (java Main author.txt command.txt)</li>

 <li>Control your output data (output.txt).</li>

</ul>