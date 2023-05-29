
# Schema Types

<details>
  <summary><strong>Table of Contents</strong></summary>

  * [Query](#query)
  * [Mutation](#mutation)
  * [Objects](#objects)
    * [Authorization](#authorization)
    * [BrandPion](#brandpion)
    * [Card](#card)
    * [Cards](#cards)
    * [DateWithGranularity](#datewithgranularity)
    * [Home](#home)
    * [HomeBasicInfo](#homebasicinfo)
    * [HomeBuildingSocietyInfo](#homebuildingsocietyinfo)
    * [HomeConstruction](#homeconstruction)
    * [HomeElectricity](#homeelectricity)
    * [HomeHeatingAndCooling](#homeheatingandcooling)
    * [HomeMortgage](#homemortgage)
    * [HomeProperty](#homeproperty)
    * [HomeRoomsAndFloors](#homeroomsandfloors)
    * [HomeSecurityAndInsurance](#homesecurityandinsurance)
    * [HomeSettings](#homesettings)
    * [HomeValuation](#homevaluation)
    * [HomeWaterAndSewer](#homewaterandsewer)
    * [ImageFile](#imagefile)
    * [NotePion](#notepion)
    * [PDFFile](#pdffile)
    * [PDFPion](#pdfpion)
    * [PhotoPion](#photopion)
    * [Task](#task)
    * [TasksList](#taskslist)
    * [UrlPion](#urlpion)
    * [User](#user)
    * [ValueWithUnit](#valuewithunit)
  * [Inputs](#inputs)
    * [DateWithGranularityInput](#datewithgranularityinput)
    * [HomeBasicInfoInput](#homebasicinfoinput)
    * [HomeBuildingSocietyInfoInput](#homebuildingsocietyinfoinput)
    * [HomeConstructionInput](#homeconstructioninput)
    * [HomeElectricityInput](#homeelectricityinput)
    * [HomeHeatingAndCoolingInput](#homeheatingandcoolinginput)
    * [HomeMortgageInput](#homemortgageinput)
    * [HomePropertyInput](#homepropertyinput)
    * [HomeRoomsAndFloorsInput](#homeroomsandfloorsinput)
    * [HomeSecurityAndInsuranceInput](#homesecurityandinsuranceinput)
    * [HomeSettingsInput](#homesettingsinput)
    * [HomeValuationInput](#homevaluationinput)
    * [HomeWaterAndSewerInput](#homewaterandsewerinput)
    * [UploadType](#uploadtype)
    * [ValueWithUnitInput](#valuewithunitinput)
  * [Enums](#enums)
    * [PionTypes](#piontypes)
  * [Scalars](#scalars)
    * [Boolean](#boolean)
    * [DateTime](#datetime)
    * [Float](#float)
    * [ID](#id)
    * [Int](#int)
    * [JSON](#json)
    * [String](#string)
  * [Interfaces](#interfaces)
    * [File](#file)
    * [Pion](#pion)

</details>

## Query (Queries)
<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>user</strong></td>
<td valign="top"><a href="#user">User</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>card</strong></td>
<td valign="top"><a href="#card">Card</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cards</strong></td>
<td valign="top"><a href="#cards">Cards</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">homeId</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>home</strong></td>
<td valign="top"><a href="#home">Home</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>homes</strong></td>
<td valign="top">[<a href="#home">Home</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pion</strong></td>
<td valign="top"><a href="#pion">Pion</a></td>
<td>

Single Pion

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>task</strong></td>
<td valign="top"><a href="#task">Task</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">payload</td>
<td valign="top"><a href="#json">JSON</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tasksLists</strong></td>
<td valign="top">[<a href="#taskslist">TasksList</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">homeId</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
</tbody>
</table>

## Mutation (Mutations)
<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>authorize</strong></td>
<td valign="top"><a href="#authorization">Authorization</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">clientKey</td>
<td valign="top"><a href="#id">ID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>addToHomeImages</strong></td>
<td valign="top"><a href="#home">Home</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">home</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">image</td>
<td valign="top"><a href="#uploadtype">UploadType</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refreshToken</strong></td>
<td valign="top"><a href="#authorization">Authorization</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">accessToken</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">refreshToken</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createHome</strong></td>
<td valign="top"><a href="#home">Home</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">title</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">image</td>
<td valign="top"><a href="#uploadtype">UploadType</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">addressLine1</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">addressLine2</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">zipCode</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">city</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">lat</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">lon</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">country</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">countryISO</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">municipality</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">propertyName</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">buildingSociety</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">type</td>
<td valign="top"><a href="#json">JSON</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">ownershipType</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">peopleInHome</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">ownershipTiming</td>
<td valign="top"><a href="#json">JSON</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">apartmentNumber</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">otherProperties</td>
<td valign="top"><a href="#json">JSON</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createCard</strong></td>
<td valign="top"><a href="#card">Card</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">title</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">home</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">image</td>
<td valign="top"><a href="#uploadtype">UploadType</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">tags</td>
<td valign="top"><a href="#json">JSON</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createPion</strong></td>
<td valign="top"><a href="#pion">Pion</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">home</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">cards</td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">type</td>
<td valign="top"><a href="#piontypes">PionTypes</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">payload</td>
<td valign="top"><a href="#json">JSON</a></td>
<td>

"""
Pion payload per type:

          brand: {
            title       GraphQLString
            brand       GraphQLString
            model       GraphQLString
            productInfo GraphQLString
            serial      GraphQLString
            file        UploadType
          }

          note: {
            title       GraphQLString
            content     GraphQLString
            files       [UploadType]
          }

          url: {
            title       GraphQLString
            url         GraphQLString
            urlTitle    GraphQLString
            preview     GraphQLString
            favicon     GraphQLString
          }

          pdf: {
            title         GraphQLString
            documentName  GraphQLString
            file          UploadType
          }

          photo: {
            title       GraphQLString
            files       [UploadType]
          }

"""

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createTask</strong></td>
<td valign="top"><a href="#task">Task</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">homeId</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">cards</td>
<td valign="top"><a href="#json">JSON</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">payload</td>
<td valign="top"><a href="#json">JSON</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createTasksList</strong></td>
<td valign="top"><a href="#taskslist">TasksList</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">home</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">payload</td>
<td valign="top"><a href="#json">JSON</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updateCard</strong></td>
<td valign="top"><a href="#card">Card</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">title</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">home</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">image</td>
<td valign="top"><a href="#uploadtype">UploadType</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">tags</td>
<td valign="top"><a href="#json">JSON</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updateHome</strong></td>
<td valign="top"><a href="#home">Home</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">title</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">image</td>
<td valign="top"><a href="#uploadtype">UploadType</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">addressLine1</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">addressLine2</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">zipCode</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">city</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">lat</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">lon</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">language</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">country</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">countryISO</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">municipality</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">propertyName</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">buildingSociety</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">tags</td>
<td valign="top"><a href="#json">JSON</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">type</td>
<td valign="top"><a href="#json">JSON</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">ownershipType</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">peopleInHome</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">ownershipTiming</td>
<td valign="top"><a href="#json">JSON</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">apartmentNumber</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">otherProperties</td>
<td valign="top"><a href="#json">JSON</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">settings</td>
<td valign="top"><a href="#homesettingsinput">HomeSettingsInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">basicInfo</td>
<td valign="top"><a href="#homebasicinfoinput">HomeBasicInfoInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">property</td>
<td valign="top"><a href="#homepropertyinput">HomePropertyInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">buildingSocietyInfo</td>
<td valign="top"><a href="#homebuildingsocietyinfoinput">HomeBuildingSocietyInfoInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">roomsAndFloors</td>
<td valign="top"><a href="#homeroomsandfloorsinput">HomeRoomsAndFloorsInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">construction</td>
<td valign="top"><a href="#homeconstructioninput">HomeConstructionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">electricity</td>
<td valign="top"><a href="#homeelectricityinput">HomeElectricityInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">heatingAndCooling</td>
<td valign="top"><a href="#homeheatingandcoolinginput">HomeHeatingAndCoolingInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">waterAndSewer</td>
<td valign="top"><a href="#homewaterandsewerinput">HomeWaterAndSewerInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">securityAndInsurance</td>
<td valign="top"><a href="#homesecurityandinsuranceinput">HomeSecurityAndInsuranceInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">mortgage</td>
<td valign="top"><a href="#homemortgageinput">HomeMortgageInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">valuation</td>
<td valign="top">[<a href="#homevaluationinput">HomeValuationInput</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatePion</strong></td>
<td valign="top"><a href="#pion">Pion</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">cards</td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">payload</td>
<td valign="top"><a href="#json">JSON</a></td>
<td>

"""
Pion payload per type:

          brand: {
            title       GraphQLString
            brand       GraphQLString
            model       GraphQLString
            productInfo GraphQLString
            serial      GraphQLString
            file        UploadType
          }

          note: {
            title       GraphQLString
            content     GraphQLString
            files       [UploadType]
          }

          url: {
            title       GraphQLString
            url         GraphQLString
            urlTitle    GraphQLString
            preview     GraphQLString
            favicon     GraphQLString
          }

          pdf: {
            title         GraphQLString
            documentName  GraphQLString
            file          UploadType
          }

          photo: {
            title       GraphQLString
            files       [UploadType]
          }

"""

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updateTask</strong></td>
<td valign="top"><a href="#task">Task</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">homeId</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">cards</td>
<td valign="top"><a href="#json">JSON</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">payload</td>
<td valign="top"><a href="#json">JSON</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updateTasksList</strong></td>
<td valign="top"><a href="#taskslist">TasksList</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">home</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">payload</td>
<td valign="top"><a href="#json">JSON</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deleteHome</strong></td>
<td valign="top"><a href="#home">Home</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deleteCard</strong></td>
<td valign="top"><a href="#card">Card</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deleteFromHomeImages</strong></td>
<td valign="top"><a href="#home">Home</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">home</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">image</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deletePion</strong></td>
<td valign="top"><a href="#pion">Pion</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deleteTask</strong></td>
<td valign="top"><a href="#pion">Pion</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deleteTasksList</strong></td>
<td valign="top"><a href="#card">Card</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">deleteAllTasks</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>addUserToHome</strong></td>
<td valign="top"><a href="#home">Home</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">email</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>removeUserFromHome</strong></td>
<td valign="top"><a href="#home">Home</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">userId</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reorderHomeImages</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">homeId</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">imageIds</td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reorderTask</strong></td>
<td valign="top"><a href="#task">Task</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">insertAfter</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">tasksListId</td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
</tbody>
</table>

## Objects

### Authorization

An authorization result

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>accessToken</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Access token

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>accessTokenExpiresAt</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Access token expiration time

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refreshToken</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Refresh token

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refreshTokenExpiresAt</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Refresh token expiration time

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Scope of the token

</td>
</tr>
</tbody>
</table>

### BrandPion

Brand type of a pion

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#piontypes">PionTypes</a></td>
<td>

Pion type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cards</strong></td>
<td valign="top">[<a href="#card">Card</a>]</td>
<td>

Cards IDs, which cards this pion belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>home</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

Home ID, which home this pion belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

User ID, which user this pion belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>payload</strong></td>
<td valign="top"><a href="#json">JSON</a></td>
<td>

Fields related to the Pion, differs between types.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>title</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Title of the pion

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>brand</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Brand name of the brand

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>model</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The model of the brand

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>productInfo</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The info of the product

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>serial</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The serial number of the product

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>productPhoto</strong></td>
<td valign="top"><a href="#imagefile">ImageFile</a></td>
<td>

The product photo

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Created date

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Updated date

</td>
</tr>
</tbody>
</table>

### Card

A card

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>title</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Card title

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>subtitle</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Description of content inside card

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>home</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

Home ID, which home this card belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

User ID, which user this card belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Created date

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Updated date

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>placeholderImage</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The URL to placeholder image

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>image</strong></td>
<td valign="top"><a href="#imagefile">ImageFile</a></td>
<td>

Card image

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tags</strong></td>
<td valign="top">[<a href="#card">Card</a>]</td>
<td>

Tags of the card

</td>
</tr>
</tbody>
</table>

### Cards

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>items</strong></td>
<td valign="top">[<a href="#card">Card</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
</tbody>
</table>

### DateWithGranularity

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>date</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>granularity</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### Home

A home

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>title</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Home title

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Home type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>image</strong></td>
<td valign="top"><a href="#imagefile">ImageFile</a></td>
<td>

Home image

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>images</strong></td>
<td valign="top">[<a href="#imagefile">ImageFile</a>]</td>
<td>

Home images

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#user">User</a></td>
<td>

Home owner

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>users</strong></td>
<td valign="top">[<a href="#user">User</a>]</td>
<td>

Home users

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>language</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Language

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>addressLine1</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

addressLine1

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>addressLine2</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

addressLine2

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>zipCode</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

zipCode

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>city</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

city

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>country</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

country

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>countryISO</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

countryISO

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lat</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Latitude

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lon</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Longitude

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>municipality</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

municipality

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>municipalityDetails</strong></td>
<td valign="top"><a href="#json">JSON</a></td>
<td>

municipality details

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>apartmentNumber</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

apartmentNumber

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ownershipType</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

ownershipType

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ownershipTiming</strong></td>
<td valign="top"><a href="#json">JSON</a></td>
<td>

ownershipTiming

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>propertyName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

propertyName

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>peopleInHome</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

peopleInHome

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>buildingSociety</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

buildingSociety

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>settings</strong></td>
<td valign="top"><a href="#homesettings">HomeSettings</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>basicInfo</strong></td>
<td valign="top"><a href="#homebasicinfo">HomeBasicInfo</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>property</strong></td>
<td valign="top"><a href="#homeproperty">HomeProperty</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>buildingSocietyInfo</strong></td>
<td valign="top"><a href="#homebuildingsocietyinfo">HomeBuildingSocietyInfo</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>roomsAndFloors</strong></td>
<td valign="top"><a href="#homeroomsandfloors">HomeRoomsAndFloors</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>construction</strong></td>
<td valign="top"><a href="#homeconstruction">HomeConstruction</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>electricity</strong></td>
<td valign="top"><a href="#homeelectricity">HomeElectricity</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>heatingAndCooling</strong></td>
<td valign="top"><a href="#homeheatingandcooling">HomeHeatingAndCooling</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>waterAndSewer</strong></td>
<td valign="top"><a href="#homewaterandsewer">HomeWaterAndSewer</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>securityAndInsurance</strong></td>
<td valign="top"><a href="#homesecurityandinsurance">HomeSecurityAndInsurance</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mortgage</strong></td>
<td valign="top"><a href="#homemortgage">HomeMortgage</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>valuation</strong></td>
<td valign="top">[<a href="#homevaluation">HomeValuation</a>]</td>
<td></td>
</tr>
</tbody>
</table>

### HomeBasicInfo

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>homeType</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

home type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ownership</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Ownership type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>usage</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

home usage type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>partOfSociety</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Part of a society / community

</td>
</tr>
</tbody>
</table>

### HomeBuildingSocietyInfo

Home building society information

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>societyName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Society name

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>societyNumber</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Society number

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>societyURL</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Society website

</td>
</tr>
</tbody>
</table>

### HomeConstruction

Home construction

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constructionDate</strong></td>
<td valign="top"><a href="#datewithgranularity">DateWithGranularity</a></td>
<td>

Date of construction

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundation</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Foundation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundationAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Foundation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>frame</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Frame material

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>frameAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Frame material

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>facade</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Facade

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>facadeAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Facade

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>roofing</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roofing

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>roofingAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roofing

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>windowType</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Window type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>windowTypeAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Window type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ventilationType</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Ventilation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>byManufacturer</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Built by house manufacturer

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>company</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

House supplier

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>model</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

House model name

</td>
</tr>
</tbody>
</table>

### HomeElectricity

Home electricity

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>fuseSize</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Main fuse size

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>electricityCompany</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Electricity company

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>electricityCompanyAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Electricity company

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>electricityBoxID</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Box ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>electricityCustomerID</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Customer ID

</td>
</tr>
</tbody>
</table>

### HomeHeatingAndCooling

Home heating and cooling systems

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>heatingSystem</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Heating system

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>heatingSystemAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Heating system

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>heatPumpType</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Pump type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>boilerType</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Boiler type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stoveType</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Stove type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>coolingSystem</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Cooling system

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>coolingSystemAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Cooling system

</td>
</tr>
</tbody>
</table>

### HomeMortgage

Home mortgage info

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>mortgageCompany</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Mortgage provider

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mortgageCompanyAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Mortgage provider

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interestRate</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Interest rate

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refinancingDateUpcoming</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Upcoming refinacing date

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refinancingDateFollowing</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Following refinancing date

</td>
</tr>
</tbody>
</table>

### HomeProperty

Home Property

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>designation</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Property designation / Cadaster ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>plotSize</strong></td>
<td valign="top"><a href="#valuewithunit">ValueWithUnit</a></td>
<td>

Plot size

</td>
</tr>
</tbody>
</table>

### HomeRoomsAndFloors

Home rooms and floors

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>livingArea</strong></td>
<td valign="top"><a href="#valuewithunit">ValueWithUnit</a></td>
<td>

Living area

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ancillaryArea</strong></td>
<td valign="top"><a href="#valuewithunit">ValueWithUnit</a></td>
<td>

Ancillary area

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalArea</strong></td>
<td valign="top"><a href="#valuewithunit">ValueWithUnit</a></td>
<td>

Total area

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>floors</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Floors

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>basement</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Basement

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>attic</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Attic

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>bedrooms</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Bedrooms

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>bathrooms</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Bathrooms

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>separateWC</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Separate WC

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>otherRooms</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Other rooms (incl kitchen)

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalRooms</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Total rooms

</td>
</tr>
</tbody>
</table>

### HomeSecurityAndInsurance

Home security and insurance info

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>securityCompany</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Security company

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>securityCompanyAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Security company

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insuranceCompany</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Insurance company

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insuranceCompanyAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Insurance company

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insuranceCustomerID</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Insurance number

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insurancePackage</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Insurance package

</td>
</tr>
</tbody>
</table>

### HomeSettings

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>currency</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Used for display & receipt / cost calculation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>unit</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Units and measurments

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timeZone</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Will be used to time / send Push notifs

</td>
</tr>
</tbody>
</table>

### HomeValuation

Home valuation info

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>purchasePrice</strong></td>
<td valign="top"><a href="#valuewithunit">ValueWithUnit</a></td>
<td>

Purchase price

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>purchaseDate</strong></td>
<td valign="top"><a href="#datewithgranularity">DateWithGranularity</a></td>
<td>

Purchase date

</td>
</tr>
</tbody>
</table>

### HomeWaterAndSewer

Home home water and sewer systems

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>waterSource</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Water source

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>waterSourceAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Water source

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>waterSupplier</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Water supplier

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>waterHardness</strong></td>
<td valign="top"><a href="#valuewithunit">ValueWithUnit</a></td>
<td>

Water hardness

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sewage</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Sewage type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sewageAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Sewage type

</td>
</tr>
</tbody>
</table>

### ImageFile

An image file

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>home</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

Which home this file is related to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>size</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Size of file in bytes

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mime</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Mimetype of file (ex. image/jpeg)

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The filename it was uploaded as

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>payload</strong></td>
<td valign="top"><a href="#json">JSON</a></td>
<td>

Fields related to the File, differs between types.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>width</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Image width

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>height</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Image height

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>caption</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Caption for the image

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Description for the image

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Direct URL to the file.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tinyUrl</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Tiny thumbnail url

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>smallUrl</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Small thumbnail url

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mediumUrl</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Medium thumbnail url

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>largeUrl</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Large thumbnail url

</td>
</tr>
</tbody>
</table>

### NotePion

Note type of a pion

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#piontypes">PionTypes</a></td>
<td>

Pion type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cards</strong></td>
<td valign="top">[<a href="#card">Card</a>]</td>
<td>

Cards IDs, which cards this pion belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>home</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

Home ID, which home this pion belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

User ID, which user this pion belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdBy</strong></td>
<td valign="top"><a href="#user">User</a></td>
<td>

User which created the pion

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>payload</strong></td>
<td valign="top"><a href="#json">JSON</a></td>
<td>

Fields related to the Pion, differs between types.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>title</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Title of the note

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>content</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Content of the note

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>files</strong></td>
<td valign="top">[<a href="#imagefile">ImageFile</a>]</td>
<td>

Files of the content of the rich editor

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Created date

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Updated date

</td>
</tr>
</tbody>
</table>

### PDFFile

A PDF file

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>home</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

Which home this file is related to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>size</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Size of file in bytes

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mime</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Mimetype of file (ex. image/jpeg)

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The filename it was uploaded as

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>payload</strong></td>
<td valign="top"><a href="#json">JSON</a></td>
<td>

Fields related to the File, differs between types.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pages</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Number of pages

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Direct URL to the file.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tinyUrl</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Tiny thumbnail url

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>smallUrl</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Small thumbnail url

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mediumUrl</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Medium thumbnail url

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>largeUrl</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Large thumbnail url

</td>
</tr>
</tbody>
</table>

### PDFPion

PDF type of a pion

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#piontypes">PionTypes</a></td>
<td>

Pion type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cards</strong></td>
<td valign="top">[<a href="#card">Card</a>]</td>
<td>

Cards IDs, which cards this pion belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>home</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

Home ID, which home this pion belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

User ID, which user this pion belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>title</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Title

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>payload</strong></td>
<td valign="top"><a href="#json">JSON</a></td>
<td>

Fields related to the Pion, differs between types.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>file</strong></td>
<td valign="top"><a href="#pdffile">PDFFile</a></td>
<td>

The uploaded PDF

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>documentName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Source document name

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scanned</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Scanned flag

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Created date

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Updated date

</td>
</tr>
</tbody>
</table>

### PhotoPion

Photo type of a pion

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#piontypes">PionTypes</a></td>
<td>

Pion type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>title</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Title

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cards</strong></td>
<td valign="top">[<a href="#card">Card</a>]</td>
<td>

Cards IDs, which cards this pion belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>home</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

Home ID, which home this pion belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

User ID, which user this pion belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>payload</strong></td>
<td valign="top"><a href="#json">JSON</a></td>
<td>

Fields related to the Pion, differs between types.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>photos</strong></td>
<td valign="top">[<a href="#imagefile">ImageFile</a>]</td>
<td>

Photos related to the Pion

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Created date

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Updated date

</td>
</tr>
</tbody>
</table>

### Task

Task item

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>title</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

title

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Description of task

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#user">User</a></td>
<td>

Owner user of this task

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>home</strong></td>
<td valign="top"><a href="#home">Home</a></td>
<td>

Home ID, which home this task belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tasksList</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

Tasks list ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cards</strong></td>
<td valign="top">[<a href="#card">Card</a>]</td>
<td>

Array of cards

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>payload</strong></td>
<td valign="top"><a href="#json">JSON</a></td>
<td>

Fields related to the task, differs between types.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>order</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Order of task in the card

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prevTask</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

Previous task in the list of ones in the tasks list

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>done</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

State of task

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dueDate</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Due date

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>repeatInterval</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

CRON expression for repeat interval

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reminder</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

An option point of a reminder

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Created date

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Updated date

</td>
</tr>
</tbody>
</table>

### TasksList

A tasks list

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>title</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

title

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Description of the list

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>home</strong></td>
<td valign="top"><a href="#home">Home</a></td>
<td>

Home ID, which home this tasks list belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#user">User</a></td>
<td>

Owner user of this tasks list

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tasks</strong></td>
<td valign="top">[<a href="#task">Task</a>]</td>
<td>

List of the related tasks

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>color</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Color of the list

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>icon</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Icon of the list

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>image</strong></td>
<td valign="top"><a href="#imagefile">ImageFile</a></td>
<td>

Custom icon of the list

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>payload</strong></td>
<td valign="top"><a href="#json">JSON</a></td>
<td>

Fields related to the Pion, differs between types.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Created date

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Updated date

</td>
</tr>
</tbody>
</table>

### UrlPion

URL type of a pion

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#piontypes">PionTypes</a></td>
<td>

Pion type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cards</strong></td>
<td valign="top">[<a href="#card">Card</a>]</td>
<td>

Cards IDs, which cards this pion belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>home</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

Home ID, which home this pion belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

User ID, which user this pion belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>payload</strong></td>
<td valign="top"><a href="#json">JSON</a></td>
<td>

Fields related to the Pion, differs between types.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Full URL

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>title</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Title for the pion

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlTitle</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Title of the URL destination

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>preview</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

URL to the preview image (OG)

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>favicon</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

URL to the favicon

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Created date

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Updated date

</td>
</tr>
</tbody>
</table>

### User

A user

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>role</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

User role

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>firstName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Firstname

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Lastname

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

E-mail

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>image</strong></td>
<td valign="top"><a href="#imagefile">ImageFile</a></td>
<td>

User's image

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>language</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Language

</td>
</tr>
</tbody>
</table>

### ValueWithUnit

Value with unit

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Value

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>unit</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Unit of value

</td>
</tr>
</tbody>
</table>

## Inputs

### DateWithGranularityInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>date</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>granularity</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### HomeBasicInfoInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>homeType</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

home type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ownership</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Ownership type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>usage</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

home usage type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>partOfSociety</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Part of a society / community

</td>
</tr>
</tbody>
</table>

### HomeBuildingSocietyInfoInput

Home building society information

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>societyName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Society name

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>societyNumber</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Society number

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>societyURL</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Society website

</td>
</tr>
</tbody>
</table>

### HomeConstructionInput

Home construction

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constructionDate</strong></td>
<td valign="top"><a href="#datewithgranularityinput">DateWithGranularityInput</a></td>
<td>

Date of construction

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundation</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Foundation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundationAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Foundation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>frame</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Frame material

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>frameAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Frame material

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>facade</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Facade

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>facadeAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Facade

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>roofing</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roofing

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>roofingAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roofing

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>windowType</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Window type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>windowTypeAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Window type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ventilationType</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Ventilation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>byManufacturer</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Built by house manufacturer

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>company</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

House supplier

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>model</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

House model name

</td>
</tr>
</tbody>
</table>

### HomeElectricityInput

Home electricity

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>fuseSize</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Main fuse size

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>electricityCompany</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Electricity company

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>electricityCompanyAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Electricity company

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>electricityBoxID</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Box ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>electricityCustomerID</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Customer ID

</td>
</tr>
</tbody>
</table>

### HomeHeatingAndCoolingInput

Home heating and cooling systems

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>heatingSystem</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Heating system

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>heatingSystemAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Heating system

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>heatPumpType</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Pump type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>boilerType</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Boiler type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stoveType</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Stove type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>coolingSystem</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Cooling system

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>coolingSystemAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Cooling system

</td>
</tr>
</tbody>
</table>

### HomeMortgageInput

Home mortgage info

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>mortgageCompany</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Mortgage provider

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mortgageCompanyAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Mortgage provider

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interestRate</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Interest rate

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refinancingDateUpcoming</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Upcoming refinacing date

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refinancingDateFollowing</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Following refinancing date

</td>
</tr>
</tbody>
</table>

### HomePropertyInput

Home Property

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>designation</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Property designation / Cadaster ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>plotSize</strong></td>
<td valign="top"><a href="#valuewithunitinput">ValueWithUnitInput</a></td>
<td>

Plot size

</td>
</tr>
</tbody>
</table>

### HomeRoomsAndFloorsInput

Home rooms and floors

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>livingArea</strong></td>
<td valign="top"><a href="#valuewithunitinput">ValueWithUnitInput</a></td>
<td>

Living area

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ancillaryArea</strong></td>
<td valign="top"><a href="#valuewithunitinput">ValueWithUnitInput</a></td>
<td>

Ancillary area

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalArea</strong></td>
<td valign="top"><a href="#valuewithunitinput">ValueWithUnitInput</a></td>
<td>

Total area

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>floors</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Floors

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>basement</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Basement

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>attic</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Attic

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>bedrooms</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Bedrooms

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>bathrooms</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Bathrooms

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>separateWC</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Separate WC

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>otherRooms</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Other rooms (incl kitchen)

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalRooms</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Total rooms

</td>
</tr>
</tbody>
</table>

### HomeSecurityAndInsuranceInput

Home security and insurance info

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>securityCompany</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Security company

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>securityCompanyAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Security company

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insuranceCompany</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Insurance company

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insuranceCompanyAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Insurance company

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insuranceCustomerID</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Insurance number

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insurancePackage</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Insurance package

</td>
</tr>
</tbody>
</table>

### HomeSettingsInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>currency</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Used for display & receipt / cost calculation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>unit</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Units and measurments

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timeZone</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Will be used to time / send Push notifs

</td>
</tr>
</tbody>
</table>

### HomeValuationInput

Home valuation info

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>purchasePrice</strong></td>
<td valign="top"><a href="#valuewithunitinput">ValueWithUnitInput</a></td>
<td>

Purchase price

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>purchaseDate</strong></td>
<td valign="top"><a href="#datewithgranularityinput">DateWithGranularityInput</a></td>
<td>

Purchase date

</td>
</tr>
</tbody>
</table>

### HomeWaterAndSewerInput

Home home water and sewer systems

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>waterSource</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Water source

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>waterSourceAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Water source

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>waterSupplier</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Water supplier

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>waterHardness</strong></td>
<td valign="top"><a href="#valuewithunitinput">ValueWithUnitInput</a></td>
<td>

Water hardness

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sewage</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Sewage type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sewageAdditionalText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Sewage type

</td>
</tr>
</tbody>
</table>

### UploadType

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Name of upload

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Type of upload

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>size</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Size of file

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>path</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Path of file

</td>
</tr>
</tbody>
</table>

### ValueWithUnitInput

Value with unit

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Value

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>unit</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Unit of value

</td>
</tr>
</tbody>
</table>

## Enums

### PionTypes

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>note</strong></td>
<td>

A Pion of type Note

</td>
</tr>
<tr>
<td valign="top"><strong>brand</strong></td>
<td>

A Pion of type Brand

</td>
</tr>
<tr>
<td valign="top"><strong>photo</strong></td>
<td>

A Pion of type Photo

</td>
</tr>
<tr>
<td valign="top"><strong>url</strong></td>
<td>

A Pion of type URL

</td>
</tr>
<tr>
<td valign="top"><strong>pdf</strong></td>
<td>

A pion containing a PDF

</td>
</tr>
</tbody>
</table>

## Scalars

### Boolean

The `Boolean` scalar type represents `true` or `false`.

### DateTime

A date-time string at UTC, such as 2007-12-03T10:15:30Z, compliant with the `date-time` format outlined in section 5.6 of the RFC 3339 profile of the ISO 8601 standard for representation of dates and times using the Gregorian calendar.

### Float

The `Float` scalar type represents signed double-precision fractional values as specified by [IEEE 754](https://en.wikipedia.org/wiki/IEEE_floating_point).

### ID

The `ID` scalar type represents a unique identifier, often used to refetch an object or as key for a cache. The ID type appears in a JSON response as a String; however, it is not intended to be human-readable. When expected as an input type, any string (such as `"4"`) or integer (such as `4`) input value will be accepted as an ID.

### Int

The `Int` scalar type represents non-fractional signed whole numeric values. Int can represent values between -(2^31) and 2^31 - 1.

### JSON

The `JSON` scalar type represents JSON values as specified by [ECMA-404](http://www.ecma-international.org/publications/files/ECMA-ST/ECMA-404.pdf).

### String

The `String` scalar type represents textual data, represented as UTF-8 character sequences. The String type is most often used by GraphQL to represent free-form human-readable text.


## Interfaces


### File

A file

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>home</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

Which home this file is related to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>size</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Size of file in bytes

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mime</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Mimetype of file (ex. image/jpeg)

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The filename it was uploaded as

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>payload</strong></td>
<td valign="top"><a href="#json">JSON</a></td>
<td>

Fields related to the File, differs between types.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Direct URL to the file.

</td>
</tr>
</tbody>
</table>

### Pion

Piece of Information type

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#piontypes">PionTypes</a></td>
<td>

Pion type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cards</strong></td>
<td valign="top">[<a href="#card">Card</a>]</td>
<td>

Cards IDs, which cards this pion belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>home</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

Home ID, which home this pion belongs to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

Which user created the pion

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>payload</strong></td>
<td valign="top"><a href="#json">JSON</a></td>
<td>

Fields related to the Pion, differs between types.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Created date

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Updated date

</td>
</tr>
</tbody>
</table>
Done in 0.44s.
