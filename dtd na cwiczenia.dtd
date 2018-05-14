<?xml encoding="UTF-8"?>

<!ELEMENT Configuration (SynchronizationAgent,ExchangeServer,
                         DataSetsConfiguration+)>
<!ATTLIST Configuration
  xmlns CDATA #FIXED ''>

<!ELEMENT SynchronizationAgent (TempDataLocation)>
<!ATTLIST SynchronizationAgent
  xmlns CDATA #FIXED ''
  server NMTOKEN #REQUIRED
  server_agent_nr CDATA #REQUIRED>

<!ELEMENT ExchangeServer EMPTY>
<!ATTLIST ExchangeServer
  xmlns CDATA #FIXED ''
  RootCatalog NMTOKEN #REQUIRED
  URL NMTOKEN #REQUIRED
  login NMTOKEN #REQUIRED
  pass CDATA #REQUIRED>

<!ELEMENT DataSetsConfiguration (DataSetConfiguration)+>
<!ATTLIST DataSetsConfiguration
  xmlns CDATA #FIXED ''
  mode NMTOKEN #REQUIRED
  retrieveDataTriesNumber CDATA #IMPLIED>

<!ELEMENT TempDataLocation EMPTY>
<!ATTLIST TempDataLocation
  xmlns CDATA #FIXED ''
  Database NMTOKEN #REQUIRED
  Password NMTOKEN #REQUIRED
  Server NMTOKEN #REQUIRED
  UserId NMTOKEN #REQUIRED
  dbtype NMTOKEN #REQUIRED
  type NMTOKEN #REQUIRED>

<!ELEMENT DataSetConfiguration (Schedule,DataArea+)>
<!ATTLIST DataSetConfiguration
  xmlns CDATA #FIXED ''
  ID NMTOKEN #REQUIRED>

<!ELEMENT Schedule EMPTY>
<!ATTLIST Schedule
  xmlns CDATA #FIXED ''
  every CDATA #IMPLIED
  time NMTOKEN #IMPLIED
  type NMTOKEN #REQUIRED>

<!ELEMENT DataArea (DataLocation,Actions?,DataDefinition)>
<!ATTLIST DataArea
  xmlns CDATA #FIXED ''
  FileExistAction NMTOKEN #IMPLIED
  ID NMTOKEN #REQUIRED
  type NMTOKEN #REQUIRED>

<!ELEMENT DataLocation EMPTY>
<!ATTLIST DataLocation
  xmlns CDATA #FIXED ''
  Database NMTOKEN #IMPLIED
  Password NMTOKEN #IMPLIED
  Server NMTOKEN #IMPLIED
  UserId NMTOKEN #IMPLIED
  dbtype NMTOKEN #IMPLIED
  path CDATA #IMPLIED
  type NMTOKEN #REQUIRED>

<!ELEMENT Actions (Before+,After*)>
<!ATTLIST Actions
  xmlns CDATA #FIXED ''>

<!ELEMENT DataDefinition (Filter|(Query,Mapping))?>
<!ATTLIST DataDefinition
  xmlns CDATA #FIXED ''>

<!ELEMENT Before EMPTY>
<!ATTLIST Before
  xmlns CDATA #FIXED ''
  expression CDATA #REQUIRED
  job_name CDATA #REQUIRED
  sql_type NMTOKEN #REQUIRED
  type NMTOKEN #REQUIRED>

<!ELEMENT After EMPTY>
<!ATTLIST After
  xmlns CDATA #FIXED ''
  FireWhen NMTOKEN #REQUIRED
  expression CDATA #REQUIRED
  job_name CDATA #REQUIRED
  sql_type NMTOKEN #REQUIRED
  type NMTOKEN #REQUIRED>

<!ELEMENT Filter EMPTY>
<!ATTLIST Filter
  xmlns CDATA #FIXED ''
  extension NMTOKEN #REQUIRED
  fileNamePattern CDATA #REQUIRED>

<!ELEMENT Query EMPTY>
<!ATTLIST Query
  xmlns CDATA #FIXED ''
  sql CDATA #REQUIRED
  sql_type NMTOKEN #REQUIRED>

<!ELEMENT Mapping (Field)+>
<!ATTLIST Mapping
  xmlns CDATA #FIXED ''>

<!ELEMENT Field EMPTY>
<!ATTLIST Field
  xmlns CDATA #FIXED ''
  destination NMTOKEN #REQUIRED
  source NMTOKEN #REQUIRED>
