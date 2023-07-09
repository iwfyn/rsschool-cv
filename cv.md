# Dzima Bykau

## Contact information

**Location:** Minsk, Belarus  
**E-mail:** <bykovdmitry3@gmail.com>  
**Discord:** @iwfyn  
[Linkedin](www.linkedin.com/in/dzima-bykau-ab3903229) [GitHub](https://github.com/iwfyn)

## Summary

Sport is the sphere of my professional interests. Having a qualification of "trainer-teacher" in modern pentathlon, I am engaged, among other things, in scientific research in the field of sports biomechanics. I actively contribute to the dissemination and use of modern achievements in this direction among the national teams of the Republic of Belarus in various sports: speed skating, rowing and canoeing, etc.

In one of the recent projects, not only in word, but also in deed, I oversaw the selection of children aged 5-12 years old to the school of the Minsk golf club. Recently, I have been increasingly studying the problems associated with the identification and development of sports talent in children, as well as their early sports specialization. Against the background of work in this direction, I had a very promising business idea.

During my studies at rs.school, I hope to systematically acquire new knowledge that will make it possible to implement many elements of this wonderful idea.

## Skills

* Matlab
* Git *(basic knowledge)*
* Figma *(basic knowledge)*

## Code example

```matlab
% Cycle time normalization 0-->100

norm_FORCE_DATA_F = [];
norm_FORCE_DATA_H = [];
norm_FORCE_DATA_M = [];
FORCE_DATA_normed = [];

for k = 1:NoS
    new_len = 0:99; % number of data values within a single cycle
    data_len = []; % a variable in which linearly distributed data values will be written in each of the motor cycles            
    for FHM = 1:3 % a variable that will determine the number of foot segments to order     (Foot, Heel, Metatarsal)
        data_len(FHM,:) = linspace(0,99,length(FORCE_DATA(fix(StartCycle(k)):fix(EndCycle(k)))));
        FORCE_DATA_normed(FHM,:) = spline(data_len(FHM,:), FORCE_DATA(fix(StartCycle(k)):fix(EndCycle(k)),FHM),new_len); % spline data on three segments of the foot (Foot, Heel, Metatarsal)
    end
    % recording of all normalized motor cycles for each segment in the corresponding variable
    norm_FORCE_DATA_F(:,k) = FORCE_DATA_normed(1,:);      
    norm_FORCE_DATA_H(:,k) = FORCE_DATA_normed(2,:);   
    norm_FORCE_DATA_M(:,k) = FORCE_DATA_normed(3,:);
end
```

## Education

* Belarusian National Technical University
  * 2016 - bachelor, major «Sports engineering»
  * 2017 - master's degree program, major «Methods and Facilities of Technical Support for Physical Education and Sports»
  * 2020 - doctoral degree program, major «Methods and Facilities of Technical Support for Physical Education and Sports»

* Courses
  * Skills for All by Cisco:
    * Networking Basics
    * Network Addressing and Basic Troubleshooting
    * Networking Devices and Initial Configuration
  * «JavaScript/Front-end. Stage 0» by rs.school (in progress)

## Languages

* English (A2+)
* Russian (Native)
* Belarusian (Native)
