# 加入 springCloud

springboot与springcloud版本对应   
jar包名更改  

HystrixFallbackConfiguration implements FallbackProvider  

Eureka注册中心设置：          
    设置是否将自己作为客户端注册到注册中心（缺省true）  
    这里为不需要（查看@EnableEurekaServer注解的源码，会发现它间接用到了@EnableDiscoveryClient）  
    eureka.client.register-with-eureka=false  
    eureka.client.fetch-registry: false  
    eureka.client.service-url.defaultZone: http://localhost:8761/eureka/  