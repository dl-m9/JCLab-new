---
# Leave the homepage title empty to use the site title
title: 
date: 2022-10-24
type: landing

sections:

  - block: markdown
    content:
      title: 
      subtitle:
      text: |
       
        <div class="slideshow-container">
          <div class="mySlides fade">
            <img src="files/signage.png" style="width:100%">
          </div>
          <div class="mySlides fade">
            <img src="files/group1.jpg" style="width:100%">
          </div>
          <div class="mySlides fade">
            <img src="files/group2.JPG" style="width:100%">
          </div>
          <div class="mySlides fade">
            <img src="files/group3.JPG" style="width:100%">
          </div>

          <!-- 前后导航按钮 -->
          <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
          <a class="next" onclick="plusSlides(1)">&#10095;</a>
        </div>

        <!-- 导航点 -->
        <div style="text-align:center">
          <span class="dot" onclick="currentSlide(1)"></span>
          <span class="dot" onclick="currentSlide(2)"></span>
          <span class="dot" onclick="currentSlide(3)"></span>
          <span class="dot" onclick="currentSlide(4)"></span>
        </div>

        <style>
        /* 幻灯片容器样式 */
        .slideshow-container {
          max-width: 100%;
          position: relative;
          margin: auto;
          height: 800px; /* 设置固定高度 */
          overflow: hidden;
        }

        /* 修改幻灯片显示方式 */
        .mySlides {
          display: none; /* 默认隐藏 */
          width: 100%;
          height: 100%;
        }

        /* 确保第一张幻灯片默认显示 */
        .mySlides:first-child {
          display: block;
        }

        .mySlides img {
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;
        }

        /* 前后按钮 */
        .prev, .next {
          cursor: pointer;
          position: absolute;
          top: 50%;
          width: auto;
          margin-top: -22px;
          padding: 16px;
          color: white;
          font-weight: bold;
          font-size: 18px;
          transition: 0.6s ease;
          border-radius: 0 3px 3px 0;
          user-select: none;
          background-color: rgba(0,0,0,0.3);
          z-index: 2; /* 确保按钮在图片上方 */
        }

        /* 定位"下一个"按钮到右边 */
        .next {
          right: 0;
          border-radius: 3px 0 0 3px;
        }

        /* 悬停时添加黑色背景 */
        .prev:hover, .next:hover {
          background-color: rgba(0,0,0,0.8);
        }

        /* 导航点样式 */
        .dot {
          cursor: pointer;
          height: 15px;
          width: 15px;
          margin: 0 2px;
          background-color: #bbb;
          border-radius: 50%;
          display: inline-block;
          transition: background-color 0.6s ease;
        }

        .active, .dot:hover {
          background-color: #717171;
        }

        /* 淡入淡出动画 */
        .fade {
          animation-name: fade;
          animation-duration: 1.5s;
        }

        @keyframes fade {
          from {opacity: .4}
          to {opacity: 1}
        }
        </style>

        <script>
        let slideIndex = 1;

        // 简化的显示幻灯片函数
        function showSlides(n) {
          const slides = document.getElementsByClassName("mySlides");
          const dots = document.getElementsByClassName("dot");
          
          if (n > slides.length) {slideIndex = 1}
          if (n < 1) {slideIndex = slides.length}
          
          // 隐藏所有幻灯片
          for (let i = 0; i < slides.length; i++) {
            slides[i].style.display = "none";
          }
          
          // 移除所有导航点的active类
          for (let i = 0; i < dots.length; i++) {
            dots[i].className = dots[i].className.replace(" active", "");
          }
          
          // 显示当前幻灯片和激活对应导航点
          slides[slideIndex-1].style.display = "block";
          dots[slideIndex-1].className += " active";
        }

        function plusSlides(n) {
          showSlides(slideIndex += n);
        }

        function currentSlide(n) {
          showSlides(slideIndex = n);
        }

        // 页面加载完成后初始化
        window.onload = function() {
          showSlides(slideIndex);
        };

        // 确保DOM加载完成后也初始化
        document.addEventListener("DOMContentLoaded", function() {
          showSlides(slideIndex);
        });
        </script>
        
    # design:
    #   columns: '1'
    #   background:
    #     image:
    #       filename: group2.jpg
    #       filters:
    #         brightness: 1
    #       parallax: True
    #       position: center
    #       size: coverhu
    #     text_color_light: False
        
          
      css_class: fullscreen
      spacing:
        padding: ['40px', '0', '20px', '0']
  # - block: hero
  #   content: 
  #     title: 
  #       JC STEM Lab of Smart City
  #     image:
  #       filename: group_photo.jpg
  #     text: | 
  #       <br>
  #       <p>
  #       The JC STEM Lab of Smart City was founded by <a href="https://www.cs.cityu.edu.hk/~yugufang/">Prof. FANG Yuguang</a> in 2022 in Hong Kong, Our mission is to leverage vehicles to build a smarter city.  
  #       </p>
        
  #   design:
  #     background:
  #       gradient_start: '#0476D0'
  #       gradient_end: '#D26085'
  #       text_color_light: true
  #       gradient_angle: 45

  - block: features
    design:
      background:
        color: 
    content:
      title: Our Research
      
      items:
        - name: Internet of Things
          description:
          icon: iot
          icon_pack: custom
        - name: Federated Learning
          description:
          icon: chart-line
          icon_pack: fas
        - name: Smart City
          description: 
          icon: 🌆
          icon_pack: emoji
        - name: Wireless Communication
          description: 
          icon: 📱
          icon_pack: emoji
        - name: Vehicle as a Service (VaaS)
          description: 
          icon: car
          icon_pack: custom
        - name: Security & Privacy
          description: 
          icon: user-secret
          icon_pack: fas
        - name: Health Monitoring
          description: 
          icon: 🏥
          icon_pack: emoji
        - name: Semantic + AI Communications
          description: 
          icon: key
          icon_pack: fas 
        - name: Collaborative Distributed ML
          description: 
          icon: 🤝
          icon_pack: emoji
    
        
  - block: markdown
    id: news
    content:
      title: Latest News
      
      subtitle: 
      text: |-

            
            # <html lang="en">
            # <head>
            #     <meta charset="UTF-8">
            #     <meta name="viewport" content="width=device-width, initial-scale=1.0">
            #     <title>Scrollable Content</title>
            #     <style>
            #         .scrollable-content {
            #             height: 800px;
            #             overflow-y: scroll;
            #             # border: 1px solid #ccc;
            #             padding: 10px;
            #         }
            #     </style>
            # </head>
            # <body>

            # <div class="scrollable-content">
            <div>
            <ul>
              <li><b>[Dec. 2024]</b> Congratulations to <b>Dr. Xiaojing Wen</b>, our former visiting student, who joined Shanghai Jiao Tong University as a <b>Assistant Researcher</b>!!!</li>
              <li><b>[Oct. 2024]</b> Congratulations to <b>Professor Xianhao Chen (EEE, HKU)</b>, our former lab member, who received the <b>Hong Kong Research Grant Council's Early Career Award</b> in 2024/25!</li> 
              <li><b>[Jul. 2024]</b> Congratulations to <b>Dr. Guowen Xu</b>, who will join the Department of Computer Science at the <b>University of Electronic Science and Technology of China (UESTC)</b> as a <b>full professor</b>!!!</li> 
              <li><b>[Jul. 2024]</b> Congratulations to <b>Dr. Hao Yue</b>, who will move to the Department of Computer Science and Engineering at the <b>University of California, Santa Cruz (UCSC)</b> as a <b>tenured associate professor</b> in September!!!</li> 
              <li><b>[11/23/2023]</b>   Congratulations to Professor <b><a href="author/dr.-li-pan">Pan Li</a></b>, our former lab member, who has been elevated  to <b>IEEE Fellow</b>!!!</li> 
              
              <li><b>[01/18/2023]</b> 🔥🔥🔥 Congratulations to <b>Prof. Fang</b>, who has been elevated to <b><span style="color:#1565C0;"><a href="https://www.acm.org/media-center/2023/january/fellows-2022">  ACM Fellow</a>   </span></b>!!!</li>
              
              <li><b>[08/05/2022]</b> 🔥🔥🔥 Congratulations to <b>Prof. Fang</b>, who will join the Department of Computer Science, City University of Hong Kong (CityU), as the <b>Chair Professor of Internet of Things</b>!!! </li>
              
              <li><b>[06/21/2022]</b> Congratulations to <b>Dr. Jianqing Liu</b>, our former member, who will join the Department of Computer Science, North Carolina State University (NC State), as an <b>assistant professor</b>!!! </li>
              
              <li><b>[05/10/2022]</b> Congratulations to <b>Kaichen</b>, who has accepted an <b>assistant professor</b> position in the Department of Electrical and Computer Engineering at <b>Michigan Technological University</b>!!! </li>
              
              <li><b>[05/05/2022]</b> Congratulations to <b>Linke</b>, our former member, who has been promoted to <b>Associate Professor</b> with tenure in the Department of Electrical and Computer Engineering at Clemson University!!!</li>
              
              <li><b>[03/29/2022]</b> Congratulations to <b>Xianhao</b>, who has accepted a <b>tenure-track Assistant Professor</b> position in the Department of Electrical and Electronic Engineering at <b>The University of Hong Kong</b>!!! </li>

              <li><b>[04/30/2022]</b> Congratulations to <b>Rui Hu</b> (a PhD student of Dr. Yanmin Gong), who has accepted an <b>Assistant Professor</b> position at the Department of Computer Science and Engineering, <b>University of Nevada, Reno</b>!!!</li>

              <li><b>[04/25/2022]</b> Congratulations to <b>Yifang Guo</b> and <b>Tianxi Ji</b> (PhD students of Dr. Pan Li), who have accepted <b>tenure-track</b> <b>Assistant Professor</b> positions in the Department of Computer and Information Sciences at <b>Towson University</b> and the Department of Computer Science at <b>Texas Technological University</b>, respectively!!! Congratulations to Pan as well!</li>

              <li><b>[04/01/2022]</b> Congratulations to <b>Yaodan</b>, who has accepted an <b>assistant professor</b> position in the Department of Electrical and Computer Engineering at <b>Idaho State University</b>!!!</li> 
              
              <li><b>[02/02/2022]</b> Congratulations to <b>Yanmin</b> and <b>Yuanxiong</b>, our former members, who have been promoted to <b>Associate Professor</b> with tenure at University of Texas at San Antonio!!!</li>

              <li><b>[11/11/2022]</b> Congratulations to <b>Haichuan Ding</b>, who has joined the School of Cyberspace Science and Technology, <b>Beijing Institute of Technology</b>, Beijing, China, as a <b>full professor</b>! </li>
              <li> Check more previous news <a href="https://winet.cs.cityu.edu.hk/">here</a>.</li>
            </ul>
            </div>

            # </body>
            # </html>
    design:
      columns: '1'
      background:
        image: 
          filename: 
          filters:
            brightness: 1
          parallax: false
          position: center
          size: cover
          text_color_light: true
      # spacing:
      #   padding: ['20px', '0', '20px', '0']
      # css_class: fullscreen
      
  # - block: collection
  #   content:
  #     title: Latest News
  #     subtitle: 
  #     text: 
  #     count: 5
  #     filters:
  #       author: ''
  #       category: ''
  #       exclude_featured: false
  #       publication_type: ''
  #       tag: ''
  #     offset: 0
  #     order: desc
  #     page_type: event
  #   design:
  #     view: showcase
  #     columns: '2'
  
  # - block: markdown
  #   content:
  #     title:
  #     subtitle: ''
  #     text:
  #   design:
  #     columns: '1'
  #     background:
  #       image: 
  #         filename: coders.jpg
  #         filters:
  #           brightness: 1
  #         parallax: false
  #         position: center
  #         size: cover
  #         text_color_light: true
  #     spacing:
  #       padding: ['20px', '0', '20px', '0']
  #     css_class: fullscreen
  - block: contact
    id: contact
    content:
      title: Contact
      text: |-
        We are located in the main campus of City University of Hong Kong. Our old website is <a href="https://winet.cs.cityu.edu.hk/">here</a>.
      email: my.Fang@cityu.edu.hk
      # link: 'https://www.cs.cityu.edu.hk/~yugufang/'
      # phone: +852 3442-2596
      # Fax: +852 3442-0503
      address:
        street: 83 Tat Chee Ave
        city: Kowloon Tong
        region: Hong Kong
        # postcode: '94305'
        # country: United States
        # country_code: US
      coordinates:
        latitude: '22.33703'
        longitude: '114.173196'
      # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      # office_hours:
      #   - 'Monday 10:00 to 13:00'
      #   - 'Wednesday 09:00 to 10:00'
      # appointment_url: 'https://calendly.com'
      #contact_links:
      #  - icon: comments
      #    icon_pack: fas
      #    name: Discuss on Forum
      #    link: 'https://discourse.gohugo.io'
    
      # Automatically link email and phone or display as text?
      autolink: true
    
      # Email form provider
      # form:
      #   provider: netlify
      #   formspree:
      #     id:
      #   netlify:
      #     # Enable CAPTCHA challenge to reduce spam?
      #     captcha: false
    design:
      columns: '2'
  - block: markdown
    content:
      title:
      subtitle:
      text: |
        ![](files/plaque.png)
    design:
      columns: '1'
      background:
        image:
          filename: 
  - block: markdown
    content:
      title:
      subtitle:
      text: |
        <div style="width: 30%; height: auto; margin: auto;">
        <script type="text/javascript" id="clstr_globe" src="//clustrmaps.com/globe.js?d=5ARm8_nN_s8xJvlRADyN_VZA0ugAYp45tSMSw9xW0Uc"></script>
        </div>
    design:
      columns: '1'
      background:
        image:
          filename: 
      # css_class: fullscreen
---