# TC Explorer - Tropical Cyclone Visualisation Tool
**Version 2.1.0**

*Developed by Team Sharks: May, Markey, Scott, Jackson, and Wheeler*

## Overview

TC Explorer is an interactive web application for visualizing and analyzing tropical cyclone data across different climate scenarios. The application provides comprehensive tools for researchers to explore cyclone tracks, genesis locations, intensity patterns, and scenario comparisons.

**Live Application:** https://tcexplorerdd.azurewebsites.net/

## Installation & Setup

### Requirements
- XAMPP (Apache web server)
- Modern web browser (Chrome, Firefox, Safari, or Edge)

### Local Installation
1. Install XAMPP from https://www.apachefriends.org/
2. Copy the TCExplorer folder to the `htdocs` directory in your XAMPP installation
3. Start Apache from the XAMPP control panel
4. Navigate to `http://localhost/TCExplorer/` in your web browser
5. If using the IBTrACS-devoid branch, no further action is required. If using main, configure PHP environment variables to expand memory limit to >1500MB and timeout to >= 300

**Note:** This application has been tested on Linux, Windows, and macOS platforms.

## Key Features

### Data Visualisation
- **Cyclone Tracks**: Interactive visualisation of tropical cyclone paths across the Australian region
- **Genesis Locations**: Display cyclone formation points (≥Category 1 strength)
- **Intensity Mapping**: Color-coded tracks showing cyclone intensity categories
- **Heatmap Analysis**: Density visualisation showing cyclone frequency patterns

### Scenario Analysis
- **Multiple Climate Scenarios**: Current, Natural (NAT), 2K warming, and 4K warming scenarios
- **Ensemble Selection**: Access to multiple ensemble members for statistical analysis
- **SST Model Support**: Sea Surface Temperature model variations for future scenarios
- **Comparison Mode**: Side-by-side analysis of different scenarios

### Interactive Controls
- **Year Range Filtering**: Flexible time period selection
- **Real-time Updates**: Dynamic visualisation updates based on control settings
- **Export Functionality**: Data export capabilities for further analysis
- **Mobile Support**: Responsive design for tablet and mobile devices

### User Experience
- **Interactive Tutorial**: Guided introduction to application features
- **Collapsible Interface**: Optimized layout for various screen resolutions
- **Professional Interface**: Clean, intuitive design for research environments 

## Data Sources

The application utilizes tropical cyclone data from the d4PDF (database for Policy Decision making for Future climate change) project, providing comprehensive climate model outputs for:

- **Historical Climate** (1951-2011): Current climate conditions
- **Natural Climate** (1951-2010): Climate conditions without anthropogenic warming
- **2K Warming Scenario** (2031-2090): Climate projections with 2°C global warming
- **4K Warming Scenario** (2051-2110): Climate projections with 4°C global warming

## Usage Guidelines

### Getting Started
1. Launch the application and complete the interactive tutorial for an overview of features
2. Select your desired climate scenario and ensemble member
3. Adjust year ranges to focus on specific time periods
4. Toggle visualisation options to explore different aspects of the data

### Best Practices
- Use comparison mode to analyze differences between climate scenarios
- Export data for detailed statistical analysis outside the application
- Utilize the collapsible interface on smaller screens for optimal viewing

## Technical Specifications

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Mapping**: Leaflet.js with OpenStreetMap tiles
- **Data Format**: JSON-based cyclone track data
- **Browser Support**: Modern browsers with JavaScript enabled
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices

## Support & Documentation

For technical documentation and development information, please refer to:
- `AZURE_DEPLOYMENT.md`
- Accompanying documentation files

## Version History

**v2.1.0**
- Optimised IBTrACS data loading, by compressing and extracting between back and front end. This reduces load times by ~15-30seconds.

**v2.0.0**
- Finalised files for streamlined GitHub-Azure deployment. 

**v1.2.0**
- Colourblind support added
- Satellite view added
- Refined tutorial
- (also un~~fucked~~ my attempt at database integration. she aint ready yet)


**v1.0.0a** - Alpha-testing of Production Release
- Collapsible desktop interface
- Enhanced mobile responsiveness
- Production-ready codebase

**Previous Versions**
- v0.10.0 Added experimental heatmap view, which utilises pre-processed cell data to draw the heatmap. This was created from Client's IPYNB code modified to pre-process data, and then uploaded into application through density_data/
See known issues with this experimental implementation.
- v0.11.0 Modularised JS for extendability, added support for mobile devices.
- v0.12.0 Added cool shark favicon. Arguably not deserving of a full number bump, but it *is* a really cool shark.
- v0.13.0 Added support for the long-awaited 'HPB_NAT' scenario. This is historical data with natural warming still included. Also re-styled control group to allow for extra buttons to be added without display nastiness.
- v0.14.0 Added scenario comparison functionality. Now different scenarios can be compared in terms of tracks and genesis locations. Also removed old heatmap visualisation, and removed the "Filter to Aus" toggle as I have deemed it no longer necessary lol
- v0.14.5 Genesis locations modified to first occurence >= Cat 1 (previously just first data point). This can be toggled with the relevant button. Loading text also fixed to correctly display loaded cache data. Assorted styling improved.
- v0.15.0 Added collapsible control panel to desktop mode as well. This allows app to facilitate lower resolution displays much more effectively.
- v0.15.5 Mobile version of site updated for functionality. Now functions horizontally and vertically, with a hamburger options menu allowing elements to be disabled for visibility and functions to be selected. Additional testing required to ensure full functionality.
- v0.16.0 Added individual year sliders and visibility toggles to scenario comparison. Investigating a potential issue with mobile display (full header showing in horizontal view).
- v0.17.0 Add full user tutorial for both desktop and mobile. Tutorial is configured to launch automatically for first-time users, and also be toggleable with a header option. 

## About Team Sharks

This application was developed by Team Sharks, comprising May, Markey, Scott, Jackson, and Wheeler, as an educational and research tool for tropical cyclone analysis in the Australian region.

---

*TC Explorer v2.1.0 - Ready for deployment and educational use*







                    #########
                    ##XXXX#XX####                    #########
                    ###############          #####################
                      ###XXXXXXXXX### ########XXXXXXXXXXXXXXXXXX##
                        #X#XXXXXXX#X#####XX#XXXXXXX XXXXXXX XX###
                         #XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX###
                         ##XXXXXXXXX##XXXXXXXXXXXXXXXXXXXXXXXXX##
                          #XXXXXXXX##XXXXXXXXXXXXXXXXXXXXXXXXX###
                          ##XXXX###XXXXXXXXXXXXXXXXXXXXXXXX#####
                        ####XXX##XXXXXXXXXXXXXXXXXXXXXXX#######
                       ##X##XX#XXXXXXXXXXXXXXXXXXXXXXXX#######
                  #####XXX#XXXXXXXXXXXXXXXXXXXXXXXX##########
         ##########X##XXXXXXXXXXXXXXXXXXXXXXXXXXX###XXX#####
      #######XXXXXXXXX##XXXXXXXXXXXXXXXXXXXXXXXXXX###XXX#######
      ####XXXXXXXXXXXXXX##XXXXXXXXXXXXXXXXXXXXXXXXX###XXXX##XXXXX#####
      ##XX###############XXXXXXXXXXXXXXXXXXXXXXX###XXXXXX##XXXXXXXXXX#####
      #######XXXXXXXXXXXXXXXXXXXXX###XXXXXXX##XXXXXXXXXXXXXXX###
                ##XXXXXXXXXXXXXXXXXXXX###XXXXXXXX##XXXXXXXXXXXXXXXXXXX###
               ##XXXXXXXXXXXXXXXXXXX###XXXXXXXX#######XXXXXXXXXXXXXXXXXX###
              ##XXXXXXXXXXXXXXXX#####XXXXXXXX###     ############XXXXXXXXX###
             ##XXXXXXXXXXXXX#####XXXXXXXXX###                   ######XXXXXX#
             #XXXXXXXXXXX####XXXXXXXXXX####                          ######X#
            ##XXXXXXXXX###XXXXXXXXXX####                                  ###
           ##XXXXXXXXX##XXXXXXXX#####
           #XXXX#XXXX##XXXXXX####                #####
          ##XXXXXXXX##XXXXX#####              ####XXX#
          #XXXXXXXXX#XXXX###XX#             ###XXXX##
          #XXXXXXXX##XX###XXXX#          ####XXXXXX#
          #XXXXXXXX#X######XXX#        ###XXXXXXXX##
          #XXXXXXXX#X#    #####      ###XXXXXXXXXX#
          #XXXXXXX###        ##    ###XXXXXXXXXXX##
          #XXXXXXX#X#            ###XXXXXXXXX#####
          #XXXXXXX###          ###XXXXXXX#####
          ##XXXXX#X##        ###XXXXXXX###
           #XXXXX####   #####XXXXXXXX##
           ##XXXXXX######XXXXXXXXXX###
           ###XXXXXXXXXXXXXXXXXXX###
           #X##XXXXXXXXXXXXXXXXX##
          ##X####XXXXXXXXXXXXXX##
          ####  ###XXXXXXXXXXX##
          ##      ###XXXXXXXX##
                    #XXXXXXXX#
                     #XXXXXX##
                     #XXXXXX#
                     ##XXXXX#
                      #XXXXX#
                      #XXXXX#
                       #XXXX#
                       ##XXX#
                        #XXXX#
                        ##XXX#
                         ##XX##
                          ##XX##
                           ##XX#
                            ##XX##
                             ##XX##
                              ###X##
                                #####
                                  #####
                                    ###
