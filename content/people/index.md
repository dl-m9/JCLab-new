---
title: People
date: 2022-10-24

type: landing

sections:
  
  # - block: 
  #   # id: about
  #   content: 
  #     title: <img src="http://www.fang.ece.ufl.edu/fang13.jpg" width="60%"> 
  #     subtitle: <b>Prof. FANG Yuguang<b><br>ACM Fellow, IEEE Fellow
  #     # Choose a user profile to display (a folder name within `content/authors/`)
  #     text: |-
        
  #   design:
  #     columns: '2'
      # username: admin
  - block: people
    content:
      title: Meet the Team
      # Choose which groups/teams of users to display.
      #   Edit `user_groups` in each user's profile to add them to one or more of these groups.
      user_groups:
          - Faculty
          - Postdoctoral Researchers
          - Current PhD Students
          - Visitors

      sort_by: Params.last_name
      sort_ascending: true
    design:
      show_interests: false
      show_role: true
      show_social: true
  - block: people
    content:
      title: Former Members
      # Choose which groups/teams of users to display.
      #   Edit `user_groups` in each user's profile to add them to one or more of these groups.
      user_groups:
          # - Principal Investigators
          # - Faculty
          # - Researchers
          # - Current PhD Students
          # - Postdoctoral Researchers
          # - Visitors
          # - Alumnis
        

      sort_by: Params.last_name
      sort_ascending: true
    design:
      show_interests: false
      show_role: true
      show_social: true
---
