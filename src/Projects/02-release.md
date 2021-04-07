# Releases/Version System

In the MKProjects Rust Command Line Programs: 
- Phaktionz CLI
- Tomorrow Study's Packager  
- UniConv 

They will all follow the same **Release** and **Version** system, so how about we 
talk about each respectively. 

## Release System

In our release system, we will be following the edge -> beta -> stable channel format. 
Each of these programs will have the following branches to indicate the following channels: 

- main => stable channel
- beta => beta channel
- edge => edge channel

So now you may ask what the difference of these may be? Well they correspond to the different stages 
of the applications build process.  

### Edge:
- The everyday changes of the code that is always changing, and may be unstable 
- Once feature may be stable, it will be moved to the beta channel

### Beta: 
- The beta channel is used to organize all the new changes, and apply patches to find the best way to implement them
- The beta channel is pre-production and should be relatively stable during production 

### Stable: 
- The stable channel is the ready to use code
- All the code should be working properly and safely
- Depending on the new feature: 
  - The Major or Minor will be incremented and the patch will be reset to 0

## Version System 

The projects follow the same semantic version system other Rust projects use:

```
Version M.m.P
M - Major change (Like a new feature)
m - Minor change (New API)
P - Patches (Fixes on the code)
```