# Grafana dashboard


## GlusterFS-***.json

Dashboard for GlusterFS data from gluster_exporter via Prometheus
- inodes by volume
- size by volume
- +/- volumes data growth
- heal files count
- available bricks

gluster_exporter: https://github.com/ofesseler/gluster_exporter

Prometheus yml
  - job_name: gluster
    static_configs:
    - targets: ['localhost:9189']
