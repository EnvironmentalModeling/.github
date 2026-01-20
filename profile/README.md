# Environmental Modeling Team

The Environmental Modeling Team is an interdisciplinary group of scientists and engineers led by the [Environmental Laboratory](https://www.erdc.usace.army.mil/Locations/EL/), [Engineer Research and Development Center (ERDC)](https://www.erdc.usace.army.mil), [U.S. Army Corps of Engineers (USACE)](https://www.usace.army.mil). Our primary focus is developing and applying advanced modeling tools and frameworks to simulate hydrological, ecological, and biogeochemical processes in aquatic systems. We support informed decision-making for water resource management, ecosystem restoration, and sustainable development through quantitative analysis and predictive modeling.

Aquatic ecosystems and the communities that depend on them face increasing threats from hydrological and climate extremes, development pressures, harmful algal blooms, and water quality degradation. Our modeling approaches integrate physical, chemical, and biological processes across multiple spatial and temporal scales to help achieve the dynamic balance needed to protect and restore these systems.

Environmental modeling encompasses process-based numerical simulation as well as data-driven statistical and machine learning (ML) approaches, hybrid methods such as physics-informed ML, and analysis tools for uncertainty quantification and sensitivity analysis. Our work develops and applies these computational methods, tools, and frameworks to support water resource management and environmental research.

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

ClearWater (Corps Library for Environmental Analysis and Restoration of Watersheds) is an environmental modeling system whose primary purpose is the integration of water quality and ecohydrologic modeling with diverse hydraulic and hydrologic (H&H) models. ClearWater supports the simulation of biogeochemical and thermal processes and advection-diffusion calculations in riverine and reservoir systems as well as watershed runoff, leveraging existing H&H models for the hydrodynamic framework. ClearWater's modules simulate ecohydrological processes including heat balance (temperature), advanced biogeochemical kinetics, nutrient cycling, algal dynamics, dissolved oxygen, vegetation dynamics, and contaminant fate and transport. Its transport engines compute advection and diffusion in complex riverine systems and stratified reservoirs.

The ClearWater system comprises the following process simulation modules:

- **TSM (Temperature Simulation Module)**: Simulates heat balance processes including solar radiation, atmospheric exchange, and thermal stratification dynamics.
- **NSM (Nutrient Simulation Modules)**: NSM-I simulates fundamental eutrophication processes including interactions among temperature, nutrients, algae, dissolved oxygen, and organic matter. NSM-II extends these capabilities with a two-layer sediment diagenesis model, labile and refractory organic matter pools, multiple algal groups including nitrogen-fixing cyanobacteria, silica cycling, and anaerobic processes (methane and sulfide dynamics).
- **GSM (General Constituent Simulation Module)**: Simulates user-defined conservative and non-conservative constituents with customizable decay and transformation rates.
- **CSM (Contaminant Simulation Module)**: Simulates fate and transport of organic chemicals, pesticides, and metals, including multi-phase partitioning (dissolved, DOC-sorbed, algae-sorbed, POM-sorbed, solid-sorbed), decay and biodegradation, hydrolysis, photolysis, volatilization, and bed sediment interactions.
- **MSM (Mercury Simulation Module)**: Simulates mercury speciation (elemental Hg0, inorganic HgII, and methylmercury MeHg), methylation and demethylation, photoreduction, volatilization, partitioning, and bioaccumulation processes in aquatic systems with optional sediment diagenesis.
- **ESM (Ecohydrology Simulation Module)**: A process-based 2D ecohydrology model that simulates vegetation dynamics in river corridors, floodplains, and aquatic ecosystems, including recruitment, growth, mortality (scour, burial, drowning, drying, ice, competition), and feedbacks between vegetation structure and hydraulic roughness. ESM supports six vegetation categories: trees, shrubs, grasses, emergent aquatic, submerged aquatic, and floating vegetation. ESM is currently loosely coupled with HEC-RAS 2D: hydraulics and sediment outputs from completed HEC-RAS simulations serve as inputs to ESM, which computes updated Manning's n roughness values based on evolving vegetation structure. However, these roughness values are not currently fed back into HEC-RAS during simulation. Within ClearWater-Riverine, ESM is tightly coupled with NSM (nutrients) and TSM (temperature), enabling bidirectional exchange of nutrient uptake, thermal effects, and vegetation state at each computational timestep.

ClearWater modules are written in modern Python and designed to flexibly couple with a variety of H&H models including HEC-RAS 2D, GSSHA, CE-QUAL-W2, and [AdH](https://www.erdc.usace.army.mil/Locations/CHL/AdH/) via the [Basic Model Interface (BMI)](https://csdms.colorado.edu/wiki/BMI). The Python implementation modernizes algorithms originally developed in Fortran 95 and documented in ERDC technical reports by Zhang and Johnson (2016).

### ClearWater-Riverine

ClearWater-Riverine provides two-dimensional water quality and ecohydrologic simulation capabilities that couple with the model grid and hydraulics outputs computed by the two-dimensional (2D) [River Analysis System (HEC-RAS)](https://www.hec.usace.army.mil/software/hec-ras/) developed by the USACE [Hydrologic Engineering Center (HEC)](https://www.hec.usace.army.mil). ClearWater-Riverine is a 2D water quality transport model that calculates conservative advection and diffusion of constituents from an unstructured grid of flows within complex river systems and floodplains. It reads hydrodynamic outputs from H&H models and computes advection-diffusion transport along with biogeochemical kinetics by coupling to the ClearWater process simulation modules.

ClearWater-Riverine assumes vertical homogeneity and is best suited for evaluating riverine systems during conditions where vertical stratification does not contribute significantly to water quality dynamics, but where longitudinal and lateral changes are important. At present, TSM and NSM have been successfully coupled to HEC-RAS 2D models via ClearWater-Riverine, enabling simulation of fundamental eutrophication processes such as the interactions among temperature, nutrients, algae, dissolved oxygen, and organic matter.

Work is in progress to integrate ClearWater-Riverine with ERDC's [Gridded Surface Subsurface Hydrologic Analysis (GSSHA)](https://www.erdc.usace.army.mil/Locations/CHL/GSSHA/) model via the [Basic Model Interface (BMI)](https://csdms.colorado.edu/wiki/BMI), extending its applicability to watershed-scale simulations.

### ClearWater-Data

ClearWater-Data provides flexible and performant data access and storage protocols for the ClearWater system. It combines the capabilities of [xarray](https://xarray.dev) with flexible access patterns to facilitate data exchange among ClearWater components and with external H&H models.

### NADI

The [Network Analysis and Data Integration (NADI) System](https://github.com/Nadi-System) is a software framework designed to facilitate river data extraction, organization, analysis, and visualization with explicit representation of upstream and downstream relationships. NADI includes a Geographic Information System (GIS) tool that uses spatial methods to generate river networks and a Domain Specific Language (DSL) that provides a concise and intuitive syntax for network metadata analysis. The framework is extensible through a plugin system that enables user-defined functions to operate on individual nodes or entire networks, providing seamless integration with other software and programming languages. NADI can be used from the command line interface (CLI), graphical user interface (GUI) via the NADI Integrated Development Environment (IDE), or as a Rust or Python library, allowing users to develop custom plugins and applications.

NADI's capabilities have been demonstrated through large-scale analysis of river basins, identifying data gaps and characterizing the availability and quality of hydrologic records. For example, analysis of the Ohio River basin revealed that approximately half of USGS streamflow gages were constructed after upstream dams, with only 35% of gages remaining unaffected by upstream impoundments—and those unaffected gages account for just 1.2% of measured streamflow, illustrating the scarcity of natural streamflow data. Such analyses support both military and civil works needs by enabling systematic assessment of data availability, network connectivity, and infrastructure impacts across watersheds.

### Environmental Pool Management Screening Tools

[Environmental Pool Management (EPM)](https://www.mvs-wc.usace.army.mil/epm/epmindex.html) is an operational strategy that adjusts the magnitude, timing, frequency, and duration of reservoir pool levels to achieve ecological outcomes such as improved wetland habitat, enhanced water quality, and increased habitat value for waterbirds, reptiles, and other wildlife. The EPM Screening Tools apply spatial and hydrologic screening criteria to identify USACE reservoirs with high potential for EPM implementation.

The spatial analysis component uses satellite imagery from Sentinel-2 and Landsat, processed via [Google Earth Engine](https://earthengine.google.com), in conjunction with the [Global Surface Water Dataset (GSWD)](https://global-surface-water.appspot.com), [National Land Cover Dataset (NLCD)](https://www.usgs.gov/centers/eros/science/national-land-cover-database), and [National Elevation Dataset (NED)](https://www.usgs.gov/publications/national-elevation-dataset) to identify and characterize reservoir sediment deltas suitable for habitat management. Water occurrence, seasonality, and inter-annual variability metrics are computed to assess the ecological viability of delta areas. Soil characteristics from the [U.S. Department of Agriculture (USDA)](https://www.usda.gov) [Soil Survey Geographic Database (SSURGO)](https://www.nrcs.usda.gov/resources/data-and-reports/soil-survey-geographic-database-ssurgo) support assessment of habitat suitability for target species.

The hydrologic analysis component retrieves pool stage records from the USACE Access to Water (A2W) system and computes growing-season metrics including stage range, variability, and frequency of fluctuations. A hydrologic management opportunity framework links combinations of water level characteristics to distinct ecological management opportunities, classifying reservoirs by their suitability for persistent wetland vegetation, seasonal shorebird habitat, waterfowl foraging areas, or other ecological targets.

The tools support prioritization of reservoirs for EPM across ecoregions and climate zones, enabling USACE Districts to identify opportunities for habitat improvement through modest operational adjustments.

## References

Baird, A.J. and Wilby, R.L. (Eds.). (1999). Eco-Hydrology: Plants and Water in Terrestrial and Aquatic Environments. Routledge, New York.

Bowie, G.L., Mills, W.B., Porcella, D.B., Campbell, C.L., Pagenkopf, J.R., Rupp, G.L., Johnson, K.M., Chan, P.W.H., Gherini, S.A., and Chamberlin, C.E. (1985). Rates, Constants, and Kinetics Formulations in Surface Water Quality Modeling (2nd ed.). EPA/600/3-85/040. U.S. Environmental Protection Agency, Athens, GA.

Brewer, S.K., Worthington, T.A., Mollenhauer, R., Stewart, D.R., McManamay, R.A., Guertault, L., and Moore, D. (2018). Synthesizing Models Useful for Ecohydrology and Ecohydraulic Approaches: An Emphasis on Integrating Models to Address Complex Research Questions. Ecohydrology, 11(7). https://doi.org/10.1002/eco.1966

Chapra, S.C. (1997). Surface Water-Quality Modeling. McGraw-Hill, New York.

Chapra, S.C. (2008). Surface Water-Quality Modeling. Waveland Press, Long Grove, IL.

Di Toro, D.M. (2001). Sediment Flux Modeling. Wiley-Interscience, New York.

Eagleson, P.S. (1978a). Climate, Soil, and Vegetation: 1. Introduction to Water Balance Dynamics. Water Resources Research, 14(5), 705–712. https://doi.org/10.1029/WR014i005p00705

Eagleson, P.S. (1978b). Climate, Soil, and Vegetation: 2. The Distribution of Annual Precipitation Derived from Observed Storm Sequences. Water Resources Research, 14(5), 713–721. https://doi.org/10.1029/WR014i005p00713

Eagleson, P.S. (1978c). Climate, Soil, and Vegetation: 3. A Simplified Model of Soil Moisture Movement in the Liquid Phase. Water Resources Research, 14(5), 722–730. https://doi.org/10.1029/WR014i005p00722

Eagleson, P.S. (1978d). Climate, Soil, and Vegetation: 4. The Expected Value of Annual Evapotranspiration. Water Resources Research, 14(5), 731–739. https://doi.org/10.1029/WR014i005p00731

Eagleson, P.S. (1978e). Climate, Soil, and Vegetation: 5. A Derived Distribution of Storm Surface Runoff. Water Resources Research, 14(5), 741–748. https://doi.org/10.1029/WR014i005p00741

Eagleson, P.S. (1978f). Climate, Soil, and Vegetation: 6. Dynamics of the Annual Water Balance. Water Resources Research, 14(5), 749–764. https://doi.org/10.1029/WR014i005p00749

Eagleson, P.S. (1978g). Climate, Soil, and Vegetation: 7. A Derived Distribution of Annual Water Yield. Water Resources Research, 14(5), 765–776. https://doi.org/10.1029/WR014i005p00765

Eagleson, P.S. (1982). Ecological Optimality in Water-Limited Natural Soil-Vegetation Systems: 1. Theory and Hypothesis. Water Resources Research, 18(2), 325–340. https://doi.org/10.1029/WR018i002p00325

Fu, B., Horsburgh, J.S., Jakeman, A.J., Gualtieri, C., Arnold, T., Marshall, L., Green, T.R., Quinn, N.W.T., Volk, M., Hunt, R.J., Vezzaro, L., Croke, B.F.W., Jakeman, J.D., Snow, V., and Rashleigh, B. (2020). Modeling Water Quality in Watersheds: From Here to the Next Generation. Water Resources Research, 56(11). https://doi.org/10.1029/2020WR027721

Hatton, T.J., Salvucci, G.D., and Wu, H.I. (1997). Eagleson's Optimality Theory of an Ecohydrological Equilibrium: Quo Vadis? Functional Ecology, 11(6), 665–674. https://doi.org/10.1046/j.1365-2435.1997.00159.x

Hunt, R.J. and Wilcox, D.A. (2003). Ecohydrology—Why Hydrologists Should Care. Ground Water, 41(3), 289–289. https://doi.org/10.1111/j.1745-6584.2003.tb02592.x

Janauer, G.A. (2000). Ecohydrology: Fusing Concepts and Scales. Ecological Engineering, 16(1), 9–16. https://doi.org/10.1016/S0925-8574(00)00072-0

Ji, Z.-G. (2008). Hydrodynamics and Water Quality: Modeling Rivers, Lakes, and Estuaries. Wiley-Interscience, Hoboken, NJ.

Johnson, B.E. and Zhang, Z. (2016). Testing and Validation Studies of the NSMII-Benthic Sediment Diagenesis Module. ERDC/EL TR-16-11. U.S. Army Engineer Research and Development Center, Vicksburg, MS. https://hdl.handle.net/11681/20343

Krysanova, V. and Arnold, J.G. (2008). Advances in Ecohydrological Modelling with SWAT—A Review. Hydrological Sciences Journal, 53(5), 939–947. https://doi.org/10.1623/hysj.53.5.939

Kui, L., Stella, J.C., Lightbody, A., and Wilcox, A.C. (2014). Ecogeomorphic Feedbacks and Flood Loss of Riparian Tree Seedlings in Meandering Channel Experiments. Water Resources Research, 50(12), 9366–9384. https://doi.org/10.1002/2014WR015719

Rodríguez-Iturbe, I. (2000). Ecohydrology: A Hydrologic Perspective of Climate-Soil-Vegetation Dynamics. Water Resources Research, 36(1), 3–9. https://doi.org/10.1029/1999WR900210

Sullivan, C.J., Vokoun, J.C., Helton, A.M., Briggs, M.A., and Kurylyk, B.L. (2021). An Ecohydrological Typology for Thermal Refuges in Streams and Rivers. Ecohydrology, 14(5). https://doi.org/10.1002/eco.2295

Sun, G., Hallema, D., and Asbjornsen, H. (2017). Ecohydrological Processes and Ecosystem Services in the Anthropocene: A Review. Ecological Processes, 6(1), 35. https://doi.org/10.1186/s13717-017-0104-6

Thomann, R.V. and Mueller, J.A. (1987). Principles of Surface Water Quality Modeling and Control. Harper & Row, New York.

Vannote, R.L., Minshall, G.W., Cummins, K.W., Sedell, J.R., and Cushing, C.E. (1980). The River Continuum Concept. Canadian Journal of Fisheries and Aquatic Sciences, 37(1), 130–137. https://doi.org/10.1139/f80-017

Yin, X.A., Petts, G.E., and Yang, Z.F. (2015). Ecofriendly River Management under Ever-Increasing Environmental Pressures. River Research and Applications, 31(4), 403–405. https://doi.org/10.1002/rra.2902

Zalewski, M., Janauer, G.A., and Jolánkai, G. (1997). Ecohydrology: A New Paradigm for the Sustainable Use of Aquatic Resources. UNESCO IHP Technical Document in Hydrology No. 7.

Zhang, Z. and Johnson, B.E. (2016). Aquatic Contaminant and Mercury Simulation Modules Developed for Hydrologic and Hydraulic Models. ERDC/EL TR-16-8. U.S. Army Engineer Research and Development Center, Vicksburg, MS. https://hdl.handle.net/11681/20249

Zhang, Z. and Johnson, B.E. (2016). Aquatic Nutrient Simulation Modules (NSMs) Developed for Hydrologic and Hydraulic Models. ERDC/EL TR-16-1. U.S. Army Engineer Research and Development Center, Vicksburg, MS. https://hdl.handle.net/11681/10112

## Contact

For questions about our tools, models, or collaborative opportunities, please contact the Environmental Modeling Team at the U.S. Army Corps of Engineers Engineer Research and Development Center, Environmental Laboratory.
