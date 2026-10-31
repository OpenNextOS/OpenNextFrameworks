This project aims to completely reïmplement Rhapsody OS components. These components are intended to have a build mode that creates binary compatible (ABI stable) Frameworks and Services. 

# Build Modes
-DDistributionRhapsodyOS (intended for Rhapsody OS, and Mac OS X Server 1.0-1.2v3)
-DDistributionOpenNext aliased -DDistributionRhapsodiOS [Information Here] (https://github.com/RhapsodiOS/RhapsodiOS)

## Usage
Within the source code you will find 
#if defined(DistributionRhapsodyOS) 
…
#endif

#if defined(DistributionOpenNext) || defined(DistributionRhapsodiOS)
…
#endif

These gates are primarily used decide where and how features are implemented so on RhaspdyOS they will not be ABI breaking. On OpenNext or RhapsodiOS, they can break ABI as they are new distributions. 

# Frameworks
- AppKit (near complete) [Information](https://github.com/austintatiousness/OpenNextFrameworks/wiki/AppKit.framework)
- Foundation (in progress)

# Private Frameworks

# CoreServices
- WindowServer (in prgoress) [Information](https://github.com/austintatiousness/OpenNextFrameworks/wiki/WindowServer)
