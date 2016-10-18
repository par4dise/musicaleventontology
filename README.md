# Musical event ontology
Ontology of a musical event ; initiated for a scholar project in computing MSc.  
Mostly in french, sorry.  

### Files
*meo-model.rdf*: OWL ontology in RDF format  
*MusicEventOntology.png*: simplified schema of the ontology  
*MusicEventOntology full.png*: full graphical representation of the ontology  
*MusicEventArchitecture.png*: architecture of web client (see below)  

### Web client
See https://github.com/chenyang/FindEvent

### History
v0.5
* Ajout de la classe #DataBusiness pour les annotations
* Ajout de la propriété #hasForTarget
* Suppression de la classe #Artist
* Suppression de la propriété #hasForMember
* Ajout de commentaires FRA/ENG pour toutes les classes/propriétés

v0.4
* Ajout de <rdfs:comment> pour décrire une évènement musical
* Suppression de la propriété #aPourGroupe afin d'éviter le doublon avec #aPourMembre
* Traduction en anglais
* Tous les genres sont <skos:broader> de #MusicalGenre

v0.3
* Séparation modèle/instances
* Ajout de rdfs:label un peu partout
* Remplacement de <schema:startDate> et <schema:endDate> (dont les domaines sont spécifiés) par les propriétés #dateDebut et #dateFin 

v0.2
* Ajout du namespace schema ="http://schema.org/Event"
* Ajout de <rdfs:equivalentClass rdf:resource="schema:MusicEvent"/> dans la classe #EvenementMusical
* Ajout de <owl:equivalentProperty rdf:resource="schema:subEvent" /> dans la propriété #seComposeDe
* Remplacement de <owl:equivalentProperty rdf:resource="foaf:member" /> par <owl:equivalentProperty rdf:resource="mo:member" /> dans la propriété #aPourMembre
* Ajout de <owl:equivalentProperty rdf:resource="schema:performer" /> dans la propriété #aPourParticipant
* Ajout des propriétés <schema:startDate> et <schema:endDate> à meo:EvenementMusical
* Ajout de <foaf:homepage> et <meo:aPourGenre> dans les instances d'artistes
* Suppression des foaf:firstName, foaf:lastName et foaf:name dans les instances d'artistes
* Suppression de commentaires inutiles

v0.1
* 1ère version

## Inspiration
*A Distributed Music Information System* [PhD thesis](http://raimond.me.uk/phd/) by Yves Raimond.

### Licence
Music Event Ontology est mis à disposition selon les termes de la licence [Creative Commons Attribution -  Partage dans les Mêmes Conditions 4.0 International](http://creativecommons.org/licenses/by-sa/4.0/).   
![CC BY 4.0 logo](https://i.creativecommons.org/l/by/4.0/88x31.png "CC BY 4.0 logo")
