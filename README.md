# using-micronaut-in-spring-error
----

Error:

```
# rhasija ~/tmp/using-micronaut-in-spring-error on git:master x  
$ mvn spring-boot:run -o   
[INFO] Scanning for projects...
[INFO] 
[INFO] ------------------------------------------------------------------------
[INFO] Building spring-data-performance 0.0.1-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO] 
[INFO] >>> spring-boot-maven-plugin:2.0.6.RELEASE:run (default-cli) > test-compile @ spring-data-performance >>>
[INFO] 
[INFO] --- gmavenplus-plugin:1.6.1:addTestSources (default) @ spring-data-performance ---
[INFO] 
[INFO] --- gmavenplus-plugin:1.6.1:addSources (default) @ spring-data-performance ---
[INFO] 
[INFO] --- build-helper-maven-plugin:1.5:add-source (add-source) @ spring-data-performance ---
[INFO] Source directory: /Users/rhasija/tmp/using-micronaut-in-spring-error/src/main/java added.
[INFO] Source directory: /Users/rhasija/tmp/using-micronaut-in-spring-error/src/main/groovy added.
[INFO] 
[INFO] --- maven-resources-plugin:3.0.2:resources (default-resources) @ spring-data-performance ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] Copying 0 resource
[INFO] 
[INFO] --- maven-compiler-plugin:3.7.0:compile (default-compile) @ spring-data-performance ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- gmavenplus-plugin:1.6.1:compile (default) @ spring-data-performance ---
[INFO] No sources specified for compilation.  Skipping.
[INFO] 
[INFO] --- build-helper-maven-plugin:1.5:add-test-source (add-test-source) @ spring-data-performance ---
[INFO] Test Source directory: /Users/rhasija/tmp/using-micronaut-in-spring-error/src/test/java added.
[INFO] Test Source directory: /Users/rhasija/tmp/using-micronaut-in-spring-error/src/test/groovy added.
[INFO] 
[INFO] --- maven-resources-plugin:3.0.2:testResources (default-testResources) @ spring-data-performance ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /Users/rhasija/tmp/using-micronaut-in-spring-error/src/test/resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.7.0:testCompile (default-testCompile) @ spring-data-performance ---
[INFO] No sources to compile
[INFO] 
[INFO] --- gmavenplus-plugin:1.6.1:compileTests (default) @ spring-data-performance ---
[INFO] No sources specified for compilation.  Skipping.
[INFO] 
[INFO] <<< spring-boot-maven-plugin:2.0.6.RELEASE:run (default-cli) < test-compile @ spring-data-performance <<<
[INFO] 
[INFO] 
[INFO] --- spring-boot-maven-plugin:2.0.6.RELEASE:run (default-cli) @ spring-data-performance ---

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v2.0.6.RELEASE)

2018-10-26 11:10:05.327  INFO 21865 --- [           main] exp.spring.data.performance.Application  : Starting Application on KAPAMAC12FMG3QD with PID 21865 (/Users/rhasija/tmp/using-micronaut-in-spring-error/target/classes started by rhasija in /Users/rhasija/tmp/using-micronaut-in-spring-error)
2018-10-26 11:10:05.330  INFO 21865 --- [           main] exp.spring.data.performance.Application  : The following profiles are active: production,development,mysql,datacenter
2018-10-26 11:10:05.379  INFO 21865 --- [           main] ConfigServletWebServerApplicationContext : Refreshing org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@3b743a1b: startup date [Fri Oct 26 11:10:05 PDT 2018]; root of context hierarchy
2018-10-26 11:10:06.277  WARN 21865 --- [           main] o.s.c.a.ConfigurationClassEnhancer       : @Bean method Application.beanProcessor is non-static and returns an object assignable to Spring's BeanFactoryPostProcessor interface. This will result in a failure to process annotations such as @Autowired, @Resource and @PostConstruct within the method's declaring @Configuration class. Add the 'static' modifier to this method to avoid these container lifecycle issues; see @Bean javadoc for complete details.
2018-10-26 11:10:06.790  INFO 21865 --- [           main] f.a.AutowiredAnnotationBeanPostProcessor : JSR-330 'javax.inject.Inject' annotation found and supported for autowiring
2018-10-26 11:10:06.823  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.reactive.rxjava2.RxJava2Instrumentation' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.823  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.validation.ValidatingInterceptor' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.824  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.http.resource.ResourceLoaderFactory' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.824  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.http.ssl.ServerSslConfiguration' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.824  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.core.io.scan.ClassPathResourceLoader' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.825  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.http.ssl.ClientSslConfiguration' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.825  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.http.MediaTypeConverter' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.825  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.core.io.ResourceResolver' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.826  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.http.ssl.DefaultSslConfiguration$DefaultKeyConfiguration' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.826  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.http.util.OutgoingHttpRequestProcessorImpl' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.827  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.http.codec.CodecConfiguration' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.827  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.core.io.file.FileSystemResourceLoader' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.828  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.http.bind.DefaultRequestBinderRegistry' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.828  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.http.ssl.DefaultSslConfiguration$DefaultKeyStoreConfiguration' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.829  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.http.ssl.DefaultSslConfiguration' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.830  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.http.ssl.DefaultSslConfiguration$DefaultTrustStoreConfiguration' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.830  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.runtime.http.converters.HttpStatusConverter' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.831  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.scheduling.executor.DefaultThreadFactory' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.831  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.discovery.config.DefaultCompositeConfigurationClient' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.831  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.jackson.serialize.ConvertibleValuesSerializer' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.832  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.http.codec.MediaTypeCodecRegistry' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.832  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.cache.DefaultSyncCache' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.833  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.scheduling.executor.ExecutorFactory' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.833  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.jackson.convert.ArrayNodeToArrayConverter' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.833  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.scheduling.executor.DefaultExecutorSelector' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.834  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.discovery.DefaultServiceInstanceIdGenerator' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.834  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.jackson.serialize.ResourceModule' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.834  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.scheduling.executor.ExecutorConfiguration' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.835  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.cache.DefaultCacheManager' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.835  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.scheduling.DefaultTaskExceptionHandler' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.835  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.jackson.convert.ObjectToJsonNodeConverter' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.836  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.jackson.bind.MapToObjectConverter' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.836  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.jackson.ObjectMapperFactory' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.836  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.cache.interceptor.CacheInterceptor' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.842  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.jackson.bind.JacksonBeanPropertyBinder' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.842  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.jackson.codec.JsonStreamMediaTypeCodec' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.842  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.scheduling.async.AsyncInterceptor' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.843  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.runtime.context.scope.refresh.RefreshScope' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.843  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.jackson.convert.ArrayNodeToIterableConverter' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.846  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.discovery.DefaultCompositeDiscoveryClient' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.847  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.reactive.rxjava2.converters.RxJavaConverterRegistrar' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.847  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.scheduling.executor.ScheduledExecutorServiceConfig' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.847  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.retry.intercept.RecoveryInterceptor' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.848  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.runtime.ApplicationConfiguration$InstanceConfiguration' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.848  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.runtime.http.codec.TextPlainCodec' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.848  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.runtime.converters.time.TimeConverterRegistrar' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.848  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'java.util.concurrent.ThreadFactory' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.849  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.health.DefaultCurrentHealthStatus' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.849  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.jackson.serialize.OptionalValuesSerializer' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.849  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.health.HeartbeatConfiguration' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.850  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.jackson.codec.JsonMediaTypeCodec' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.850  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'java.util.concurrent.ExecutorService' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.851  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.jackson.JacksonConfiguration' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.851  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.jackson.serialize.ResourceSerializerModifier' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.852  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.runtime.context.scope.ThreadLocalCustomScope' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.852  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.scheduling.executor.IOExecutorServiceConfig' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.852  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.jackson.convert.ObjectNodeToConvertibleValuesConverter' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.853  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.cache.DefaultCacheErrorHandler' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.853  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.cache.AsyncCacheErrorHandler' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.853  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.runtime.ApplicationConfiguration' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.854  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.cache.CacheConfiguration' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.854  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.jackson.serialize.JacksonObjectSerializer' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.854  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'com.fasterxml.jackson.databind.ObjectMapper' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.855  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.jackson.serialize.ConvertibleMultiValuesSerializer' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.855  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.scheduling.processor.ScheduledMethodProcessor' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.855  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.jackson.convert.JsonNodeToObjectConverter' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.856  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.retry.intercept.DefaultRetryInterceptor' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.856  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.scheduling.executor.UserExecutorConfiguration' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.856  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.runtime.context.scope.refresh.RefreshInterceptor' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.857  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.runtime.http.codec.MediaTypeCodecRegistryFactory' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.857  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'org.springframework.jdbc.datasource.DataSourceTransactionManager' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.858  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.spring.tx.datasource.DataSourceTransactionManagerFactory' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.858  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.spring.tx.annotation.TransactionInterceptor' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.858  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'io.micronaut.spring.tx.datasource.DataSourceTransactionManagerFactory$TransactionAwareDataSourceListener' of type [io.micronaut.spring.beans.MicronautSpringBeanFactory] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:06.937  INFO 21865 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'org.springframework.transaction.annotation.ProxyTransactionManagementConfiguration' of type [org.springframework.transaction.annotation.ProxyTransactionManagementConfiguration$$EnhancerBySpringCGLIB$$6a31a7be] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2018-10-26 11:10:07.296  INFO 21865 --- [           main] o.s.b.w.embedded.tomcat.TomcatWebServer  : Tomcat initialized with port(s): 8080 (http)
2018-10-26 11:10:07.323  INFO 21865 --- [           main] o.apache.catalina.core.StandardService   : Starting service [Tomcat]
2018-10-26 11:10:07.323  INFO 21865 --- [           main] org.apache.catalina.core.StandardEngine  : Starting Servlet Engine: Apache Tomcat/8.5.34
2018-10-26 11:10:07.335  INFO 21865 --- [ost-startStop-1] o.a.catalina.core.AprLifecycleListener   : The APR based Apache Tomcat Native library which allows optimal performance in production environments was not found on the java.library.path: [/Users/rhasija/Library/Java/Extensions:/Library/Java/Extensions:/Network/Library/Java/Extensions:/System/Library/Java/Extensions:/usr/lib/java:.]
2018-10-26 11:10:07.421  INFO 21865 --- [ost-startStop-1] o.a.c.c.C.[.[localhost].[/spring]        : Initializing Spring embedded WebApplicationContext
2018-10-26 11:10:07.421  INFO 21865 --- [ost-startStop-1] o.s.web.context.ContextLoader            : Root WebApplicationContext: initialization completed in 2045 ms
2018-10-26 11:10:07.489  INFO 21865 --- [ost-startStop-1] o.s.b.w.servlet.ServletRegistrationBean  : Servlet dispatcherServlet mapped to [/]
2018-10-26 11:10:07.493  INFO 21865 --- [ost-startStop-1] o.s.b.w.servlet.FilterRegistrationBean   : Mapping filter: 'characterEncodingFilter' to: [/*]
2018-10-26 11:10:07.493  INFO 21865 --- [ost-startStop-1] o.s.b.w.servlet.FilterRegistrationBean   : Mapping filter: 'hiddenHttpMethodFilter' to: [/*]
2018-10-26 11:10:07.493  INFO 21865 --- [ost-startStop-1] o.s.b.w.servlet.FilterRegistrationBean   : Mapping filter: 'httpPutFormContentFilter' to: [/*]
2018-10-26 11:10:07.493  INFO 21865 --- [ost-startStop-1] o.s.b.w.servlet.FilterRegistrationBean   : Mapping filter: 'requestContextFilter' to: [/*]
2018-10-26 11:10:07.637  INFO 21865 --- [           main] com.zaxxer.hikari.HikariDataSource       : HikariPool-1 - Starting...
2018-10-26 11:10:07.953  INFO 21865 --- [           main] com.zaxxer.hikari.HikariDataSource       : HikariPool-1 - Start completed.
2018-10-26 11:10:08.002  INFO 21865 --- [           main] j.LocalContainerEntityManagerFactoryBean : Building JPA container EntityManagerFactory for persistence unit 'default'
2018-10-26 11:10:08.018  INFO 21865 --- [           main] o.hibernate.jpa.internal.util.LogHelper  : HHH000204: Processing PersistenceUnitInfo [
        name: default
        ...]
2018-10-26 11:10:08.084  INFO 21865 --- [           main] org.hibernate.Version                    : HHH000412: Hibernate Core {5.2.17.Final}
2018-10-26 11:10:08.085  INFO 21865 --- [           main] org.hibernate.cfg.Environment            : HHH000206: hibernate.properties not found
2018-10-26 11:10:08.119  INFO 21865 --- [           main] o.hibernate.annotations.common.Version   : HCANN000001: Hibernate Commons Annotations {5.0.1.Final}
2018-10-26 11:10:08.226  INFO 21865 --- [           main] org.hibernate.dialect.Dialect            : HHH000400: Using dialect: org.hibernate.dialect.H2Dialect
2018-10-26 11:10:08.635  INFO 21865 --- [           main] o.h.t.schema.internal.SchemaCreatorImpl  : HHH000476: Executing import script 'org.hibernate.tool.schema.internal.exec.ScriptSourceInputNonExistentImpl@261e793c'
2018-10-26 11:10:08.638  INFO 21865 --- [           main] j.LocalContainerEntityManagerFactoryBean : Initialized JPA EntityManagerFactory for persistence unit 'default'
2018-10-26 11:10:08.919  INFO 21865 --- [           main] o.s.w.s.handler.SimpleUrlHandlerMapping  : Mapped URL path [/**/favicon.ico] onto handler of type [class org.springframework.web.servlet.resource.ResourceHttpRequestHandler]
2018-10-26 11:10:09.154  INFO 21865 --- [           main] s.w.s.m.m.a.RequestMappingHandlerAdapter : Looking for @ControllerAdvice: org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@3b743a1b: startup date [Fri Oct 26 11:10:05 PDT 2018]; root of context hierarchy
2018-10-26 11:10:09.204  WARN 21865 --- [           main] aWebConfiguration$JpaWebMvcConfiguration : spring.jpa.open-in-view is enabled by default. Therefore, database queries may be performed during view rendering. Explicitly configure spring.jpa.open-in-view to disable this warning
2018-10-26 11:10:09.246  INFO 21865 --- [           main] s.w.s.m.m.a.RequestMappingHandlerMapping : Mapped "{[/person/{id}],methods=[GET]}" onto exp.spring.data.performance.domain.Person exp.spring.data.performance.rest.PersonController.getPerson(java.lang.Long)
2018-10-26 11:10:09.251  INFO 21865 --- [           main] s.w.s.m.m.a.RequestMappingHandlerMapping : Mapped "{[/error]}" onto public org.springframework.http.ResponseEntity<java.util.Map<java.lang.String, java.lang.Object>> org.springframework.boot.autoconfigure.web.servlet.error.BasicErrorController.error(javax.servlet.http.HttpServletRequest)
2018-10-26 11:10:09.251  INFO 21865 --- [           main] s.w.s.m.m.a.RequestMappingHandlerMapping : Mapped "{[/error],produces=[text/html]}" onto public org.springframework.web.servlet.ModelAndView org.springframework.boot.autoconfigure.web.servlet.error.BasicErrorController.errorHtml(javax.servlet.http.HttpServletRequest,javax.servlet.http.HttpServletResponse)
2018-10-26 11:10:09.287  INFO 21865 --- [           main] o.s.w.s.handler.SimpleUrlHandlerMapping  : Mapped URL path [/webjars/**] onto handler of type [class org.springframework.web.servlet.resource.ResourceHttpRequestHandler]
2018-10-26 11:10:09.287  INFO 21865 --- [           main] o.s.w.s.handler.SimpleUrlHandlerMapping  : Mapped URL path [/**] onto handler of type [class org.springframework.web.servlet.resource.ResourceHttpRequestHandler]
2018-10-26 11:10:09.497  WARN 21865 --- [           main] ConfigServletWebServerApplicationContext : Exception encountered during context initialization - cancelling refresh attempt: org.springframework.beans.factory.UnsatisfiedDependencyException: Error creating bean with name 'org.springframework.boot.autoconfigure.transaction.TransactionAutoConfiguration$TransactionTemplateConfiguration': Unsatisfied dependency expressed through constructor parameter 0; nested exception is org.springframework.beans.factory.BeanCreationException: Error creating bean with name 'org.springframework.jdbc.datasource.DataSourceTransactionManager': FactoryBean threw exception on object creation; nested exception is io.micronaut.context.exceptions.BeanInstantiationException: Could Not Create Bean [class org.springframework.jdbc.datasource.DataSourceTransactionManager]
2018-10-26 11:10:09.497  INFO 21865 --- [           main] o.s.j.e.a.AnnotationMBeanExporter        : Unregistering JMX-exposed beans on shutdown
2018-10-26 11:10:09.499  INFO 21865 --- [           main] j.LocalContainerEntityManagerFactoryBean : Closing JPA EntityManagerFactory for persistence unit 'default'
2018-10-26 11:10:09.499  INFO 21865 --- [           main] .SchemaDropperImpl$DelayedDropActionImpl : HHH000477: Starting delayed drop of schema as part of SessionFactory shut-down'
2018-10-26 11:10:09.505  INFO 21865 --- [           main] com.zaxxer.hikari.HikariDataSource       : HikariPool-1 - Shutdown initiated...
2018-10-26 11:10:09.510  INFO 21865 --- [           main] com.zaxxer.hikari.HikariDataSource       : HikariPool-1 - Shutdown completed.
2018-10-26 11:10:09.513  INFO 21865 --- [           main] o.apache.catalina.core.StandardService   : Stopping service [Tomcat]
2018-10-26 11:10:09.531  INFO 21865 --- [           main] ConditionEvaluationReportLoggingListener : 

Error starting ApplicationContext. To display the conditions report re-run your application with 'debug' enabled.
2018-10-26 11:10:09.540 ERROR 21865 --- [           main] o.s.boot.SpringApplication               : Application run failed

org.springframework.beans.factory.UnsatisfiedDependencyException: Error creating bean with name 'org.springframework.boot.autoconfigure.transaction.TransactionAutoConfiguration$TransactionTemplateConfiguration': Unsatisfied dependency expressed through constructor parameter 0; nested exception is org.springframework.beans.factory.BeanCreationException: Error creating bean with name 'org.springframework.jdbc.datasource.DataSourceTransactionManager': FactoryBean threw exception on object creation; nested exception is io.micronaut.context.exceptions.BeanInstantiationException: Could Not Create Bean [class org.springframework.jdbc.datasource.DataSourceTransactionManager]
        at org.springframework.beans.factory.support.ConstructorResolver.createArgumentArray(ConstructorResolver.java:733) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.ConstructorResolver.autowireConstructor(ConstructorResolver.java:198) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.autowireConstructor(AbstractAutowireCapableBeanFactory.java:1266) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.createBeanInstance(AbstractAutowireCapableBeanFactory.java:1123) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.doCreateBean(AbstractAutowireCapableBeanFactory.java:535) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.createBean(AbstractAutowireCapableBeanFactory.java:495) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.AbstractBeanFactory.lambda$doGetBean$0(AbstractBeanFactory.java:317) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.DefaultSingletonBeanRegistry.getSingleton(DefaultSingletonBeanRegistry.java:222) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.AbstractBeanFactory.doGetBean(AbstractBeanFactory.java:315) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.AbstractBeanFactory.getBean(AbstractBeanFactory.java:199) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.DefaultListableBeanFactory.preInstantiateSingletons(DefaultListableBeanFactory.java:759) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.context.support.AbstractApplicationContext.finishBeanFactoryInitialization(AbstractApplicationContext.java:867) ~[spring-context-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.context.support.AbstractApplicationContext.refresh(AbstractApplicationContext.java:548) ~[spring-context-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.boot.web.servlet.context.ServletWebServerApplicationContext.refresh(ServletWebServerApplicationContext.java:140) ~[spring-boot-2.0.6.RELEASE.jar:2.0.6.RELEASE]
        at org.springframework.boot.SpringApplication.refresh(SpringApplication.java:754) [spring-boot-2.0.6.RELEASE.jar:2.0.6.RELEASE]
        at org.springframework.boot.SpringApplication.refreshContext(SpringApplication.java:386) [spring-boot-2.0.6.RELEASE.jar:2.0.6.RELEASE]
        at org.springframework.boot.SpringApplication.run(SpringApplication.java:307) [spring-boot-2.0.6.RELEASE.jar:2.0.6.RELEASE]
        at org.springframework.boot.SpringApplication.run(SpringApplication.java:1242) [spring-boot-2.0.6.RELEASE.jar:2.0.6.RELEASE]
        at org.springframework.boot.SpringApplication.run(SpringApplication.java:1230) [spring-boot-2.0.6.RELEASE.jar:2.0.6.RELEASE]
        at exp.spring.data.performance.Application.main(Application.java:21) [classes/:na]
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[na:1.8.0_162]
        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[na:1.8.0_162]
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[na:1.8.0_162]
        at java.lang.reflect.Method.invoke(Method.java:498) ~[na:1.8.0_162]
        at org.springframework.boot.maven.AbstractRunMojo$LaunchRunner.run(AbstractRunMojo.java:497) [spring-boot-maven-plugin-2.0.6.RELEASE.jar:2.0.6.RELEASE]
        at java.lang.Thread.run(Thread.java:748) [na:1.8.0_162]
Caused by: org.springframework.beans.factory.BeanCreationException: Error creating bean with name 'org.springframework.jdbc.datasource.DataSourceTransactionManager': FactoryBean threw exception on object creation; nested exception is io.micronaut.context.exceptions.BeanInstantiationException: Could Not Create Bean [class org.springframework.jdbc.datasource.DataSourceTransactionManager]
        at org.springframework.beans.factory.support.FactoryBeanRegistrySupport.doGetObjectFromFactoryBean(FactoryBeanRegistrySupport.java:178) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.FactoryBeanRegistrySupport.getObjectFromFactoryBean(FactoryBeanRegistrySupport.java:101) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.AbstractBeanFactory.getObjectForBeanInstance(AbstractBeanFactory.java:1644) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.getObjectForBeanInstance(AbstractAutowireCapableBeanFactory.java:1174) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.AbstractBeanFactory.doGetBean(AbstractBeanFactory.java:257) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.AbstractBeanFactory.getBean(AbstractBeanFactory.java:199) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.config.DependencyDescriptor.resolveCandidate(DependencyDescriptor.java:251) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.DefaultListableBeanFactory.addCandidateEntry(DefaultListableBeanFactory.java:1322) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.DefaultListableBeanFactory.findAutowireCandidates(DefaultListableBeanFactory.java:1288) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.DefaultListableBeanFactory.doResolveDependency(DefaultListableBeanFactory.java:1098) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.DefaultListableBeanFactory.resolveDependency(DefaultListableBeanFactory.java:1062) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.ConstructorResolver.resolveAutowiredArgument(ConstructorResolver.java:819) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        at org.springframework.beans.factory.support.ConstructorResolver.createArgumentArray(ConstructorResolver.java:725) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        ... 25 common frames omitted
Caused by: io.micronaut.context.exceptions.BeanInstantiationException: Could Not Create Bean [class org.springframework.jdbc.datasource.DataSourceTransactionManager]
        at io.micronaut.spring.beans.MicronautSpringBeanFactory.getObject(MicronautSpringBeanFactory.java:67) ~[micronaut-spring-1.0.0.jar:1.0.0]
        at org.springframework.beans.factory.support.FactoryBeanRegistrySupport.doGetObjectFromFactoryBean(FactoryBeanRegistrySupport.java:171) ~[spring-beans-5.0.10.RELEASE.jar:5.0.10.RELEASE]
        ... 37 common frames omitted

[WARNING] 
java.lang.reflect.InvocationTargetException
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.lang.reflect.Method.invoke(Method.java:498)
        at org.springframework.boot.maven.AbstractRunMojo$LaunchRunner.run(AbstractRunMojo.java:497)
        at java.lang.Thread.run(Thread.java:748)
Caused by: org.springframework.beans.factory.UnsatisfiedDependencyException: Error creating bean with name 'org.springframework.boot.autoconfigure.transaction.TransactionAutoConfiguration$TransactionTemplateConfiguration': Unsatisfied dependency expressed through constructor parameter 0; nested exception is org.springframework.beans.factory.BeanCreationException: Error creating bean with name 'org.springframework.jdbc.datasource.DataSourceTransactionManager': FactoryBean threw exception on object creation; nested exception is io.micronaut.context.exceptions.BeanInstantiationException: Could Not Create Bean [class org.springframework.jdbc.datasource.DataSourceTransactionManager]
        at org.springframework.beans.factory.support.ConstructorResolver.createArgumentArray(ConstructorResolver.java:733)
        at org.springframework.beans.factory.support.ConstructorResolver.autowireConstructor(ConstructorResolver.java:198)
        at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.autowireConstructor(AbstractAutowireCapableBeanFactory.java:1266)
        at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.createBeanInstance(AbstractAutowireCapableBeanFactory.java:1123)
        at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.doCreateBean(AbstractAutowireCapableBeanFactory.java:535)
        at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.createBean(AbstractAutowireCapableBeanFactory.java:495)
        at org.springframework.beans.factory.support.AbstractBeanFactory.lambda$doGetBean$0(AbstractBeanFactory.java:317)
        at org.springframework.beans.factory.support.DefaultSingletonBeanRegistry.getSingleton(DefaultSingletonBeanRegistry.java:222)
        at org.springframework.beans.factory.support.AbstractBeanFactory.doGetBean(AbstractBeanFactory.java:315)
        at org.springframework.beans.factory.support.AbstractBeanFactory.getBean(AbstractBeanFactory.java:199)
        at org.springframework.beans.factory.support.DefaultListableBeanFactory.preInstantiateSingletons(DefaultListableBeanFactory.java:759)
        at org.springframework.context.support.AbstractApplicationContext.finishBeanFactoryInitialization(AbstractApplicationContext.java:867)
        at org.springframework.context.support.AbstractApplicationContext.refresh(AbstractApplicationContext.java:548)
        at org.springframework.boot.web.servlet.context.ServletWebServerApplicationContext.refresh(ServletWebServerApplicationContext.java:140)
        at org.springframework.boot.SpringApplication.refresh(SpringApplication.java:754)
        at org.springframework.boot.SpringApplication.refreshContext(SpringApplication.java:386)
        at org.springframework.boot.SpringApplication.run(SpringApplication.java:307)
        at org.springframework.boot.SpringApplication.run(SpringApplication.java:1242)
        at org.springframework.boot.SpringApplication.run(SpringApplication.java:1230)
        at exp.spring.data.performance.Application.main(Application.java:21)
        ... 6 more
Caused by: org.springframework.beans.factory.BeanCreationException: Error creating bean with name 'org.springframework.jdbc.datasource.DataSourceTransactionManager': FactoryBean threw exception on object creation; nested exception is io.micronaut.context.exceptions.BeanInstantiationException: Could Not Create Bean [class org.springframework.jdbc.datasource.DataSourceTransactionManager]
        at org.springframework.beans.factory.support.FactoryBeanRegistrySupport.doGetObjectFromFactoryBean(FactoryBeanRegistrySupport.java:178)
        at org.springframework.beans.factory.support.FactoryBeanRegistrySupport.getObjectFromFactoryBean(FactoryBeanRegistrySupport.java:101)
        at org.springframework.beans.factory.support.AbstractBeanFactory.getObjectForBeanInstance(AbstractBeanFactory.java:1644)
        at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.getObjectForBeanInstance(AbstractAutowireCapableBeanFactory.java:1174)
        at org.springframework.beans.factory.support.AbstractBeanFactory.doGetBean(AbstractBeanFactory.java:257)
        at org.springframework.beans.factory.support.AbstractBeanFactory.getBean(AbstractBeanFactory.java:199)
        at org.springframework.beans.factory.config.DependencyDescriptor.resolveCandidate(DependencyDescriptor.java:251)
        at org.springframework.beans.factory.support.DefaultListableBeanFactory.addCandidateEntry(DefaultListableBeanFactory.java:1322)
        at org.springframework.beans.factory.support.DefaultListableBeanFactory.findAutowireCandidates(DefaultListableBeanFactory.java:1288)
        at org.springframework.beans.factory.support.DefaultListableBeanFactory.doResolveDependency(DefaultListableBeanFactory.java:1098)
        at org.springframework.beans.factory.support.DefaultListableBeanFactory.resolveDependency(DefaultListableBeanFactory.java:1062)
        at org.springframework.beans.factory.support.ConstructorResolver.resolveAutowiredArgument(ConstructorResolver.java:819)
        at org.springframework.beans.factory.support.ConstructorResolver.createArgumentArray(ConstructorResolver.java:725)
        ... 25 more
Caused by: io.micronaut.context.exceptions.BeanInstantiationException: Could Not Create Bean [class org.springframework.jdbc.datasource.DataSourceTransactionManager]
        at io.micronaut.spring.beans.MicronautSpringBeanFactory.getObject(MicronautSpringBeanFactory.java:67)
        at org.springframework.beans.factory.support.FactoryBeanRegistrySupport.doGetObjectFromFactoryBean(FactoryBeanRegistrySupport.java:171)
        ... 37 more
[INFO] ------------------------------------------------------------------------
[INFO] BUILD FAILURE
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 6.510 s
[INFO] Finished at: 2018-10-26T11:10:09-07:00
[INFO] Final Memory: 45M/450M
[INFO] ------------------------------------------------------------------------
[ERROR] Failed to execute goal org.springframework.boot:spring-boot-maven-plugin:2.0.6.RELEASE:run (default-cli) on project spring-data-performance: An exception occurred while running. null: InvocationTargetException: Error creating bean with name 'org.springframework.boot.autoconfigure.transaction.TransactionAutoConfiguration$TransactionTemplateConfiguration': Unsatisfied dependency expressed through constructor parameter 0; nested exception is org.springframework.beans.factory.BeanCreationException: Error creating bean with name 'org.springframework.jdbc.datasource.DataSourceTransactionManager': FactoryBean threw exception on object creation; nested exception is io.micronaut.context.exceptions.BeanInstantiationException: Could Not Create Bean [class org.springframework.jdbc.datasource.DataSourceTransactionManager] -> [Help 1]
[ERROR] 
[ERROR] To see the full stack trace of the errors, re-run Maven with the -e switch.
[ERROR] Re-run Maven using the -X switch to enable full debug logging.
[ERROR] 
[ERROR] For more information about the errors and possible solutions, please read the following articles:
[ERROR] [Help 1] http://cwiki.apache.org/confluence/display/MAVEN/MojoExecutionException
```