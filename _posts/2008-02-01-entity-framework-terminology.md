---
layout: post
title: Entity Framework Terminology
date: 2008-02-01 18:53
author: John
comments: true
categories: [All]
---
<p>I have some articles to write&nbsp;on the Entity Framework and&nbsp;LINQ to ADO.NET, so I will be busy in the depths of EF for a while.&nbsp;I have been spending the past few days immersing myself in the Orcas March CTP. While there are features I am still longing for (such as the EDM Designer) this is the most EF &amp; LINQ complete CTP in a long time. While the MSDN Documentation is not complete by any means, there is some great information in there. For example, I found this fantastic page in the help docs that is a glossary of the Entity Framework terminology. I pulled this directly from their documentation, which you can find at this link (ms-help://MS.MSDNQTR.v90.en/MS.MSDN.v90/MS.VisualStudio.v90.en/WD_ADONET/html/fa2a1bd1-6118-487b-8673-eebc66b92945.htm ) in the March CTP&#39;s help docs. This is a great reference to lean on when learning the EF ... kudos to the data team for creating and including this information in the CTP.</p><p>&nbsp;</p><p><font color="#4f81bd" face="Cambria" size="4">Entity Framework terminology:</font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">alias</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>An attribute of the Schema element in CSDL and SSDL schemas that can be substituted for the full namespace to shorten element references in the schema.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">association</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>The definition of a relationship between entity types.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">association set</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A logical container for instances of associations of the same type. </font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">base type</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A parent type or super-type in the EDM from which derived types inherit some of their properties. </font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">complex type</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>An entity type whose properties have internal properties. Used as a property of an entity type or of another complex type. </font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">conceptual schema definition language (CSDL)</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>XML-based dialect used to define the entity types, associations, entity containers, entity sets, and association sets of a conceptual model. </font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">conceptual model</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>Abstract specification for the entity types, associations, entity containers, entity sets, and association sets comprising an application domain. </font></font></font></p><p class="MsoNormal" style="margin: 0in 0in 10pt"><font color="#1f497d" face="Calibri" size="3"></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">constraint</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>Restricts the possible values of a property and ensures that a value is valid. </font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">container</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A logical grouping of entity and association sets. </font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">degree</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>The number of entity types in a relationship. Relationships are classified as unary, binary, ternary, or n-ary. </font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">direction</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>Refers to the asymmetrical nature of some associations. Direction is specified with FromRole and ToRole attributes of ReferentialConstraint elements in entity data models.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">end</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A participating entity in an association. </font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">entity</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>An instance of an entity type.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">EntityClient</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A storage-independent ADO.NET data provider containing classes such as EntityConnection, EntityCommand, and EntityDataReader. Works with Entity SQL and connects to storage specific ADO.NET Data Providers, such as SqlClient.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">entity container</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>Specifies the sets of entity types and associations that will be available in a specified namespace. </font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">Entity Data Model (EDM)</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A system for defining application data as sets of entities and relationships.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">Entity Framework</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A set of technologies that supports development of data-oriented software applications by allowing developers to work with conceptual models that are mapped to logical schemas in data sources.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">entity-relationship model</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A data model that uses relationships between entities as the basis for describing application data schemas. </font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">entity set</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A logical container for entities of the same type, mapped to tables in a database. </font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">Entity SQL</font></h3><
p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A storage-independent dialect of SQL that works directly with conceptual entity schemas and that supports entity data model features such as inheritance and relationships.</font></font></font></p><p class="MsoNormal" style="margin: 0in 0in 10pt"><font color="#1f497d" face="Calibri" size="3"></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">entity type</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A named set of properties representing a top-level item in a data model.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">enumeration</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A simple type whose single value is selected from a specified set of options. </font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">facet</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A constraint, such as Nullable, MaxLength, or Precision, that limits the allowable values for a property.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">helper method</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>User-defined operations implemented in partial classes that add functionality to objects generated from entity data models.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">key</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>The attribute of an entity type that specifies which property or set of properties is used to identify unique instances of the entity type.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">language integrated query (LINQ)</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A query syntax that defines a set of query operators that allow traversal, filter, and projection operations to be expressed in a direct, declarative way in C# and Visual Basic.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">LINQ to Entities</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>The use of language integrated query operators with objects representing a conceptual model.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">mapping</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A set of correspondences between items in a conceptual model and items in a storage model.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">mapping specification language (MSL)</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>An XML-based dialect used to map items defined in a conceptual model to items in a storage model.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">metadata</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>Data used to describe the structure of other data, including the SSDL XML file, which describes the structure of data in a data store. </font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">Metadata Workspace</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A class that represents the metadata runtime service component that provides support for retrieving metadata. </font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">multiplicity</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>The number of entities that can exist on each side of a relationship. </font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">navigation property</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A property of entity types that uses an association to reference related entities.</font></font></font></p><p class="MsoNormal" style="margin: 0in 0in 10pt"><font color="#1f497d" face="Calibri" size="3"></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">object services</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>Services provided by the Entity Framework to classes generated from a set of metadata.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">object context</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A base class that provides object services such as tracking and saving changes, and that contains a connection to the underlying data store.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">referential constraint</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>An element of an SSDL entity data model that specifies the direction of an association with FromRole and ToRole attributes. Corresponds to a CSDL navigation property.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">relational model</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>The logical model used to define the tables, columns, and constraints in a database.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">relationship</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A logical connection between entities. </font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">role</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>The name given to each end of an association to clarify the semantics of the relationship.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">simple type </font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>Primitive type used for defining properties in entity data models.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">store schema definition language (SSDL)</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>XML-based dialect used to define the entity types, associations, entity containers, entity sets, and association sets of a storage model, often corresponding to a database schema. </font></font></font></p><h3 st
yle="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">table-per hierarchy (TPH)</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A method of modeling a type hierarchy in a database that includes the attributes of all the types in the hierarchy in one table.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">table-per-type (TPT)</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>A method of modeling a type hierarchy in a database that uses multiple tables with one-to-one relationships to model the various types.</font></font></font></p><h3 style="margin: 10pt 0in 0pt"><font color="#4f81bd" face="Cambria" size="3">XML (simple type)</font></h3><p class="MsoNormal" style="margin: 0in 0in 10pt"><font size="3"><font color="#1f497d"><font face="Calibri"><span>&nbsp;</span>Can contain well-formed XML or valid XML data. The facets of this type control which kind of XML data can be contained within it. </font></font></font></p><p class="MsoNormal" style="margin: 0in 0in 10pt"><font color="#1f497d" face="Calibri" size="3"></font></p>
