<h1>Microsoft Azure Disired State Configuration (DSC)</h1>

# Course Overview

- Create a DSC configuration Script
- How to find and use DSC resources
- Configure managed servers to use DSC
- Deploy your configurations

# Introduction to Desired State Configuration

# DSC Fundamentals

# Creating a DSC Configuration

# Deploying a DSC Configuration

# Advanced Configurations

# Creating Custom Resources

# Troubleshooting DSC

# Using a Pull Server

# Advanced DSC Techniques





---










$PSVerstionTable

Commands:
set-azurerm-vmdscextention
Find-DSCResource -name smbShare
Find-Module computermanagementdsc | Tee-Object -variable m
$m | Format-Table author,publisheddate,projecturi,description -wrap


-----

Configuration Sample {
   Import-DscResource -ModuleName PSDesiredStateConfiguration -ModuleVersion 1.1
      #this is using a built-in DSC Resource
      File Demo {
         Destination = "C:\DSCDemo"
         Ensure      = "Present"
         Type        = "Directory"
      }
   }
}

