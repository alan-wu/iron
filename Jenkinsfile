stage 'configure' 

parallel 'Slave1':{
	node('TestSlave1') {
		dir('./iron/src') {
		   	checkout([$class: 'GitSCM', branches: [[name: '*/JenkinsTest']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/alan-wu/iron.git']]])
	}
		echo 'Checked out'
		dir('./iron/build') {
sh '/home/opencmiss/cmake-3.4.3-Linux-x86_64/bin/cmake --no-warn-unused-cli -DCMAKE_BUILD_TYPE=RELEASE -DBUILD_PRECISION=sd -DBUILD_TESTS=ON -DCMAKE_PREFIX_PATH="/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_linux/gnu-C4.8-gnu-F4.8/no_mpi/release/cmake;/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_linux/gnu-C4.8-gnu-F4.8/openmpi_release/release/cmake" -DCMAKE_MODULE_PATH="/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/manage/CMakeScripts;/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/manage/Config;/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/manage;/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/cmake/OpenCMISSFindModuleWrappers;/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/manage/CMakeModules" -DFORTRAN_MANGLING=Add_ -DINT_TYPE=int32 -DPACKAGE_CONFIG_DIR=cmake -DCMAKE_NO_SYSTEM_FROM_IMPORTED=YES -DCMAKE_DEBUG_POSTFIX=d -DCMAKE_POSITION_INDEPENDENT_CODE=YES -DWARN_ALL=ON -DCHECK_ALL=ON -DWITH_PROFILING=NO -DCMAKE_INSTALL_DEFAULT_COMPONENT_NAME=Development -DCMAKE_C_FLAGS_RELEASE="-O3 -DNDEBUG -Ofast" -DCMAKE_C_FLAGS_DEBUG="-g -O0 -Wall" -DCMAKE_CXX_FLAGS_RELEASE="-O3 -DNDEBUG -Ofast" -DCMAKE_CXX_FLAGS_DEBUG="-g -O0 -Wall" -DCMAKE_Fortran_FLAGS_RELEASE="-O3 -Ofast" -DCMAKE_Fortran_FLAGS_DEBUG="-g -O0 -Wall -fbacktrace -Warray-temporaries -Wextra -Wsurprising -Wrealloc-lhs-all -finit-real=snan -fcheck=all" -DOC_SYSTEM_BLAS=ON -DOC_SYSTEM_BZIP2=OFF -DOC_SYSTEM_CELLML=OFF -DOC_SYSTEM_CLANG=OFF -DOC_SYSTEM_CSIM=OFF -DOC_SYSTEM_FIELDML-API=OFF -DOC_SYSTEM_FREETYPE=ON -DOC_SYSTEM_FTGL=OFF -DOC_SYSTEM_GDCM-ABI=OFF -DOC_SYSTEM_GLEW=OFF -DOC_SYSTEM_GTEST=OFF -DOC_SYSTEM_HDF5=OFF -DOC_SYSTEM_HYPRE=OFF -DOC_SYSTEM_IMAGEMAGICK=OFF -DOC_SYSTEM_IRON=OFF -DOC_SYSTEM_ITK=OFF -DOC_SYSTEM_JPEG=ON -DOC_SYSTEM_LAPACK=ON -DOC_SYSTEM_LIBCELLML=OFF -DOC_SYSTEM_LIBXML2=ON -DOC_SYSTEM_LLVM=OFF -DOC_SYSTEM_MUMPS=OFF -DOC_SYSTEM_NETGEN=OFF -DOC_SYSTEM_OPTPP=OFF -DOC_SYSTEM_PARMETIS=OFF -DOC_SYSTEM_PASTIX=OFF -DOC_SYSTEM_PETSC=OFF -DOC_SYSTEM_PLAPACK=OFF -DOC_SYSTEM_PNG=OFF -DOC_SYSTEM_PTSCOTCH=OFF -DOC_SYSTEM_SCALAPACK=OFF -DOC_SYSTEM_SCOTCH=OFF -DOC_SYSTEM_SLEPC=OFF -DOC_SYSTEM_SOWING=OFF -DOC_SYSTEM_SUITESPARSE=OFF -DOC_SYSTEM_SUNDIALS=OFF -DOC_SYSTEM_SUPERLU=OFF -DOC_SYSTEM_SUPERLU_DIST=OFF -DOC_SYSTEM_SZIP=OFF -DOC_SYSTEM_TIFF=OFF -DOC_SYSTEM_ZINC=OFF -DOC_SYSTEM_ZLIB=OFF -DCMAKE_INSTALL_RPATH="/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_linux/gnu-C4.8-gnu-F4.8/no_mpi/release/lib;/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_linux/gnu-C4.8-gnu-F4.8/openmpi_release/release/lib;/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_linux/gnu-C4.8-gnu-F4.8/mpi/openmpi/release/lib" -DCMAKE_INSTALL_RPATH_USE_LINK_PATH=TRUE -DCMAKE_INSTALL_PREFIX:STRING=/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_linux/gnu-C4.8-gnu-F4.8/openmpi_release/release -DBUILD_SHARED_LIBS=ON -DMPI=openmpi -DMPI_HOME=/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_linux/gnu-C4.8-gnu-F4.8/mpi/openmpi/release -DCMAKE_C_COMPILER=/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_linux/gnu-C4.8-gnu-F4.8/mpi/openmpi/release/bin/mpicc -DMPI_C_COMPILER=/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_linux/gnu-C4.8-gnu-F4.8/mpi/openmpi/release/bin/mpicc -DCMAKE_CXX_COMPILER=/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_linux/gnu-C4.8-gnu-F4.8/mpi/openmpi/release/bin/mpicxx -DMPI_CXX_COMPILER=/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_linux/gnu-C4.8-gnu-F4.8/mpi/openmpi/release/bin/mpicxx -DCMAKE_Fortran_COMPILER=/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_linux/gnu-C4.8-gnu-F4.8/mpi/openmpi/release/bin/mpifort -DMPI_Fortran_COMPILER=/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_linux/gnu-C4.8-gnu-F4.8/mpi/openmpi/release/bin/mpifort -DWITH_CELLML=ON -DCELLML_VERSION=1.0 -DLIBCELLML_VERSION=1.0 -DWITH_FIELDML=ON -DFIELDML-API_VERSION=0.5.0 -DWITH_HYPRE=ON -DHYPRE_VERSION=2.10.0 -DWITH_SUNDIALS=ON -DSUNDIALS_VERSION=2.5 -DWITH_MUMPS=ON -DMUMPS_VERSION=5.0.0 -DWITH_SCALAPACK=ON -DSCALAPACK_VERSION=2.8 -DWITH_PETSC=ON -DPETSC_VERSION=3.6.1 -DWITH_PROFILING=NO -DWITH_C_BINDINGS=ON -DWITH_Python_BINDINGS=ON -DINSTALL_TO_VIRTUALENV=/home/opencmiss/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_linux/gnu-C4.8-gnu-F4.8/openmpi_release/release/ -G"Unix Makefiles" ../src'
		}
		echo 'Configured'
	}
}, 'Slave2':{
	node('TestSlave2') {
		echo 'HPC Disabled'
	}
}, 'Slave3':{
	node('TestSlave3') {
		dir('./iron/src') {
		   	checkout([$class: 'GitSCM', branches: [[name: '*/JenkinsTest']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/alan-wu/iron.git']]])
		}
		echo 'Checked out'
		dir('./iron/build') {
			sh '/Users/mwu035/cmake-3.6.1/CMake.app/Contents/bin/cmake --no-warn-unused-cli -DCMAKE_BUILD_TYPE=RELEASE -DBUILD_PRECISION=sd -DBUILD_TESTS=OFF -DCMAKE_PREFIX_PATH="/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_darwin/clang-C6.0-gnu-F4.5/no_mpi/release/cmake;/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_darwin/clang-C6.0-gnu-F4.5/openmpi_release/release/cmake" -DCMAKE_MODULE_PATH="/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/manage/CMakeScripts;/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/manage/Config;/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/manage;/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/cmake/OpenCMISSFindModuleWrappers;/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/manage/CMakeModules" -DFORTRAN_MANGLING=Add_ -DINT_TYPE=int32 -DPACKAGE_CONFIG_DIR=cmake -DCMAKE_NO_SYSTEM_FROM_IMPORTED=YES -DCMAKE_DEBUG_POSTFIX=d -DCMAKE_POSITION_INDEPENDENT_CODE=YES -DWARN_ALL=ON -DCHECK_ALL=ON -DWITH_PROFILING=NO -DCMAKE_INSTALL_DEFAULT_COMPONENT_NAME=Development -DCMAKE_C_FLAGS_RELEASE="-O3 -DNDEBUG" -DCMAKE_C_FLAGS_DEBUG=-g -DCMAKE_CXX_FLAGS_RELEASE="-O3 -DNDEBUG" -DCMAKE_CXX_FLAGS_DEBUG=-g -DCMAKE_Fortran_FLAGS_RELEASE=-O3 -DCMAKE_Fortran_FLAGS_DEBUG=-g -DOC_SYSTEM_BLAS=ON -DOC_SYSTEM_BZIP2=OFF -DOC_SYSTEM_CELLML=OFF -DOC_SYSTEM_CLANG=OFF -DOC_SYSTEM_CSIM=OFF -DOC_SYSTEM_FIELDML-API=OFF -DOC_SYSTEM_FREETYPE=ON -DOC_SYSTEM_FTGL=OFF -DOC_SYSTEM_GDCM-ABI=OFF -DOC_SYSTEM_GLEW=OFF -DOC_SYSTEM_GTEST=OFF -DOC_SYSTEM_HDF5=OFF -DOC_SYSTEM_HYPRE=OFF -DOC_SYSTEM_IMAGEMAGICK=OFF -DOC_SYSTEM_IRON=OFF -DOC_SYSTEM_ITK=OFF -DOC_SYSTEM_JPEG=ON -DOC_SYSTEM_LAPACK=ON -DOC_SYSTEM_LIBCELLML=OFF -DOC_SYSTEM_LIBXML2=ON -DOC_SYSTEM_LLVM=OFF -DOC_SYSTEM_MUMPS=OFF -DOC_SYSTEM_NETGEN=OFF -DOC_SYSTEM_OPTPP=OFF -DOC_SYSTEM_PARMETIS=OFF -DOC_SYSTEM_PASTIX=OFF -DOC_SYSTEM_PETSC=OFF -DOC_SYSTEM_PLAPACK=OFF -DOC_SYSTEM_PNG=OFF -DOC_SYSTEM_PTSCOTCH=OFF -DOC_SYSTEM_SCALAPACK=OFF -DOC_SYSTEM_SCOTCH=OFF -DOC_SYSTEM_SLEPC=OFF -DOC_SYSTEM_SOWING=OFF -DOC_SYSTEM_SUITESPARSE=OFF -DOC_SYSTEM_SUNDIALS=OFF -DOC_SYSTEM_SUPERLU=OFF -DOC_SYSTEM_SUPERLU_DIST=OFF -DOC_SYSTEM_SZIP=OFF -DOC_SYSTEM_TIFF=OFF -DOC_SYSTEM_ZINC=OFF -DOC_SYSTEM_ZLIB=OFF -DCMAKE_INSTALL_RPATH="/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_darwin/clang-C6.0-gnu-F4.5/no_mpi/release/lib;/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_darwin/clang-C6.0-gnu-F4.5/openmpi_release/release/lib;/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_darwin/clang-C6.0-gnu-F4.5/mpi/openmpi/release/lib" -DCMAKE_INSTALL_RPATH_USE_LINK_PATH=TRUE -DCMAKE_INSTALL_PREFIX:STRING=/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_darwin/clang-C6.0-gnu-F4.5/openmpi_release/release -DBUILD_SHARED_LIBS=ON -DMPI=openmpi -DMPI_HOME=/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_darwin/clang-C6.0-gnu-F4.5/mpi/openmpi/release -DCMAKE_C_COMPILER=/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_darwin/clang-C6.0-gnu-F4.5/mpi/openmpi/release/bin/mpicc -DMPI_C_COMPILER=/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_darwin/clang-C6.0-gnu-F4.5/mpi/openmpi/release/bin/mpicc -DCMAKE_CXX_COMPILER=/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_darwin/clang-C6.0-gnu-F4.5/mpi/openmpi/release/bin/mpicxx -DMPI_CXX_COMPILER=/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_darwin/clang-C6.0-gnu-F4.5/mpi/openmpi/release/bin/mpicxx -DCMAKE_Fortran_COMPILER=/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_darwin/clang-C6.0-gnu-F4.5/mpi/openmpi/release/bin/mpifort -DMPI_Fortran_COMPILER=/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_darwin/clang-C6.0-gnu-F4.5/mpi/openmpi/release/bin/mpifort -DWITH_CELLML=ON -DCELLML_VERSION=1.0 -DLIBCELLML_VERSION=1.0 -DWITH_FIELDML=ON -DFIELDML-API_VERSION=0.5.0 -DWITH_HYPRE=ON -DHYPRE_VERSION=2.10.0 -DWITH_SUNDIALS=ON -DSUNDIALS_VERSION=2.5 -DWITH_MUMPS=ON -DMUMPS_VERSION=5.0.0 -DWITH_SCALAPACK=ON -DSCALAPACK_VERSION=2.8 -DWITH_PETSC=ON -DPETSC_VERSION=3.6.1 -DWITH_PROFILING=NO -DWITH_C_BINDINGS=ON -DWITH_Python_BINDINGS=ON -DINSTALL_TO_VIRTUALENV=/Users/mwu035/Jenkins/workspace/Multibranch_Opencmiss/JenkinsTest/oc/install/x86_64_darwin/clang-C6.0-gnu-F4.5/openmpi_release/release/virtual_environments -G"Unix Makefiles" ../src'
		}
		echo 'Configured'
	}
}

stage 'make'

parallel 'Slave1':{
	node('TestSlave1') {
		dir('./iron/build') {
			sh 'make'
			echo 'Built'		
		}
	}
}, 'Slave2':{
	node('TestSlave2') {
		echo 'HPC Disabled'
	}
}, 'Slave3':{
	node('TestSlave3') {
		dir('./iron/build') {
			sh 'make'
			echo 'Built'
			echo 'done'
			echo 'test'		
		}
	}
}

stage 'tests'

parallel 'Slave1':{
	node('TestSlave1') {
		echo 'Iron tests'
		dir('./iron/build') {
			sh 'make test'
		}
	}
}, 'Slave2':{
	node('TestSlave2') {
		echo 'HPC Disabled'
	}
}, 'Slave3':{
	node('TestSlave3') {
		echo 'Test Disabled'
	}
}

node('TestSlave1') {
	step([$class: 'GitHubCommitStatusSetter', statusResultSource: [$class: 'ConditionalStatusResultSource', results: [[$class: 'BetterThanOrEqualBuildResult', message: 'Build succeeded.', result: 'SUCCESS', state: 'SUCCESS']]]])
}

