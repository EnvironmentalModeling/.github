# Environmental Modeling Team

The Environmental Modeling Team is an interdisciplinary group of scientists and engineers led by the Environmental Laboratory, Engineer Research and Development Center, U.S. Army Corps of Engineers. Our primary focus is developing and applying advanced modeling tools and frameworks to simulate hydrological, ecological, and biogeochemical processes in aquatic systems. We support informed decision-making for water resource management, ecosystem restoration, and sustainable development through quantitative analysis and predictive modeling.

Aquatic ecosystems and the communities that depend on them face increasing threats from hydrological and climate extremes, development pressures, harmful algal blooms, and water quality degradation. Our modeling approaches integrate physical, chemical, and biological processes across multiple spatial and temporal scales to help achieve the dynamic balance needed to protect and restore these systems.

Our work is grounded in the principles of ecohydrology, an interdisciplinary science focused on understanding the interactions between hydrological and ecological processes. Ecohydrology seeks to improve the functioning, stability, and resiliency of degraded ecosystems and foster sustainable development through better understanding and management of water-ecosystem relationships.

Zalewski et al. (1997) proposed three foundational hypotheses that guide ecohydrological thinking:

1. **Hydrological processes generally regulate biota.** Water availability, flow regimes, thermal dynamics, and transport processes create the physical and chemical template that shapes ecological communities.

2. **Biota can be shaped as a tool to regulate hydrological processes.** Vegetation, wetlands, and biological communities influence infiltration, evapotranspiration, nutrient uptake, and water quality.

3. **Hydrological and biological regulations can be integrated with hydro-technical infrastructure to achieve sustainable water and ecosystem services.** Engineered systems can work in concert with natural processes to achieve management objectives.

These hypotheses are inherently quantitative, and numerical modeling provides the means to test, refine, and apply them across diverse systems and scales.

## Guiding Principles

The principles of ecohydrology are expressed through three sequential components that structure our modeling approach:

### Hydrological Framework

Quantification of the hydrological cycle provides the physical template for functional integration of hydrological and biological processes. This framework encompasses water movement, thermal dynamics, stratification patterns, and transport processes across relevant spatial and temporal scales. Understanding hierarchical interactions between biotic and abiotic factors begins with accurate representation of the hydrodynamic environment.

### Ecological and Water Quality Targets

Integrated processes at the river basin or reservoir scale can be steered to enhance carrying capacity and ecosystem services. Simulation of biogeochemical cycles and ecological processes enables prediction of water quality conditions and ecosystem responses, addressing nutrient dynamics, dissolved oxygen, algal growth (including harmful algal blooms), and other indicators of ecosystem resilience and resistance.

### Modeling and Analysis Methods

Regulation of hydrological and ecological processes, based on an integrative systems approach, provides tools for Integrated Water Resource Management. Numerical modeling integrates the hydrological framework with ecological and water quality targets to evaluate management alternatives, from reservoir operations and selective withdrawal strategies to nature-based solutions and Natural and Nature-Based Features (NNBF).

## Core Considerations

Our modeling approaches account for the key factors that govern ecohydrological dynamics:

- **Flow paths and transport**: Movement of water and constituents through watersheds and receiving waters, from headwaters to downstream systems
- **Residence time**: Relationships between inflow, outflow, and storage that determine the time available for biogeochemical transformations
- **Biogeochemical reactions**: Processes that transform nutrients, regulate dissolved oxygen, drive primary production, and influence water quality
- **System connectivity**: Interactions among hydrology, ecology, and biogeochemistry, as well as linkages between system components and management infrastructure

## Tools and Frameworks

Our modeling tools operationalize ecohydrological principles through numerical simulation:

### CE-QUAL-W2

CE-QUAL-W2 is a two-dimensional (longitudinal-vertical) hydrodynamic and water quality model developed and maintained by the U.S. Army Corps of Engineers, Engineer Research and Development Center (ERDC), Environmental Laboratory. It simulates flow and water quality dynamics in rivers, reservoirs, lakes, estuaries, and other thermally stratified water bodies. The model resolves vertical stratification and longitudinal gradients driven by flow, mixing, inflows, withdrawals, and biogeochemical reactions. CE-QUAL-W2 enables detailed analysis of temperature stratification, contaminant transport, and nutrient cycling, simulating key water quality constituents such as temperature, dissolved oxygen, nitrogen and phosphorus compounds, algae, and organic matter. Advanced features include support for fish habitat analysis, selective withdrawal operations, hypolimnetic aeration, sediment diagenesis, and the simulation of multiple algal groups—capabilities critical for understanding harmful algal bloom dynamics and ecosystem function. With over 1,100 documented applications worldwide by USACE and numerous federal, state, academic, and international organizations, CE-QUAL-W2 supports a wide range of use cases including environmental impact assessment, reservoir operations planning, infrastructure design, and adaptive water resource management. The model is widely used by U.S. federal agencies such as USACE, EPA, USBR, and USGS; state and local water quality agencies; utilities; universities; and international institutions. These users apply CE-QUAL-W2 to support regulatory compliance, resource management, water quality forecasting, and research in complex aquatic systems.

### ClearWater

ClearWater is an environmental modeling system whose primary purpose is the integration of water quality and ecohydrologic modeling with diverse hydraulic and hydrologic (H&H) models. ClearWater supports the simulation of biogeochemical and thermal processes and advection-diffusion calculations in riverine and reservoir systems as well as watershed runoff, leveraging existing H&H models for the hydrodynamic framework. ClearWater's modules simulate ecohydrological processes including heat balance (temperature), advanced biogeochemical kinetics, nutrient cycling, algal dynamics, dissolved oxygen, and contaminant fate and transport. Its transport engines compute advection and diffusion in complex riverine systems and stratified reservoirs.

### ClearWater-Riverine

ClearWater-Riverine provides two-dimensional water quality and ecohydrologic simulation capabilities that couple with the model grid and hydraulics outputs computed by the two-dimensional (2D) [River Analysis System (HEC-RAS)](https://www.hec.usace.army.mil/software/hec-ras/) developed by the USACE [Hydrologic Engineering Center (HEC)](https://www.hec.usace.army.mil). ClearWater-Riverine reads hydrodynamic outputs from H&H models and computes advection-diffusion transport along with biogeochemical kinetics for simulating nutrient cycling, algal dynamics, dissolved oxygen, and other water quality constituents in riverine systems. Work is in progress to integrate ClearWater-Riverine with ERDC's [Gridded Surface Subsurface Hydrologic Analysis (GSSHA)](https://en.wikipedia.org/wiki/GSSHA) model via the [Basic Model Interface (BMI)](https://csdms.colorado.edu/wiki/BMI).

### NADI

The [Network Analysis and Data Integration (NADI) System](https://github.com/Nadi-System) is a software framework designed to facilitate river data extraction, organization, analysis, and visualization with explicit representation of upstream and downstream relationships. NADI includes a Geographic Information System (GIS) tool that uses spatial methods to generate river networks and a Domain Specific Language (DSL) that provides a concise and intuitive syntax for network metadata analysis. The framework is extensible through a plugin system that enables user-defined functions to operate on individual nodes or entire networks, providing seamless integration with other software and programming languages. NADI can be used from the command line interface (CLI), graphical user interface (GUI) via the NADI Integrated Development Environment (IDE), or as a Rust or Python library, allowing users to develop custom plugins and applications.

NADI's capabilities have been demonstrated through large-scale analysis of river basins, identifying data gaps and characterizing the availability and quality of hydrologic records. For example, analysis of the Ohio River basin revealed that approximately half of USGS streamflow gages were constructed after upstream dams, with only 35% of gages remaining unaffected by upstream impoundments—and those unaffected gages account for just 1.2% of measured streamflow, illustrating the scarcity of natural streamflow data. Such analyses support both military and civil works needs by enabling systematic assessment of data availability, network connectivity, and infrastructure impacts across watersheds.

### Environmental Pool Management Screening Tools

Environmental Pool Management (EPM) is an operational strategy that adjusts the magnitude, timing, frequency, and duration of reservoir pool levels to achieve ecological outcomes such as improved wetland habitat, enhanced water quality, and increased habitat value for waterbirds, reptiles, and other wildlife. The EPM Screening Tools apply spatial and hydrologic screening criteria to identify USACE reservoirs with high potential for EPM implementation.

The spatial analysis component uses satellite imagery from Sentinel-2 and Landsat, processed via Google Earth Engine, in conjunction with the Global Surface Water Dataset (GSWD), National Land Cover Dataset (NLCD), and National Elevation Dataset (NED) to identify and characterize reservoir sediment deltas suitable for habitat management. Water occurrence, seasonality, and inter-annual variability metrics are computed to assess the ecological viability of delta areas. Soil characteristics from the USDA Soil Survey Geographic Database (SSURGO) support assessment of habitat suitability for target species.

The hydrologic analysis component retrieves pool stage records from the USACE Access to Water (A2W) system and computes growing-season metrics including stage range, variability, and frequency of fluctuations. A hydrologic management opportunity framework links combinations of water level characteristics to distinct ecological management opportunities, classifying reservoirs by their suitability for persistent wetland vegetation, seasonal shorebird habitat, waterfowl foraging areas, or other ecological targets.

The tools support prioritization of reservoirs for EPM across ecoregions and climate zones, enabling USACE Districts to identify opportunities for habitat improvement through modest operational adjustments.

## References

Zalewski, M., Janauer, G.A., and Jolánkai, G. (1997). Ecohydrology: A new paradigm for the sustainable use of aquatic resources. UNESCO IHP Technical Document in Hydrology No. 7.

## Contact

For questions about our tools, models, or collaborative opportunities, please contact the Environmental Modeling Team at the U.S. Army Corps of Engineers Engineer Research and Development Center, Environmental Laboratory.
