---
# Leave the homepage title empty to use the site title
title: 
date: 2022-10-24
type: landing

sections:
  - block: hero
    content: 
      title: 
        JC STEM Lab for Smart City
      image:
        filename: group.jpg
      text: | 
        <br>
        <p>
        The JC STEM Lab for Smart City was founded by <a href="https://www.cs.cityu.edu.hk/~yugufang/">Prof. FANG Yuguang</a> in 2022 in Hong Kong, Our mission is leveraging vehicles to build a smarter city.  
        </p>
        <p style="font-size:20px;color:#B8DCFF">
          JC STEM Lab is embedded in the 
        <a href = "https://www.cs.cityu.edu.hk/">Department of Computer Science</a> 
        at 
        <a href = "https://www.cityu.edu.hk/">City Universitu of Hong Kong</a> 
        </p> 
    design:
      background:
        gradient_start: '#0476D0'
        gradient_end: '#D26085'
        text_color_light: true
        gradient_angle: 45

  - block: features
    design:
      background:
        color: 
    content:
      title: Our Topics
      subtitle: 
        <div align="center">
          <img src="https://ts1.cn.mm.bing.net/th/id/R-C.cd97f629606d8b000d974125f9a81d15?rik=ecRwQcGHGLJr9w&riu=http%3a%2f%2fwww.cityu.edu.hk%2fchem%2fconference%2f2018-icoban%2fimg%2fCityU_Logo_Basic_Signature.png&ehk=%2f8dNdGv6%2bWB%2bszhrlxZ%2fQkRRwPcRBhtde3YBTsm8JdM%3d&risl=&pid=ImgRaw&r=0" width="15%"><br>
        </div>
      text: We are based at City University of Hong Kong
      items:
        - name: Internet of Things
          description: The Internet of Things (IoT) is a network of interconnected devices that communicate and exchange data, enhancing automation and real-time monitoring in various fields, from home appliances to industrial machinery.
          icon: iot
          icon_pack: custom
        - name: Federated Learning
          description: Federated Learning is a machine learning approach where models are trained across multiple decentralized devices or servers holding local data samples, protecting privacy while still enabling collaborative learning.
          icon: chart-line
          icon_pack: fas
        - name: Smart City
          description: Our mission is to leverage vehicles to build a smarter city in Hong Kong
          icon: 🌆
          icon_pack: emoji
        - name: Wireless Communication
          description: Wireless communication refers to data transmission between devices without physical connections, using radio waves, infrared signals, or other electromagnetic waves.
          icon: 📱
          icon_pack: emoji
        - name: Vehicle as a Service (VaaS)
          description: Our Vision is to leverage the Vehicles to build a 
          icon: car
          icon_pack: custom
        - name: Cybersecurity
          description: 10%
          icon: user-secret
          icon_pack: fas
        - name: Hong Kong
          description: Our group is based in Hong Kong, which is a premier financial hub attracting global businesses. The city also boasts world-class universities, offering top-notch education and vast research opportunities, making it a magnet for international scholars.
          icon: 🇭🇰
          icon_pack: emoji
        - name: Privacy for ML & FL
          description: 10%
          icon: key
          icon_pack: fas 
        - name: Collaborative Distributed ML
          description: 10%
          icon: 🤝
          icon_pack: emoji
    
        
  - block: markdown
    content:
      title: Latest News
      subtitle: /#hello.md
      text: |-
            <b>[01/18/2023]</b> 🔥🔥🔥 Congratulations to **Prof. Fang**, who has been elevated to <b><span style="color:blue;">ACM Fellow</span></b>!!!
            <br> <br>
            <b>[08/05/2022]</b> 🔥🔥🔥 Congratulations to **Prof. Fang**, who will join the Department of Computer Science, City University of Hong Kong (CityU), as the **Chair Professor of Internet of Things**!!! 
            <br> <br>
            <b>[06/21/2022]</b> Congratulations to **Dr. Jianqing Liu**, our former member, who will join the Department of Computer Science, North Carolina State University (NC State), as an **assistant professor**!!! (6/21/2022) <br><br>
            <b>[05/10/2022]</b> Congratulations to **Kaichen**, who has accepted an **assistant professor** position in the Department of Electrical and Computer Engineering at **Michigan Technological University**!!! <br><br>

            <b>[05/05/2022]</b> Congratulations to **Linke**, our former member, who has been promoted to **Associate Professor** with tenure in the Department of Electrical and Computer Engineering at Clemson University!!!
                        <br> <br>

            
            <b>[03/29/2022]</b> Congratulations to **Xianhao**, who has accepted a **tenure-track Assistant Professor** position in the Department of Electrical and Electronic Engineering at **University of Hong Kong**!!! <br> <br>
            
            {{< spoiler text="Click to View More" >}}
            
            - <b>[04/30/2022]</b> Congratulations to **Rui Hu** (a PhD student of Dr. Yanmin Gong), who has accepted an **Assistant Professor** position at the Department of Computer Science and Engineering, **University of Nevada, Reno**!!!  <br> <br>
            - <b>[04/25/2022]</b> Congratulations to **Yifang Guo** and **Tianxi Ji** (PhD students of Dr. Pan Li), who have accepted **tenure-track** **Assistant Professor** positions in the Department of Computer and Information Sciences at **Towson University** and the Department of Computer Science at **Texas Technological University**, respectively!!! Congratulations to Pan as well!<br> <br>
            - <b>[04/01/2022]</b> Congratulations to **Yaodan**, who has accepted an **assistant professor** position in the Department of Electrical and Computer Engineering at **Idaho State University**!!!<br> <br> 
            - <b>[02/02/2022]</b> Congratulations to **Yanmin** and **Yuanxiong**, our former members, who have been promoted to **Associate Professor** with tenure at University of Texas at San Antonio!!! <br> <br>
            - <b>[11/11/2022]</b> Congratulations to **Haichuan (Ding)**, who has joined the School of Cyberspace Science and Technology, **Beijing Institute of Technology**, Beijing, China, as a **full professor**! <br> <br>
            {{< /spoiler >}}

    design:
      columns: '2'
      
        
        
       
      

    design:
      columns: '2'
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
      
  - block: collection
    content:
      title: Latest News
      subtitle: 
      text: 
      count: 5
      filters:
        author: ''
        category: ''
        exclude_featured: false
        publication_type: ''
        tag: ''
      offset: 0
      order: desc
      page_type: event
    design:
      view: showcase
      columns: '2'
  
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
  
  - block: markdown
    content:
      title:
      subtitle:
      text: |
        {{% cta cta_link="./people/" cta_text="Meet the team →" %}}
    design:
      columns: '1'
---