# bot-infection 0.2.0

Date: 2017-02-17

The schema is incompatible to 0.1.0 due to one breaking change.

## Difference to 0.1.0:

 1. The field Bot-Name was renamed to Malware-Name,
 in order to stay consistent with the field Malware-MD5.
 This change breaks compatibility with 0.1.0

 2. Six additional fields have been added to the schema:
  * Destination-ASN
  * Destination-Port
  * Source-ASN
  * Classification-Taxonomy
  * Classification-Type
  * Classification-Identifier

 Some tools, like IntelMQ for example, are
 capable of processing more information than the originating Schema 0.1.0
 supports, thus we added some of these fields, which we consider as
 especially helpful in order to categorise and identify abuse events.

 3. Some fields have been moved within the schema, in order to achieve
 a more clear order of the schema. Moved Fields:
  * User-Agent
  * Date

 4. Fixed indentation of some fields.
