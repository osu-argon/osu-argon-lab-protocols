# Constructing Mineral Separation Recipes

## Structure of Recipes, Methods and Procedures

***Recipes*** are a sequence of methods that are used to process a sample for analysis.
***Methods*** are a sequence of procedures that are used to perform a specific task during sample preparation.
***Procedures*** are individual instructions on how to perform specific tasks in the lab.


1. Recipes
    1. Procedures
        1. Tasks

Below are lists of methods in order to build a recipe for mineral separation.

## [Sample Preparation](https://paper.dropbox.com/doc/Sample-Preparation--Ao9quEt4fJzKgnOa8Y29IJe0AQ-MDUr6WjOzRLZEGKCGwlTj) Fields

These methods will describe the steps necessary before mineral separation begins. Such as sample description, taking pictures of thin sections and determining a recipe for the sample.

**Prefix for sample preparation fields**

    prepare_


- prepare
    - Preparing a sample involves reviewing the sample recipe and double checking the project ID and sample ID.
- prepare_slab
    - Sample needs to be cut into 1-inch slabs before the sample is crushed. Saw away weathering rind if possible.
- prepare_TSB
    - Sample is to be slabbed and a portion selected to be sent for a thin section.
- prepare_TSB_XRF
    - Thin section to be sent and a portion of the sample is to be prepared for XRF.
- prepare_XRF
    - A portion of the sample needs to be prepared and sent for XRF analysis.


## [Crushing Methods](https://paper.dropbox.com/doc/Crushing-Methods--Ao8nYpdbHGwTH9ZOrlpYAmwsAQ-sqs4XHKNA7d7C6ua9e9Dr) Fields

Methods that will provide guidance on how to go about crushing samples using specific equipment in the lab.

**Prefix for crushing fields**

    crush_


- crush_jaw_large
    - For large amounts of sample.
- [crush_jaw_small](https://paper.dropbox.com/doc/small_jaw_crush--AkcqVVv7f2EAq7wu0EEopEFEAQ-SZkqg26AQLHnECiWcW1qJ)
    - For small amounts of sample or when more crushing control is needed.
- crush_hammer
    - To break up large pieces of sample for use in the small or large jaw crusher.
- crush_mortar_pestle
    - To use when the sample amount is small or finer control over the crushing of the sample is needed.


## Sieve Method Field

**Prefix for sieve fields**

    sieve_
      large = large diameter sieves generally used for processing large amounts of sample.
      small = small diamter sieves generally used for processing small amounts of sample.
      xx-xx = sieve opening size in microns


- sieve_large_150-350
- sieve_large_350-800
- sieve_small_150-350
- sieve_small_350-800


## Separation Methods Fields

**Prefix for magnetic separation fields**

    magnetic_sep_


- magnetic_sep_basalt
- magnetic_sep_feldspar
- magnetic_sep_amphibole
- magnetic_sep_mica


## Heavy Liquid Fields 

**Prefix for Heavy Liquid Fields**

    heavy_liq_


- heavy_liq_2582_float
    - Target: Glass, Sanidine
- heavy_liq_2582_sink
    - Target: Biotite, Amphiboles, Plagioclase
- heavy_liq_2560_float
    - Target: Glass
- heavy_liq_2560_sink
    - Target: Sanidine
- heavy_liq_2800_sink


## [Acid Leaching](https://paper.dropbox.com/doc/Acid-Leaching-Method--Ao8L47vzdO93qRNM5WZdrfKmAQ-goRn1YumqtEXuCObodBlr) Method Fields

**Prefix for Acid Leaching Fields**

    acid_leach_
- acid_leach_concentrate
    - Samples are leached using 6N HCl, 1N HCl, 3N HNO3 and 1N HNO3 for 60 minutes each.
- acid_leach_dilute
    - Samples are leached using 1N HCl and 1N HNO3 for 60 minutes each.



## [HF Leach](https://paper.dropbox.com/doc/HF-Leaching-Methods--Ao~qr3rhZDxt70HlzIZd6phzAQ-jxDM56JPcdqTQwJYzWmXi) Fields

**Prefix for HF Leach Fields**

    leach_HF


- leach_HF_5%_03_min
    - Material: Glass, Groundmass
- leach_HF_5%_08_min
    - Material: Plagioclase, Amphiboles
- leach_HF_15%_07_min
    - Material: Sanidine

## Picking Method Fields

**Prefix for Pick Fields**

    pick_material_--mg
    --mg = amount of material to pick and pack for irradiation in grams.
    --xyl = number of crystals to pick and pack for irradiation.
- [pick_groundmass](https://paper.dropbox.com/doc/Picking-Samples--AnPRl~NT7CTHoZ54MLp3T43~AQ-ehgTtv4nfGVpO10Jz1Y3p)
- pick_feldspar
- pick_mica
- pick_amphibole


## Archive Fields

The archive field will describe what the current state the sample is in after it has been sent for irradiation. Samples will be stored temporarily in Burt before being stored at MGR or being returned to the client or researcher.

**Prefix for Archive Fields**

    archive_


- archive_in_burt
    - Samples are stored in Burt until the samples have been analyzed.
- archive_in_mgr
    - Samples are sent for long-term storage at MGR once the project is complete.
- archive_sent_pi
    - Samples are to be returned to the investigator.


## Pack for Irradiation Fields

**Prefix for Pack Fields**
`pack_`


- pack_
- 
## Examples - Mineral Separation Recipes
### Groundmass - Basalt
- groundmass_basalt_fine
    - prepare_TS
    - crush_jaw_small
    - sieve_small_150-350
    - magnetic_sep_basalt
    - acid_leach_concentrate
    - pick_groundmass_10mg
    - archive_in_burt


### Plagioclase - Basalt
- plagioclase_basalt_fine
    - prepare_TS
    - crush_jaw_small
    - sieve_small_150-350
    - magnetic_sep_feldspar
    - acid_leach_concentrate
    - leach_HF_5%_08_min 
    - archive_in_burt


### K-feldspar - Volcanic Tuff
- feldspar_K_fine_coarse
    - prepare_TS
    - crush_jaw_small
    - sieve_large_350-800
    - magnetic_sep_feldspar
    - leach_HF_5%_08_min 
    - archive_in_burt


### K-feldspar - Intrusive
- feldspar_K_fine_coarse
    - prepare_TS
    - crush_jaw_small
    - small_jaw_crush
    - sieve_large_350-800
    - magnetic_sep_feldspar
    - acid_leach_concentrate
    - archive_in_burt


### Biotite
- biotite_coarse
    - thin_section_cut
    - small_jaw_crush
    - sieve_large_350-800
    - magnetic_sep_biotite
    - heavy_liquid_2.582
    - pick_biotite
    - archive


### Muscovite
- muscovite_coarse
    - thin_section_cut
    - small_jaw_crush
    - sieve_150_350
    - magnetic_sep_low
    - heavy_liquid_2.582
    - pick
    - archive


### Amphibole
- amphibole_coarse
    - thin_section_cut
    - small_jaw_crush
    - sieve_350_650
    - magnetic_sep_low
    - heavy_liquid_2.582
    - pick
    - archive

