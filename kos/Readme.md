# KOS (Kind of Service) Implementation

This folder contains the **implementation files of controlled vocabulary or KOS**, representing the formal and machine-readable definition of needed vocabularies.

## Purpose

The goal of this directory is to store the **vocabulary or KOS files**, which describe the concepts and relations among them.

## Contents

This implementation includes two SKOS vocabularies for urban environmental monitoring:

- [`sensor-variables.ttl`](sensor-variables.ttl) - The sensor variables thesaurus
- [`feature-of-interest.ttl`](feature-of-interest.ttl) - The features of interest vocabulary

## SKOS Vocabularies Design

This KOS implementation defines two interconnected SKOS concept schemes that work together to describe sensor observations in urban environments.

### 1. SensorVariables (kos/sensor-variables.ttl)

A concept scheme that groups properties and magnitudes measured by sensors in urban environments. It follows a hierarchical structure with top-level categories and nested subcategories.

**Top-level categories:**
- MeteorologicalVariables
- AirQualityVariables
- AcousticVariables
- WaterQualityVariables
- SoilVariables
- TrafficVariables
- EnergyVariables
- WasteVariables
- SensorStatusVariables

**Hierarchical tree structure:**
```
SensorVariables
├── MeteorologicalVariables
│   ├── TemperatureVariables
│   │   ├── AirTemperature
│   │   ├── RoadTemperature
│   │   ├── DewPointTemperature
│   │   ├── WetBulbTemperature
│   │   ├── HeatIndex
│   │   └── WindChill
│   ├── HumidityVariables
│   │   ├── RelativeHumidity
│   │   └── AbsoluteHumidity
│   ├── PressureVariables
│   │   ├── AtmosphericPressure
│   │   └── SeaLevelPressure
│   ├── WindVariables
│   │   ├── WindSpeed
│   │   ├── MaximumWindSpeed
│   │   ├── WindDirection
│   │   └── WindGustDirection
│   ├── PrecipitationVariables
│   │   ├── PrecipitationAmount
│   │   ├── PrecipitationIntensity
│   │   ├── SnowDepth
│   │   └── SnowWaterEquivalent
│   ├── RadiationVariables
│   │   ├── SolarIrradiance
│   │   ├── UVIndex
│   │   ├── PhotosyntheticallyActiveRadiation
│   │   └── NetRadiation
│   ├── LightVariables
│   │   ├── Illuminance
│   │   └── SunshineDuration
│   └── VisibilityVariables
│       ├── Visibility
│       └── CloudBaseHeight
├── AirQualityVariables
│   ├── GaseousPollutants
│   │   ├── NO2Concentration
│   │   ├── NOConcentration
│   │   ├── NOxConcentration
│   │   ├── O3Concentration
│   │   ├── SO2Concentration
│   │   ├── COConcentration
│   │   ├── NH3Concentration
│   │   └── H2SConcentration
│   ├── GreenhouseGases
│   │   ├── CO2Concentration
│   │   ├── CH4Concentration
│   │   └── N2OConcentration
│   ├── VolatileOrganicCompounds
│   │   ├── BenzeneConcentration
│   │   ├── TolueneConcentration
│   │   ├── XyleneConcentration
│   │   ├── FormaldehydeConcentration
│   │   └── TotalVOCConcentration
│   ├── ParticulateMatterVariables
│   │   ├── PM1Concentration
│   │   ├── PM25Concentration
│   │   ├── PM10Concentration
│   │   ├── TotalSuspendedParticles
│   │   └── ParticleNumberConcentration
│   ├── HeavyMetalVariables
│   │   ├── ArsenicConcentration
│   │   ├── NickelConcentration
│   │   ├── CadmiumConcentration
│   │   ├── LeadConcentration
│   │   ├── MercuryConcentration
│   │   └── BenzoAPyreneConcentration
│   ├── PollenVariables
│   │   ├── PollenConcentration
│   │   └── SporeConcentration
│   └── OdorVariables
│       ├── OdorIntensity
│       └── OdorConcentration
├── AcousticVariables
│   ├── EquivalentSoundPressureLevel
│   ├── StatisticalNoiseLevels
│   │   ├── L10
│   │   ├── L50
│   │   ├── L90
│   │   ├── Lmax
│   │   └── Lmin
│   └── TemporalNoiseLevels
│       ├── DayTimeNoiseLevel
│       ├── EveningNoiseLevel
│       ├── NightTimeNoiseLevel
│       └── DayEveningNightNoiseLevel
├── WaterQualityVariables
│   ├── WaterPhysicochemicalVariables
│   │   ├── WaterTemperature
│   │   ├── WaterPH
│   │   ├── WaterElectricalConductivity
│   │   ├── WaterTurbidity
│   │   ├── TotalDissolvedSolids
│   │   ├── ResidualFreeChlorine
│   │   ├── DissolvedOxygen
│   │   ├── OxygenSaturation
│   │   └── WaterRedoxPotential
│   ├── WaterHydraulicVariables
│   │   ├── WaterLevel
│   │   ├── WaterFlowRate
│   │   ├── WaterVelocity
│   │   └── WaterPressure
│   ├── WaterNutrientVariables
│   │   ├── NitrateConcentration
│   │   ├── NitriteConcentration
│   │   ├── PhosphateConcentration
│   │   └── AmmoniumConcentration
│   └── WaterBiologicalVariables
│       ├── ChlorophyllAConcentration
│       └── BlueGreenAlgaeConcentration
├── SoilVariables
│   ├── SoilTemperature
│   ├── SoilMoistureTension
│   ├── SoilMoistureContent
│   ├── SoilPH
│   ├── SoilElectricalConductivity
│   └── SoilSalinity
├── TrafficVariables
│   ├── TrafficFlowVariables
│   │   ├── VehicleCount
│   │   └── TrafficFlow
│   ├── TrafficSpeedVariables
│   │   ├── AverageTrafficSpeed
│   │   └── MaximumTrafficSpeed
│   └── TrafficOccupancyVariables
│       ├── LaneOccupancy
│       └── ParkingOccupancy
├── EnergyVariables
│   ├── ElectricityVariables
│   │   ├── ActivePower
│   │   ├── ReactivePower
│   │   ├── ActiveEnergy
│   │   ├── Voltage
│   │   ├── ElectricCurrent
│   │   └── PowerFactor
│   └── GasVariables
│       ├── GasFlowRate
│       ├── GasPressure
│       └── GasConsumption
├── WasteVariables
│   ├── ContainerFillLevel
│   ├── ContainerTemperature
│   └── ContainerWeight
└── SensorStatusVariables
    ├── BatteryLevel
    ├── BatteryVoltage
    ├── InternalSensorTemperature
    ├── SignalStrength
    └── SensorUptime
```

### 2. FeaturesOfInterest (kos/feature-of-interest.ttl)

A concept scheme that groups features of interest observable by sensors according to SOSA ontology. Each feature has direct links to observable properties via `sosa:hasProperty` relationships.

**Hierarchical tree structure with property links:**
```
FeaturesOfInterest
├── Air
│   └── hasProperty → AirTemperature, RelativeHumidity, AtmosphericPressure,
│                     NO2Concentration, NOConcentration, NOxConcentration,
│                     O3Concentration, SO2Concentration, COConcentration,
│                     NH3Concentration, BenzeneConcentration, TolueneConcentration,
│                     XyleneConcentration
├── ParticulateMatter
│   └── hasProperty → PM1Concentration, PM25Concentration, PM10Concentration,
│                     ArsenicConcentration, NickelConcentration, CadmiumConcentration,
│                     LeadConcentration, BenzoAPyreneConcentration
├── Soil
│   └── hasProperty → SoilTemperature, SoilMoistureTension
├── RoadSurface
│   └── hasProperty → RoadTemperature
├── Wind
│   └── hasProperty → WindSpeed, MaximumWindSpeed, WindDirection
├── Precipitation
│   └── hasProperty → PrecipitationAmount
├── SolarRadiation
│   └── hasProperty → SolarIrradiance, UVIndex, PhotosyntheticallyActiveRadiation
├── AmbientLight
│   └── hasProperty → Illuminance
├── AirbornePollen
│   └── hasProperty → PollenConcentration
├── AcousticEnvironment
│   └── hasProperty → EquivalentSoundPressureLevel, DayTimeNoiseLevel,
│                     NightTimeNoiseLevel, DayEveningNightNoiseLevel
├── DrinkingWater
│   └── hasProperty → ResidualFreeChlorine, WaterTurbidity, WaterPH,
│                     WaterElectricalConductivity, DissolvedOxygen, WaterTemperature
└── IoTSensor
    └── hasProperty → BatteryLevel, BatteryVoltage, InternalSensorTemperature
```

## Design Principles

### Integration with SOSA Ontology
- Concepts in **SensorVariables** are typed as `sosa:ObservableProperty` and `qudt:QuantityKind`
- Concepts in **FeaturesOfInterest** are typed as `sosa:FeatureOfInterest`
- Features link to properties using `sosa:hasProperty` relationships

### Integration with QUDT
- Standardized units defined via `qudt:applicableUnit` for each observable property
- Uses QUDT unit vocabulary (e.g., `unit:DEG_C`, `unit:PERCENT`, `unit:DeciB`)

### Bilingual Labels
- All concepts include English (`@en`) and Spanish (`@es`) labels
- PrefLabels, AltLabels, Definitions, and Comments are provided in both languages

### Hierarchical Organization
- Uses `skos:narrower` and `skos:broader` for hierarchical relationships
- Top concepts defined via `skos:hasTopConcept` in the concept scheme

## Relationship Between Vocabularies

The two vocabularies work together to enable complete sensor observation modeling:

1. **FeaturesOfInterest** reference **ObservableProperties** from SensorVariables via `sosa:hasProperty` relationships
2. This separation allows:
   - Reusable property definitions in SensorVariables
   - Contextual grouping of properties by what is being observed (FeatureOfInterest)
   - Flexible observation modeling following SOSA patterns

### Example Observation Pattern

```turtle
# A sensor observes a property of a feature
:observation1 a sosa:Observation ;
    sosa:observedBy :sensor1 ;
    sosa:observes edintkos-vars:AirTemperature ;
    sosa:featureOfInterest edintkos-foi:Air ;
    sosa:hasSimpleResult "22.5"^^xsd:decimal ;
    qudt:unit unit:DEG_C .
```

In this pattern:
- `edintkos-foi:Air` (FeatureOfInterest) has `edintkos-vars:AirTemperature` as a property
- The observation links both the feature and the property being measured

## File Structure

| File | Description |
|------|-------------|
| [`kos/sensor-variables.ttl`](sensor-variables.ttl) | The sensor variables thesaurus - defines all observable properties with hierarchical categorization |
| [`kos/feature-of-interest.ttl`](feature-of-interest.ttl) | The features of interest vocabulary - defines observable features with links to properties |

## Best Practices

- Keep vocabulary versions clearly labeled and documented
- Validate syntax and semantics before committing changes
- Maintain consistency with conceptual diagrams and documentation
- Use standardized namespace and prefix strategy

## Notes

- This folder contains only **implementation files** — not diagrams, notes, or documentation
- Consider adding a changelog or version history if multiple vocabulary versions are maintained
