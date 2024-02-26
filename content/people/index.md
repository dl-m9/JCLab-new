---
title: People
date: 2022-10-24

type: landing

sections:
  
  # - block: 
  #   id: about
  #   content: 
  #     title: <img src="http://www.fang.ece.ufl.edu/fang13.jpg" width="60%"> 
  #     subtitle: <b>Prof. FANG Yuguang<b><br>ACM Fellow, IEEE Fellow
  #     # Choose a user profile to display (a folder name within `content/authors/`)
  #     text: |-
        
  #   design:
  #     columns: '2'
  #     username: admin
  - block: people
    content:
      title: Meet the Team
      # Choose which groups/teams of users to display.
      #   Edit `user_groups` in each user's profile to add them to one or more of these groups.
      user_groups:
          - Faculty
          - Postdoctoral Researchers
          - Current PhD Students
          - Visiting Students

      sort_by: Params.last_name
      sort_ascending: true
    design:
      show_interests: false
      show_role: true
      show_social: true
      # show_organizations: true
  - block: people
    content:
      title: Former Members (@CityU HK)
      # Choose which groups/teams of users to display.
      #   Edit `user_groups` in each user's profile to add them to one or more of these groups.
      user_groups:
          # - Principal Investigators
          # - Faculty
          # - Researchers
          # - Graduated PhD Students
          # - Graduated Master Students
          # - Former Postdoctoral Researchers
          # - Former Visiting Scholars
          # - Former Visiting Student
  
      sort_by: Params.last_name
      sort_ascending: true
    design:
      show_interests: false
      show_role: true
      show_social: true
  - block: people
    content:
      title: Former Members (@University of Florida)
      # Choose which groups/teams of users to display.
      #   Edit `user_groups` in each user's profile to add them to one or more of these groups.
      user_groups:
          # - Principal Investigators
          # - Faculty
          # - Researchers
          - Graduated PhD Students
          - Graduated Master Students
          - Former Postdoctoral Researchers
          - Former Visiting Scholars
          - Former Visiting Students

        

      sort_by: Params.last_name
      sort_ascending: true
    design:
      show_interests: false
      show_role: true
      show_social: true
---
