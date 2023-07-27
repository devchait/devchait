- 👋 Hi, I’m @devchait
- 👀 I’m interested in software designing, AI & Neural Network, Computer Vision and building intelligent softwares
- 🌱 I’m currently learning NN-designs with pytorch and CUDA GPU Programming with C++17
- 💞️ I’m looking to open source some of my developments and continue my bloging on Python designing and learning Data-Science together effectively
- 📫 How to reach me devchait@gmail.com

<!---
devchait/devchait is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

Projects:
Roles and Responsibility: 
i. To research and architect the solution and decide over the frameworks to use
ii. Draw low-level plans and class structure to assign the task to software engineers and senior software engineers
iii. Mentor and train new Developers on the technology and assist in implementing the modules
iv. Co-ordinate the solution across multiple team and decide over the optimal strategical plan of implementation
v. Maintain the github repository, Eastablish github and code of conduct practices
vi. Setting up custom CI/CD for machine learning and product development with github client, github and DVC for multiple products
vii. Research and install the most suitable tools and ecosystem for faster and better development with minimal or low cost
viii. Research project management using Github Project boards as per the customer story and targeted as multiple sprints as part of scrum meeting
1. Multi-faceted Framework for Benchmarking Deep Learning Inference Solution:
  - What this framework comprise of :
  - Famework as deployable Video Analytic solution could server 25-30 real-time rtsp-stream with 30 fps as analytical stream-out solution
  - This framework reduce model deployment time by 95%
  - Reduce 85% development time for adding new business rules through custom plugins
  - ONVIF protocol support for analytical meta-data sharing
  - Multi-platform inferencing solution supports OpenCV, OpenVino, pytorch and tensorrt allowing benchmarking among each other in real-time scenarios.
  - Could scale simultaneously on GPU and CPU
  - Support for Windows and Ubuntu
  - Responsibility: In inception phase of AI research I architected and developed the entire framework from scratch. To deploy the solution on client machine. Benchmark the performance of business rules across various frameworks. Maintained the github repository for the solution.
  - Desing Patterns: Entire framework incorporated multiple design patterns like Facade, Bridge, Adapter, Proxy, Singleton, Oberver and Visitor.
  - libraries: RabbitMQ, pytorch, tensorrt, python bindings, Opencv, OpenVino, Shapely, pytest
  - Time taken: 2020 Feb - 2020 July
2. Vicon AI:
  - Server Solution
      - Architected Mass Video Analytic Server Solution for VMS system addressing 150-300 rtsp streams with 20-30 fps on intel xeon with 4 Tesla T4 cards
      - Vicon AI could read multiple realtime rtsp stream and communicates the analytical stream along with meta-data to multiple VMS nodes
      - Responsibility: Designed and developed entire layer solution structure with analytical API as base to Business rules as tail into stream-in and stream-out architecture. Implemented analytical library abstracting the complexity of analytics with simple API to be use in pipeline analytic stage. Analytical library involves deployment of tensorrt engines along with various strategies of inferencing to balance the input request among multiple operational resource to scale with maximum channels. Runs on both GPU and CPU. Wrote Heirarchical CMake struture from scratch
      - Lead the team of 5-6 developers. Maintaining the github repository and implemented CI solution
      - Platform: C++ 11 and 14, Tensorrt, CUDA, Windows, Ubuntu, UnitTest, CMake 3.2, Openvino
      - Design Patterns: Followed SOLID design pattern with pipeline paradigm
      - Time taken: 2020 August - 2022 December
  -  Real-time Tracking Framework
        - A Templated framework in Vicon AI Server solution addressing the problem of real-time light-weight multi-object tracking for mass streams. Runs on both CPU and GPU with featured and non-featured flavours. Reduce the complexity from nxnxn to nxm(logn). 1 milli-scond latency for 6-7 people to 5-7 milli-seconds for 40-50 people. Encapsulates object id, trace-path, direction of each object as a Frame State meta-information with Controlable object off-screen timining and id reutilization option. 
        - Responsibility: Designed and implemented the Tracking framework with few Association Algorithms with plugin mechanism allowing easy to deploy new Association algorithms directly in Vicon AI solution.
        - Association Algorithm CPU:
          - Non feature Association Algorithm took 1-6 milli-seconds for 7-40 people on intel i-7 utilizing 10-20 % CPU. It has nxmx (log n) complexity. Re-associate id in case of object occlusion for particular time. 
          - Accuracy: 
          - Based on the idea of Nearest Neighbour with maximal possible object proximity for adjustable fps this algorithm draws direct association without need of prediction thus providing less run-time complexity as compare to state-of-the-art Kalman tracker
        - Association Algorithm CUDA:
          - Latency: 1 milli-seconds irrespective of number of objects in frame.
          - Accuracy : 
          - Extended Object proximity possibility with maximum overlap 
          - Custom CUDA kernel for solving the Association problem with 5 dimensional feature matching. Matching is solved in n x m time with m concurrent cuda threads.
 3. Optimizations:
    - Implemented faster custom CUDA kernel for YOLO Pre-processing including batch support and normalization. This reduce the latency of end-to-end pipeline by 17%. ~ 2 milli-second reduction in end-to-end flow tested on GTX 1060 and deployed on multiple Production system comprising of RTX 3070 and A4000 type cards.
    - Modified YOLO cuda kernel to include distance and location information of an object. This information was collected as part of new output data-structure without changing the YOLO architecture. This improved tracking performance by 30% and reduce the latency by 15%
    - Implemented custom NMS plugin layer in tensorrt. This layer involve cuda kernel to solve NMS with same dimension for input and output. It uses win loss strategy and mark the looser value.
    - Expose the API functions for python binding and separte bindings for CUDA kernels. 

 4. Scalability:
    - GStreamer : GSteamer nvinfer video encoding and decoding with GStreamer as base API for Vicon Server Solution for large scale inference server 
    - DeepStream: Linux base solutions for Vicon AI Server
    - Triton:
    - Asynchronous strategy: Increase the throughput by 65%.
5. Models Deployed:
    - For Vicon AI Solution as part of the Analytics API deployed multiple engines. Few of those are Yolov3, Yolov5, Traffic Light Classification, Gender Classification and Anamoly Detection. Implemented unified API for accessing the underlying strategies of respective use-case.
6. Hands On :
    - Pytorch Modelling: Research and implemented various models 
    - Customized the Datalaoader for custom data-set input.
    - Pytorch classification Model Trainning and Deployment. Experienced in writing and training pytorch model. Loss functions used.
    - ONNX model to tensorrt: Converted ONNX model to Tensorrt engine files. 
    - Openvino to serialized engine
    - Experienced in serializing pytorch's weight file to tensorrt engines. This includes writing network definition in Tensorrt and writing custom tensorrt functions representing the equivalent operations of pytorch network layers.
7. DataLablePro:
    - DataLablePro is an ecosystem which provides role-base interface to solve multiple operations of AI/ML pipeline from Data Collection to Benchmarking the Business Events. This ecosystem comprise of DVC and github along with set of custom ML libraries and presistent database for auditing. Based on hybrid micro-service architecture the entire interface is web-based with python as backend fueling the ML operations. It supports multiple roles like Annotator, Reviewer, ML Engineer, QA Engineer, Project Manager. It supports YOLO, coco, json and various other Annotation formats.
    - Role: Product Manager and Solution Architect.
    - Responsibility: Ideating the new features on the basis of generic usage and in-house requirement. Designed every feature and its interactions. Lead the team members to implement the features. Designed and code the backend ML library. Implemented browser base persistent state for intial Make-Sense Fork to be known as DatalablePro. Github repository maintainer. Code Review and Feature release.
    - Contribution/ Key Insights: Structured the solution as multi-faceted architecture to accomodate independent implementation of loose scripts focusing on particular aspect of a problem in ML pipeline to finally act as single Product. This is a by-product of Vicon AI Server Solution.
    - ML Operations
    - Data set Labelling to Model Benchmarking
    - Ecosystem
    - Roles
    - Layers:
    - Optimization
    - Key Features: Queue base Annotation Task Assigment, Image and Video Annotation Review and feedback, Annotation format converter, Model Accuracy Validation, AI Model and Dataset version association, Project progress tracking and contribution insights
    - Github, DVC, python bindings, PostgressSQL, Micro-Services, ReactJS and Node, MOT benchmarking, COCO, plugins
    - Team: Lead the 10 member team.
    - My responsibility
    - Contribution
    - AI/ML Role
    - Benchmarking and Verification
9. Apache Beam Inferencing
10. NLP Model Inferencing

   
  
      
    
    
