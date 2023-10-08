# DAT250: Assignment 5
By 587900 (Kjetil Berg)

### Description
The instructions of https://github.com/selabhvl/dat250public/blob/master/expassignments/expass5.md were followed gain experience with Spring Boot.
During the process we could decide to use gradle or maven. I opted for maven since I am relatively experienced with it.
Everything went according to the instructions besides what is mentioned under the 'Trials and tribulations' section (problems and noteworthy moments).

### Initial setup
During the first tutorial, I used Spring Initializr to set up the project. I used the same project (different packages) for each tutorial.

### Working status
After the trials and tribulations were resolved, here are the statuses:
1. Tutorial 1 outputted the expected results and worked properly (/hello), with and without query params.
2. Tutorial 2 outputted the expected results and worked properly (listing beans, curling, both tests pass, /actuator and /actuator/health).
3. Tutorial 3 outputted the expected results and worked properly (dynamic greeting and static file).
4. Tutorial 4 outputted the expected results and worked properly (JPA / Data storage and requests, all, by id and by last name).

### Tutorial 2 outputted beans
The following was outputted from tutorial 2:
```
Let's inspect the beans provided by Spring Boot:
application
applicationAvailability
applicationTaskExecutor
basicErrorController
beanNameHandlerMapping
beanNameViewResolver
characterEncodingFilter
commandLineRunner
conventionErrorViewResolver
defaultServletHandlerMapping
defaultViewResolver
dispatcherServlet
dispatcherServletRegistration
error
errorAttributes
errorPageCustomizer
errorPageRegistrarBeanPostProcessor
flashMapManager
forceAutoProxyCreatorToUseClassProxying
formContentFilter
handlerExceptionResolver
handlerFunctionAdapter
helloController
httpRequestHandlerAdapter
jacksonObjectMapper
jacksonObjectMapperBuilder
jsonComponentModule
jsonMixinModule
jsonMixinModuleEntries
lifecycleProcessor
localeCharsetMappingsCustomizer
localeResolver
mappingJackson2HttpMessageConverter
messageConverters
multipartConfigElement
multipartResolver
mvcContentNegotiationManager
mvcConversionService
mvcHandlerMappingIntrospector
mvcPathMatcher
mvcPatternParser
mvcResourceUrlProvider
mvcUriComponentsContributor
mvcUrlPathHelper
mvcValidator
mvcViewResolver
org.springframework.aop.config.internalAutoProxyCreator
org.springframework.boot.autoconfigure.AutoConfigurationPackages
org.springframework.boot.autoconfigure.aop.AopAutoConfiguration
org.springframework.boot.autoconfigure.aop.AopAutoConfiguration$ClassProxyingConfiguration
org.springframework.boot.autoconfigure.availability.ApplicationAvailabilityAutoConfiguration
org.springframework.boot.autoconfigure.context.ConfigurationPropertiesAutoConfiguration
org.springframework.boot.autoconfigure.context.LifecycleAutoConfiguration
org.springframework.boot.autoconfigure.context.PropertyPlaceholderAutoConfiguration
org.springframework.boot.autoconfigure.http.HttpMessageConvertersAutoConfiguration
org.springframework.boot.autoconfigure.http.HttpMessageConvertersAutoConfiguration$StringHttpMessageConverterConfiguration
org.springframework.boot.autoconfigure.http.JacksonHttpMessageConvertersConfiguration
org.springframework.boot.autoconfigure.http.JacksonHttpMessageConvertersConfiguration$MappingJackson2HttpMessageConverterConfiguration
org.springframework.boot.autoconfigure.info.ProjectInfoAutoConfiguration
org.springframework.boot.autoconfigure.internalCachingMetadataReaderFactory
org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration
org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$Jackson2ObjectMapperBuilderCustomizerConfiguration
org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$JacksonMixinConfiguration
org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$JacksonObjectMapperBuilderConfiguration
org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$JacksonObjectMapperConfiguration
org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$ParameterNamesModuleConfiguration
org.springframework.boot.autoconfigure.sql.init.SqlInitializationAutoConfiguration
org.springframework.boot.autoconfigure.ssl.SslAutoConfiguration
org.springframework.boot.autoconfigure.task.TaskExecutionAutoConfiguration
org.springframework.boot.autoconfigure.task.TaskSchedulingAutoConfiguration
org.springframework.boot.autoconfigure.web.client.RestTemplateAutoConfiguration
org.springframework.boot.autoconfigure.web.embedded.EmbeddedWebServerFactoryCustomizerAutoConfiguration
org.springframework.boot.autoconfigure.web.embedded.EmbeddedWebServerFactoryCustomizerAutoConfiguration$TomcatWebServerFactoryCustomizerConfiguration
org.springframework.boot.autoconfigure.web.servlet.DispatcherServletAutoConfiguration
org.springframework.boot.autoconfigure.web.servlet.DispatcherServletAutoConfiguration$DispatcherServletConfiguration
org.springframework.boot.autoconfigure.web.servlet.DispatcherServletAutoConfiguration$DispatcherServletRegistrationConfiguration
org.springframework.boot.autoconfigure.web.servlet.HttpEncodingAutoConfiguration
org.springframework.boot.autoconfigure.web.servlet.MultipartAutoConfiguration
org.springframework.boot.autoconfigure.web.servlet.ServletWebServerFactoryAutoConfiguration
org.springframework.boot.autoconfigure.web.servlet.ServletWebServerFactoryConfiguration$EmbeddedTomcat
org.springframework.boot.autoconfigure.web.servlet.WebMvcAutoConfiguration
org.springframework.boot.autoconfigure.web.servlet.WebMvcAutoConfiguration$EnableWebMvcConfiguration
org.springframework.boot.autoconfigure.web.servlet.WebMvcAutoConfiguration$WebMvcAutoConfigurationAdapter
org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration
org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration$DefaultErrorViewResolverConfiguration
org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration$WhitelabelErrorViewConfiguration
org.springframework.boot.autoconfigure.websocket.servlet.WebSocketServletAutoConfiguration
org.springframework.boot.autoconfigure.websocket.servlet.WebSocketServletAutoConfiguration$TomcatWebSocketConfiguration
org.springframework.boot.context.internalConfigurationPropertiesBinder
org.springframework.boot.context.properties.BoundConfigurationProperties
org.springframework.boot.context.properties.ConfigurationPropertiesBindingPostProcessor
org.springframework.boot.context.properties.EnableConfigurationPropertiesRegistrar.methodValidationExcludeFilter
org.springframework.boot.sql.init.dependency.DatabaseInitializationDependencyConfigurer$DependsOnDatabaseInitializationPostProcessor
org.springframework.context.annotation.internalAutowiredAnnotationProcessor
org.springframework.context.annotation.internalCommonAnnotationProcessor
org.springframework.context.annotation.internalConfigurationAnnotationProcessor
org.springframework.context.event.internalEventListenerFactory
org.springframework.context.event.internalEventListenerProcessor
parameterNamesModule
preserveErrorControllerTargetClassPostProcessor
propertySourcesPlaceholderConfigurer
requestContextFilter
requestMappingHandlerAdapter
requestMappingHandlerMapping
resourceHandlerMapping
restTemplateBuilder
restTemplateBuilderConfigurer
routerFunctionMapping
server-org.springframework.boot.autoconfigure.web.ServerProperties
servletWebServerFactoryCustomizer
simpleControllerHandlerAdapter
spring.info-org.springframework.boot.autoconfigure.info.ProjectInfoProperties
spring.jackson-org.springframework.boot.autoconfigure.jackson.JacksonProperties
spring.lifecycle-org.springframework.boot.autoconfigure.context.LifecycleProperties
spring.mvc-org.springframework.boot.autoconfigure.web.servlet.WebMvcProperties
spring.servlet.multipart-org.springframework.boot.autoconfigure.web.servlet.MultipartProperties
spring.sql.init-org.springframework.boot.autoconfigure.sql.init.SqlInitializationProperties
spring.ssl-org.springframework.boot.autoconfigure.ssl.SslProperties
spring.task.execution-org.springframework.boot.autoconfigure.task.TaskExecutionProperties
spring.task.scheduling-org.springframework.boot.autoconfigure.task.TaskSchedulingProperties
spring.web-org.springframework.boot.autoconfigure.web.WebProperties
sslBundleRegistry
sslPropertiesSslBundleRegistrar
standardJacksonObjectMapperBuilderCustomizer
stringHttpMessageConverter
taskExecutorBuilder
taskSchedulerBuilder
themeResolver
tomcatServletWebServerFactory
tomcatServletWebServerFactoryCustomizer
tomcatWebServerFactoryCustomizer
viewControllerHandlerMapping
viewNameTranslator
viewResolver
webServerFactoryCustomizerBeanPostProcessor
websocketServletWebServerCustomizer
welcomePageHandlerMapping
welcomePageNotAcceptableHandlerMapping
```

### Trials and tribulations
1. When setting up the project with Spring Initializr, I stumbled upon some hassle:\
   1.1 I accidentally installed the Java 17 version. Woopsies. I could have auto-installed a JDK with IntelliJ's auto-install feature, however I opted to use the Java 11 version instead.\
   1.2 After selecting Java 11 and re-downloading, the project still demanded Java 17. I **specifically** inspected the pom.xml file, and it stated "<java.version>17</java.version>". Why? Either use Java 11 or don't allow me to pick it, I say. Oh well. I resorted to auto-downloading JDK 21 with IntelliJ (OpenJDK release).
2. The first tutorial (not 2,3,4 though) did not specify how to run the project with maven (only gradle). I manually ran it with IntelliJ's inbuilt systems. Because I used the same project for all tutorials (and each tutorial had their own Main class), configuring maven run would be cumbersome, so I skipped it and just used IntelliJ to run all projects (as opposed to `./mvn spring-boot:run`).
3. During tutorial 2, I was supposed to run a groovy program. To do that, I should have installed Spring CLI. I found it quite cumbersome, so I skipped it.\
   3.1 I tried downloading it, and the instructions clearly stated it required Java 1.8 (Java 8) to run. It did not. I have Java 8 installed and set as my JAVA_HOME and added to PATH, yet still the project complained that "it has been compiled by a more recent version of the Java Runtime (class file version 61.0)" which is Java 17.\
   3.2 I am using Java on my home PC for other things, so I don't want to start messing about changing JDKs. Especially in highlight of Oracle's license changes (I'm not sure how Oracle's licensing affects other implementations like OpenJDK's, since Oracle is the "owner" of Java).\
   3.3 I cannot manually define another java.exe to use, the JAVA_HOME is targetted by a binary file (spring from spring CLI).\
   3.4 In short, they say it runs with groovy, I believe them. I still added the file to the project (I named it .groovyx so that IntelliJ wouldn't confuse the project and state "no groovy engine defined for this project" during building or running).
4. During tutorial 2 and 3, I was supposed to build an executable jar with gradle or maven.\
   4.1 They both target JAVA_HOME. I could modify the maven script to use another java.exe but:\
   4.2 Again, I have multiple Main classes in this project, so defining a build method wouldn't be straight forward (maybe easier for an expert at maven or gradle).\
   4.3 I can just use IntelliJ to build the projects using artifacts. This works, however there is a problem: The built application runs, but immediately closes after starting up. It outputs everything expected, like "project started in 1200ms", and then closes. No errors. I am sure this could be fixed by doing some configuration, but I did not figure anything out.
5. During tutorial 3, I had to manually find and install the thymeleaf and spring-devtools maven dependencies (since I did not use initializr). This went fine.\
   5.1. I did not observe spring-devtools do anything. It is a tool but it is also a library? I figured Spring might pick it up automatically, but nothing seemed to change. The tutorial did not say much about spring-devtools, and I did not investigate further.
6. Tutorial 4 brought a lot of pain.\
   6.1 First, I manually added Spring JPA and h2 database to my maven dependencies.\
   6.2 Some jakarta.persistence.xxx imports did not exist. I added another dependency: Jakarta Persistence API.\
   6.3 Following the tutorial, the program refused to run. The error was "No bean of type CustomerRepository can be found". Spring made a big point out of "If you extend CrudRepository then the implementation is auto-generated". Resolving this took a while, and eventually I resorted to:\
   6.4 A conversation with ChatGPT pointed out the error: There are **two** Spring-Boot-Jpa dependencies: spring-data-jpa and spring-boot-starter-data-jpa. Why? I am not sure. I am sure that Spring Initializr would not have given me this error, though.\
   6.5 I encountered another error. At least progress was being made. "Failed to determine a suitable driver class". I figured this was an incorrect persistence.xml. I went to Spring Initializr to make a dummy project I could copy it from ... but persistence.xml it is empty?? That should mean that even Spring Initializr would produce this error during the tutorial. I went to my group's polling-project and copied its persistence.xml (made some small modifications).\
   6.6 It still doesn't work? After some head-scratching, it seems that for some reason **this** spring project needs application.properties instead of persistence.xml? Our polling-project's application.properties is empty.
   ```Our polling-project uses Spring, this project uses Spring. Our polling-project needs persistence.xml, this project needs application.properties?```. By the way, Spring Initializr's application.properties is also empty, so point 6.5 is still valid. I asked ChatGPT to generate an application.properties file I could use. It needed some adjustment (from our old persistence.xml, copy the url=jbdc:h2:file:./DB).\
   6.7 After that, another error appears: Despite h2 being installed, org.h2.Driver was not found. Huh? I decided to peek inside the Initializr dummy project again, at its pom.xml file. There I found the proper dependencies (should have done this from the start). I noticed that the pom.xml only included the spring-boot-starter-data-jpa and not spring-data-jpa. Removing the latter (that I installed alone at first) seemed to have solved the problem. How does including an extra dependency make a class suddenly not exist!? Also, did Spring make two JPA dependencies just so if you pick the wrong one or both then your project doesn't work? What on earth.\
   6.8 Surprise! Another problem! This time it's... "Failed to execute CommandLineRunner" ... boils down to... "SQLGrammarException"? What? I decided to ask ChatGPT to transpile our old persistence.xml to an application.properties. After that the error went away and things worked properly. I think it was the spring.jpa.hibernate.ddl-auto=create flag that was missing.\
   6.9 The program finally runs as expected

### Conclusion
1. Most of the headache in 'Trials and tribulations' (point 6) could have been avoided if I had used Spring Initializr, or at least looked at its pom.xml / dependencies file earlier.
2. Do not trust Spring's Java versioning. Sources online says Spring 6 uses Java 17.
3. Realistically, projects would be kept separate so that gradle build or maven build could be used. I did not get to test this, but I am guessing they perform better than my buildings with artifacts.

### Outstanding problems
The built jar files close after starting their Spring environment. Some time spent investigating could probably solve this problem. Regardless, in a realistic setting, projects would be kept separate, and so gradle build / maven build would be used instead (pre-configured by Spring Initializr). So I do not consider this a big deal.
