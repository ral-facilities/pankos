Changes to v1.0
---------------

- intoduction of Version IRI
- Introduced Detector.  Microscope etc. are now subclasses of detector (before it was instrument, but an instrument can have many detectors)
- removed individual of instruments and facilities because they might not be up to date, they were not registered consitently (did not have a type - not declared as instrument), sometimes detectors instead of beamlines were registered e.g. EIGER (might be wrong with this assumption)
- dcterms:MediaType is no Subtype of contributer (removed relation Individual Contributer)
- added SampleEnvironment
	pressureMax
	temperatureMax
	temperatureMin

- added DataProperties to ObjectsCharacteristics
	energyRangeMax
	energyRangeMin
	energyResolution
	fluxOnSampleMax
	resolvingPower
	spotSizeOnSampleHor
	spotSizeOnSampleVert
	Units --> we need to find registered Units: http://dtr-test.pidconsortium.eu/#objects/?query=energy, http://www.ontology-of-units-of-measure.org/resource/om-2/Pressure
	Description
- deleted sublcass of Technique : inFacility 

Proposal
--------
- Use CalipsoPLUS terms for describing instruments (e.g. http://www.wayforlight.eu/en/beamline/21570)
- Add CallipsoPLUS Disciplines or verify mapping to PaNKOS Disciplines
- Review disciples of PanKOS if they are the same as on CallipsoPLUS
---> The instrument class should be aligned with the RDA PID Instrument and Individuals should be registered at DataCite and get a DOI. (We should ask, if we propose a PaN PID for Instruments with CallipsoPLUS Attributes?)

- Mapp CallipsoPLUS instrument description to NeXus definitions

- add some comments/documentation to the classes and properties 



Questions
---------

- How to use ValuePartitions? (are these Kategories)
- NuclearPraticlePhysics sound like a discipline not like an instrument or detector type?


