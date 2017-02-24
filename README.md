# eclipse-drmaa-v1
Preparation for eclipse CQ of DRMAA v1 and an SGE impl

This repo is a temporary location for the org.ggf.drmaa and com.sun.grid.drmaa bundles as submitted in Eclipse CQs :
* [CQ 12473] org.ggf.drmaa 1.0
* [CQ 12474] com.sun.grid.drmaa 1.0

The code is only slightly adapted from its origin at https://arc.liv.ac.uk/trac/SGE :
* In a first phase it was adapted to OSGi bundles in the scope of the [DAWN](http://dawnsci.org/) project of Diamond LS. Sources are at https://github.com/DawnScience/dawn-hpc :
  * add bundle metadata files (MANIFEST, DS components + eclipse project files)
  * add a org.ggf.drmaa.SessionFactory.setFactory(SessionFactory), com.sun.grid.drmaa.SessionFactoryImpl.(de)activate() to allow setting/unsetting the initialized instance via OSGi DS (de)activation
  * style/syntax things : 
    * define generic types for collections used in the API
    * style corrections in usage of constants in PartialTimestampFormat
  
* For submission as Eclipse approved artifacts, only some Javadoc additions were done

The license is unchanged from the original SISSL.
