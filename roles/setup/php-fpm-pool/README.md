# php-fpm-pool role for Ansible

## Expected data structure

    php_fpm_pool:
      name: ""
      user: ""
    
      # Pool management options
      min_servers: 1
      avg_servers: 3
      max_servers: 10
    
      # PHP ini directives
      memory_limit: "256M"
      max_post_size: "20M"
      max_file_size: "15M"
      ini_directives: []
    
      # Environment variables
      envvars:
        - name: "APPLICATION_ENV"
          value: "production"
