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
    - GStreamer : 
    - DeepStream
    - Triton
    - Asynchronous strategy
5. Models Deployed:
    - For Vicon AI Solution as part of the Analytics API deployed multiple engines. Few of those are Yolov3, Yolov5, Traffic Light Classification, Gender Classification and Anamoly Detection. Implemented unified API for accessing the underlying strategies of respective use-case.
6. Hands On :
    - Pytorch Modeling
    - Pytorch custom DataLoader
    - Pytorch classification Model Trainning and Deployment
    - Re-enforcement Learning
    - Openvino SSD Deployment
    - Pytorch models to tensorrt
    - ONNX model to tensorrt
    - Openvino to serializeed engine
    - Tensorrt Network and engine conversion
7. DataLablePro:
    - MakeSense Fork Date
    - Ideation
    - ML Operations
    - Data set Labelling to Model Benchmarking
    - Ecosystem
    - Roles
    - Layers
    - Designs
    - Optimization
    - Key Features
    - Github, DVC, python bindings, PostgressSQL, Micro-Services, ReactJS and Node
    - Team
    - My responsibility
    - Contribution
    - AI/ML Role
    - Benchmarking and Verification
8. Apache Beam Inferencing
9. NLP Model Inferencing

   
  
      
    
    
