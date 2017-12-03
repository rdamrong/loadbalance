Example Playbook
----------------

- name: Blue Deployment
  hosts: all
  
  roles:
    - {role: loadbalance, WORKSHOP_ID: '131', scenario: 'blue' }

###################

- name: Green Deployment
  hosts: all
  
  roles:
    - {role: loadbalance, WORKSHOP_ID: '131', scenario: 'green' }

###################
- name: Blue-Green Server
  hosts: all
  
  roles:
    - {role: loadbalance, WORKSHOP_ID: '131', scenario: 'blue-green' }
