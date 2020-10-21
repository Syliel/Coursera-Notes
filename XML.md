Python Dictionary ---> Serialize ---> De-serialize ---> Java HashMap
Two types of serialization = XML (older), JSON (newer)

XML = eXtensible Markup Language:
	a. Primary purpose is to help information systems share structured
	data
	b. It started as a simplified subset of the Standard Generalized Markup
	Language (SGML), and is designed to be relatively human-legible

XML "Elements" (or Nodes): < = start tag, </ = end tag

<people>
 <person>
  <name>Jenni</name>      <---- Simple Element
  <phone>303 4456</phone>
 </person>                <---- Complex Element
  <name>Noah</name>       
  <phone>622 7421</phone>
 </person>
</people>

XML Basics: White space doesn't matter, except in between text content

<person>                      <---- Start Tag
 <name>Chuck</name>
 <phone type="intl">          <---- Attribute (Key Value pairs, Always on Start)
  +1 734 303 4456             <---- Text Content
 </phone>
 <email hide="yes"/>          <---- Self Closing Tag
</person>                     <---- End Tag  

XML Schema:
	a. Describing a "contract" as to what is acceptable XML.
	b. Description of the legal format of an XML document
	c. Expressed in terms of constraints on the structure and content of
	documents
	d. Often used to specify a "contract" between systems - "My system
	will only accept XML that conforms to this particular Schema."
	e. If a particular piece of XML meets the specification of the Schema
	it is said to "validate"

Many XML Schema Languages
a. Document Type Definition (DTD)
	o http://en.wikipedia.org/wiki/Document_Type_Definition
b. Standard Generalized Markup Language (ISO 8879:1986 SGML)
	o http://en.wikipedia.org/wiki/SGML
c. XML Schema from W3C - (XSD)
	o http://en.wikipedia.org/wiki/XML_Schema_(W3C)

XML Schema from W3c - (XSD) is mostly used

XDS XML Schema (W3C spec):
a. We will focus on the World Wide Web Consortium (W3C) version
b. It is often called "W3C Schema" because "Schema" is considered generic
c. More commonly it is called XSD because the file names end in .xsd
d. Date format: YYYY-MM-DD Date/Time: YYYY-MM-DDT09:30:10Z (Z is timezone UTC)
e. Timezone - typically specified in UTC/GMT rather than local time zone
