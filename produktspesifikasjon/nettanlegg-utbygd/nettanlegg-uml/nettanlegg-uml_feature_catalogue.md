#### Transformatorstasjon

stasjon som transformerer spenningen fra ett spenningsnivå til et annet

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>geometri</td>
      <td>registreres geometri</td>
      <td>GM_<wbr />Point</td>
      <td>1</td>
    </tr>
    <tr>
      <td>spenning_<wbr />k<wbr />V</td>
      <td>spenning er kraften eller trykket som skyver strøm gjennom kraftledninger. Her angitt i kilovolt (kV)</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td></td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- målemetode</td>
      <td>metode for måling i grunnriss (x,y), og høyde (z) når metoden er den samme som ved måling i grunnriss</td>
      <td><a href="#kodeliste-målemetode">Målemetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>punktstandardavviket i grunnriss for punkter samt tverravvik for linjer<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra NettanleggUtbygdFellesEgenskaper</th>
    </tr>
    <tr>
      <td>nettnivå</td>
      <td>nettnivå viser inndelingen av det norske strømnettet. Det er inndelt etter ulike spenningsnivåer og funksjonalitet.<br /><br />Merknad: Ikke alle kodeverdier brukes i DOK-datasettet</td>
      <td><a href="#kodeliste-nvenettnivå">Nve<wbr />Nettnivå</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>drifter</td>
      <td>innrapportert navn på drifter/konsesjonær</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>drifter<wbr />Orgnr</td>
      <td>organisasjonsnummer til innrapportert drifter/konsesjonær</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>navn på stasjon eller ledningsstrekket, typisk vil dette være en plasseringsangivelse av typen 'fra stasjon - til stasjon', eventuelt et mastenummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>driftsattår</td>
      <td>årstall anlegg ble idriftsatt</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for når konsesjonær/drifter sendte dataene inn til NVEs databaser</td>
      <td>Date<wbr />Time</td>
      <td>1</td>
    </tr>
    <tr>
      <td>ident</td>
      <td>unik identifikasjon av et objekt</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br /><br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br /><br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br /><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
NettanleggUtbygdFellesEgenskaper

#### NettanleggUtbygdFellesEgenskaper

abstrakt objekt som bærer fellesegenskaper

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>nettnivå</td>
      <td>nettnivå viser inndelingen av det norske strømnettet. Det er inndelt etter ulike spenningsnivåer og funksjonalitet.<br /><br />Merknad: Ikke alle kodeverdier brukes i DOK-datasettet</td>
      <td><a href="#kodeliste-nvenettnivå">Nve<wbr />Nettnivå</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>drifter</td>
      <td>innrapportert navn på drifter/konsesjonær</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>drifter<wbr />Orgnr</td>
      <td>organisasjonsnummer til innrapportert drifter/konsesjonær</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>navn på stasjon eller ledningsstrekket, typisk vil dette være en plasseringsangivelse av typen 'fra stasjon - til stasjon', eventuelt et mastenummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>driftsattår</td>
      <td>årstall anlegg ble idriftsatt</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for når konsesjonær/drifter sendte dataene inn til NVEs databaser</td>
      <td>Date<wbr />Time</td>
      <td>1</td>
    </tr>
    <tr>
      <td>ident</td>
      <td>unik identifikasjon av et objekt</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br /><br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br /><br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br /><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
  </tbody>
</table>

#### Mast

konstruksjon for å feste ledninger eller andre objekter i. Kan bestå av en eller flere stolper. Kan være konstruert i tre, metall, kompositt eller betong

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>mastehøyde</td>
      <td>mastehøyde i meter (m). Referansehøyde varierer, men typisk er høydeangivelsen mastas høyde over bakken</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>geometri</td>
      <td>registreres geometri</td>
      <td>GM_<wbr />Point</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td></td>
      <td>Posisjonskvalitet<wbr />H<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- målemetode</td>
      <td>metode for måling i grunnriss (x,y), og høyde (z) når metoden er den samme som ved måling i grunnriss</td>
      <td><a href="#kodeliste-målemetode">Målemetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>punktstandardavviket i grunnriss for punkter samt tverravvik for linjer<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- målemetode<wbr />Høyde</td>
      <td>metode for å måle objekttypens høydeverdi</td>
      <td><a href="#kodeliste-målemetode">Målemetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>nøyaktighet for høyden i cm</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra NettanleggUtbygdFellesEgenskaper</th>
    </tr>
    <tr>
      <td>nettnivå</td>
      <td>nettnivå viser inndelingen av det norske strømnettet. Det er inndelt etter ulike spenningsnivåer og funksjonalitet.<br /><br />Merknad: Ikke alle kodeverdier brukes i DOK-datasettet</td>
      <td><a href="#kodeliste-nvenettnivå">Nve<wbr />Nettnivå</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>drifter</td>
      <td>innrapportert navn på drifter/konsesjonær</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>drifter<wbr />Orgnr</td>
      <td>organisasjonsnummer til innrapportert drifter/konsesjonær</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>navn på stasjon eller ledningsstrekket, typisk vil dette være en plasseringsangivelse av typen 'fra stasjon - til stasjon', eventuelt et mastenummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>driftsattår</td>
      <td>årstall anlegg ble idriftsatt</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for når konsesjonær/drifter sendte dataene inn til NVEs databaser</td>
      <td>Date<wbr />Time</td>
      <td>1</td>
    </tr>
    <tr>
      <td>ident</td>
      <td>unik identifikasjon av et objekt</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br /><br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br /><br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br /><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
NettanleggUtbygdFellesEgenskaper

#### Luftledning

ledninger plassert over bakken, for overføring av elektrisitet i kraftnettet

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>geometri</td>
      <td>registreres geometri</td>
      <td>GM_<wbr />Curve</td>
      <td>1</td>
    </tr>
    <tr>
      <td>spenning_<wbr />k<wbr />V</td>
      <td>spenning er kraften eller trykket som skyver strøm gjennom kraftledninger. Her angitt i kilovolt (kV)</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td></td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- målemetode</td>
      <td>metode for måling i grunnriss (x,y), og høyde (z) når metoden er den samme som ved måling i grunnriss</td>
      <td><a href="#kodeliste-målemetode">Målemetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>punktstandardavviket i grunnriss for punkter samt tverravvik for linjer<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra NettanleggUtbygdFellesEgenskaper</th>
    </tr>
    <tr>
      <td>nettnivå</td>
      <td>nettnivå viser inndelingen av det norske strømnettet. Det er inndelt etter ulike spenningsnivåer og funksjonalitet.<br /><br />Merknad: Ikke alle kodeverdier brukes i DOK-datasettet</td>
      <td><a href="#kodeliste-nvenettnivå">Nve<wbr />Nettnivå</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>drifter</td>
      <td>innrapportert navn på drifter/konsesjonær</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>drifter<wbr />Orgnr</td>
      <td>organisasjonsnummer til innrapportert drifter/konsesjonær</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>navn på stasjon eller ledningsstrekket, typisk vil dette være en plasseringsangivelse av typen 'fra stasjon - til stasjon', eventuelt et mastenummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>driftsattår</td>
      <td>årstall anlegg ble idriftsatt</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for når konsesjonær/drifter sendte dataene inn til NVEs databaser</td>
      <td>Date<wbr />Time</td>
      <td>1</td>
    </tr>
    <tr>
      <td>ident</td>
      <td>unik identifikasjon av et objekt</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br /><br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br /><br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br /><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
NettanleggUtbygdFellesEgenskaper

#### Sjøkabel

kabler plassert i vannsøylen eller på bunnen av elv/innsjø/fjord/hav, for overføring av elektrisitet i kraftnettet

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>geometri</td>
      <td>registreres geometri</td>
      <td>GM_<wbr />Curve</td>
      <td>1</td>
    </tr>
    <tr>
      <td>spenning_<wbr />k<wbr />V</td>
      <td>spenning er kraften eller trykket som skyver strøm gjennom kraftledninger. Her angitt i kilovolt (kV)</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td></td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- målemetode</td>
      <td>metode for måling i grunnriss (x,y), og høyde (z) når metoden er den samme som ved måling i grunnriss</td>
      <td><a href="#kodeliste-målemetode">Målemetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>punktstandardavviket i grunnriss for punkter samt tverravvik for linjer<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra NettanleggUtbygdFellesEgenskaper</th>
    </tr>
    <tr>
      <td>nettnivå</td>
      <td>nettnivå viser inndelingen av det norske strømnettet. Det er inndelt etter ulike spenningsnivåer og funksjonalitet.<br /><br />Merknad: Ikke alle kodeverdier brukes i DOK-datasettet</td>
      <td><a href="#kodeliste-nvenettnivå">Nve<wbr />Nettnivå</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>drifter</td>
      <td>innrapportert navn på drifter/konsesjonær</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>drifter<wbr />Orgnr</td>
      <td>organisasjonsnummer til innrapportert drifter/konsesjonær</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>navn på stasjon eller ledningsstrekket, typisk vil dette være en plasseringsangivelse av typen 'fra stasjon - til stasjon', eventuelt et mastenummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>driftsattår</td>
      <td>årstall anlegg ble idriftsatt</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for når konsesjonær/drifter sendte dataene inn til NVEs databaser</td>
      <td>Date<wbr />Time</td>
      <td>1</td>
    </tr>
    <tr>
      <td>ident</td>
      <td>unik identifikasjon av et objekt</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br /><br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br /><br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br /><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
NettanleggUtbygdFellesEgenskaper

### Kodelister

#### <a id="kodeliste-målemetode"></a>«CodeList» Målemetode

**Definisjon:** metode som ligger til grunn for registrering av posisjon


-- Definition - -
method on which registration of position is based

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="https://register.geonorge.no/sosi-kodelister/generelle-konsepter/4.5/målemetodekode">https://register.geonorge.no/sosi-kodelister/generelle-konsepter/4.5/målemetodekode</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-nvenettnivå"></a>«CodeList» NveNettnivå

**Definisjon:** nvenettnivå viser inndelingen av det norske strømnettet. Det er inndelt etter ulike spenningsnivåer og funksjonalitet.

Merknad: Ikke alle kodeverdier brukes i DOK-datasettet

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="https://register.geonorge.no/sosi-kodelister/energi/nvenettniv%C3%A5">https://register.geonorge.no/sosi-kodelister/energi/nvenettniv%C3%A5</a></td>
    </tr>
  </tbody>
</table>
