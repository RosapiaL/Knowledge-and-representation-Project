# Knowledge-and-representation-Project
The file "animal-kinodm.owl" must be opened with Protege 5.5.0. It contains an ontology for the animal kingdom. The main objective of the project is to create a structure that can represent the relationships between different animals, their habitats, their physical and  behavioral characteristics, and their ecological interactions.

The ontology was developed using OWL (Web Ontology Language) and Protegé.The ontology is structured starting from the two main classes: **Vertebrates** and **Invertebrates**, which are disjoint, and are subclasses of the general class **Animal**. 
From there, there is a further subdivision of vertebrates into classes such as **Mammals**, **Reptiles**, **Birds**, **Fish**, and **Amphibians**, and invertebrates into **Annelids**, **Arthropods**, **Echinoderms**, and **Mollusks**.
The second important section of the ontology concerns the environment in which  animals live. There are two classes:
 * **Habitat** class for vertebrates, divided into various subclasses such as **Desert**, **Forest**, **Mountain**, **Ocean**, **Savanna**, **Tundra**, and **Wetland**.
 * **Shelter** class for invertebrates.
Then, there is the **Country** class, which represents different countries around the world.

The main **_Object Properties_** are *hasHabitat, hasPrey, hasPredator,livesInShelter, foundInCountry and migratesTo*. 

Each subclass is enriched by a series of specific **_Data Properties_**. For example: 
  * Mammals have a property *bodyTemperature* , which represents their average  body temperature.
  * Some mammals have a carnivorous, herbivorous, or omnivorous diet, represented by the *hasDiet* property.
  * For birds, the *flightSpeed* property represents their flying speed.
  * Reptiles are characterized by a property called *skinType*, which describes their scaly skin.
There are also data properties to represent numerical or textual information about animals, such as their *weight*, *size*, *lifespan*.

In addition to the classes, there have been created several *individuals* in the ontology to represent specific animals, habitats, and countries.

The files DL_queries.txt and SPARQL_queries.txt contain some query executed on the ontology.
