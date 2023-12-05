# E-commerce(Electronics and Gadgets) site ontology


This ontology is designed to model an Electronics and Gadgets E-commerce site, providing a structured framework for organizing and navigating the various electronic devices and gadgets that can be sold on the site. The ontology includes a hierarchy of categories and subcategories for different types of electronics, as well as characteristics and features that can be used to describe and compare these devices. It also incorporates information on accessories and peripherals that can be sold with these devices. It includes data about the products and tracks customer interactions on the website, like viewing product details, purchasing items, and writing reviews. The primary goals of this Knowledge Base are: 

- To enhance customer experience, especially in terms of product discovery, 
- To enable effective customer segmentation, and 
- To facilitate thorough analysis.

The ontology is available in various formats including JSON-LD, and TTL.


## Authors
The ontology was developed by Tareq Md Rabiul Hossain Chy from École nationale supérieure des mines de Saint-Étienne.


## License
The ontology is licensed under the GNU General Public License (GPL) version 3.0. A copy of the license is available in the repository.

## Domain
We considered a fictionary e-commerce website, selling technological products, having two subdomains:
- A **Product domain** storing all the information related to products (categories, subcategories, properties and details);
- A **Customer domain** storing information related to customer accounts on the website and their activities (purchases, product visualizations, reviews,...).

The ontology is stored in the file e-commerce.owl, and has the following size:

Axiom	1315	

Logical axiom count	818	

Declaration axioms count	217	

Class count	44	

Object property count	9	

Data property count	28	

Individual count	129	

Annotation Property count	11

## Motivations and goals
In the E-commerce domain, semantics can really help to derive significant insights from data, in order to
- improve *customer experience* with better product retrieval and recommendation (similar products, related products, products bought together, products bought by similar users,..);
- support *customer analysis and segmentation*, diving customers basing on patterns or definitions related to their actions on the website, allowing to segment by country (looking at delivery locations), by categories or macro-categories of products they are interested in (ex: AppleFan, GamerCustomer), or *gold customers* (spending a lot of money on the website), and to analyze single user histories but also customer preferences over products (best seller product, most clicked product, most reviewed,...).

Moreover, the use of an ontology instead of a standard database allows to have a flexible representation of the domain, making possible to instanciate different properties for different category of products, without respecting a predefined schema with predefined property names.

## Querying and reasoning
Thanks to Protègè flexibility (many plugins, reasoners, views, query languages) and usability (good graphic interface), we were able to easily reason and query extracting interesting insights from our toy dataset.
Reasoning and inference has been done using *Pellet* reasoner.

We performed the following **Reasoning tasks** using OntoDebug plugin:
- Knowledge Base **consistency** and **coherency** checking;
- **Atoms entailment** (entailed and non-entailed test cases are stored as annotations in the KB);
- **Solving inconsistencies** using the Debugger;

We also queried the KB using the supported query languages:
- **DL queries** (description logics, Open World Assumption);
- **SPARQL queries** (triple based, Closed World Assumption).


## How to use this repository
1. Download *Protègè* (or the latest version that you find) and Pellet, SPARQL, DLquery tabs
2. Import e-commerce.owl in Protègè 
3. Start Pellet resoner to debug and to inferences
4. Copy queries contained in folders SPARQL-queries, DL-queries of this repo and paste them in the correspondent tab of Protègè

