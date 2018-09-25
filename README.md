# Schema Types

<details>
  <summary><strong>Table of Contents</strong></summary>

  * [Query](#query)
  * [Mutation](#mutation)
  * [Objects](#objects)
    * [Action](#action)
    * [AllocationGroup](#allocationgroup)
    * [AllocationGroupConnection](#allocationgroupconnection)
    * [AllocationGroupPageInfo](#allocationgrouppageinfo)
    * [Artist](#artist)
    * [ArtistConnection](#artistconnection)
    * [ArtistPageInfo](#artistpageinfo)
    * [Category](#category)
    * [CategoryConnection](#categoryconnection)
    * [CategoryPageInfo](#categorypageinfo)
    * [ChannelFee](#channelfee)
    * [Client](#client)
    * [ClientConnection](#clientconnection)
    * [ClientEventGuestCheckoutSettings](#clienteventguestcheckoutsettings)
    * [ClientEventImageSettings](#clienteventimagesettings)
    * [ClientEventSettings](#clienteventsettings)
    * [ClientLoadingFlag](#clientloadingflag)
    * [ClientPageInfo](#clientpageinfo)
    * [ClientRelationshipManager](#clientrelationshipmanager)
    * [Country](#country)
    * [CountryConnection](#countryconnection)
    * [CountryPageInfo](#countrypageinfo)
    * [Customer](#customer)
    * [CustomerAddress](#customeraddress)
    * [CustomerServiceResponse](#customerserviceresponse)
    * [DistanceFrom](#distancefrom)
    * [EmailAddress](#emailaddress)
    * [EmailAddressConnection](#emailaddressconnection)
    * [EmailAddressPageInfo](#emailaddresspageinfo)
    * [Event](#event)
    * [EventConnection](#eventconnection)
    * [EventImage](#eventimage)
    * [EventImageConnection](#eventimageconnection)
    * [EventImagePageInfo](#eventimagepageinfo)
    * [EventImageVersion](#eventimageversion)
    * [EventImageVersionConnection](#eventimageversionconnection)
    * [EventImageVersionPageInfo](#eventimageversionpageinfo)
    * [EventPageInfo](#eventpageinfo)
    * [EventReportSettings](#eventreportsettings)
    * [FacebookPsid](#facebookpsid)
    * [FeatureToggle](#featuretoggle)
    * [Fee](#fee)
    * [FeeTotal](#feetotal)
    * [Feedback](#feedback)
    * [FeedbackConnection](#feedbackconnection)
    * [FeedbackPageInfo](#feedbackpageinfo)
    * [Genre](#genre)
    * [GenreConnection](#genreconnection)
    * [GenrePageInfo](#genrepageinfo)
    * [ImageDimension](#imagedimension)
    * [MenuItem](#menuitem)
    * [MenuItemConnection](#menuitemconnection)
    * [MenuItemPageInfo](#menuitempageinfo)
    * [MultipleChoiceOption](#multiplechoiceoption)
    * [MultipleChoiceOptionConnection](#multiplechoiceoptionconnection)
    * [MultipleChoiceOptionPageInfo](#multiplechoiceoptionpageinfo)
    * [MutationViewer](#mutationviewer)
    * [OfferCode](#offercode)
    * [OfferCodeConnection](#offercodeconnection)
    * [OfferCodePageInfo](#offercodepageinfo)
    * [Order](#order)
    * [OrderConnection](#orderconnection)
    * [OrderFee](#orderfee)
    * [OrderPageInfo](#orderpageinfo)
    * [QueryViewer](#queryviewer)
    * [Question](#question)
    * [QuestionConnection](#questionconnection)
    * [QuestionPageInfo](#questionpageinfo)
    * [Region](#region)
    * [RegionConnection](#regionconnection)
    * [RegionPageInfo](#regionpageinfo)
    * [Skin](#skin)
    * [SkinConnection](#skinconnection)
    * [SkinPageInfo](#skinpageinfo)
    * [Tag](#tag)
    * [TagConnection](#tagconnection)
    * [TagPageInfo](#tagpageinfo)
    * [Ticket](#ticket)
    * [TicketConnection](#ticketconnection)
    * [TicketPageInfo](#ticketpageinfo)
    * [TicketType](#tickettype)
    * [TicketTypeConnection](#tickettypeconnection)
    * [TicketTypePageInfo](#tickettypepageinfo)
    * [TicketTypeSaleChannel](#tickettypesalechannel)
    * [User](#user)
    * [UserAction](#useraction)
    * [UserActionConnection](#useractionconnection)
    * [UserActionPageInfo](#useractionpageinfo)
    * [UserConnection](#userconnection)
    * [UserPageInfo](#userpageinfo)
    * [Venue](#venue)
    * [VenueAddress](#venueaddress)
    * [VenueConnection](#venueconnection)
    * [VenueLocation](#venuelocation)
    * [VenuePageInfo](#venuepageinfo)
    * [Viewer](#viewer)
    * [ViewerFeatureToggle](#viewerfeaturetoggle)
    * [ViewerFeatureToggleConnection](#viewerfeaturetoggleconnection)
    * [ViewerFeatureTogglePageInfo](#viewerfeaturetogglepageinfo)
    * [ViewerRole](#viewerrole)
    * [ViewerRoleConnection](#viewerroleconnection)
    * [ViewerRolePageInfo](#viewerrolepageinfo)
    * [Webhook](#webhook)
    * [WebhookConnection](#webhookconnection)
    * [WebhookHeader](#webhookheader)
    * [WebhookHeaderConnection](#webhookheaderconnection)
    * [WebhookHeaderPageInfo](#webhookheaderpageinfo)
    * [WebhookPageInfo](#webhookpageinfo)
    * [WebhookSystemEventType](#webhooksystemeventtype)
    * [WebhookSystemEventTypeConnection](#webhooksystemeventtypeconnection)
    * [WebhookSystemEventTypePageInfo](#webhooksystemeventtypepageinfo)
    * [fileUploadCredentials](#fileuploadcredentials)
    * [fileUploadLinkType](#fileuploadlinktype)
  * [Enums](#enums)
    * [AgeRestriction](#agerestriction)
    * [AgeRestrictionInput](#agerestrictioninput)
    * [ArtistSortOptionsInput](#artistsortoptionsinput)
    * [ClientSortOptionsInput](#clientsortoptionsinput)
    * [CountrySortOptionsInput](#countrysortoptionsinput)
    * [EventSortOptionsInput](#eventsortoptionsinput)
    * [FeedbackContext](#feedbackcontext)
    * [FeedbackContextInput](#feedbackcontextinput)
    * [FeedbackSortOptionsInput](#feedbacksortoptionsinput)
    * [FileUploadPurposeInput](#fileuploadpurposeinput)
    * [Gender](#gender)
    * [GenderInput](#genderinput)
    * [OfferCodeSortOptionsInput](#offercodesortoptionsinput)
    * [OrderChannel](#orderchannel)
    * [OrderChannelInput](#orderchannelinput)
    * [OrderSortOptionsInput](#ordersortoptionsinput)
    * [SaleChannelInput](#salechannelinput)
    * [SkinSortOptionsInput](#skinsortoptionsinput)
    * [SortByDirectionInput](#sortbydirectioninput)
    * [StatusOptions](#statusoptions)
    * [StatusOptionsInput](#statusoptionsinput)
    * [SystemEventType](#systemeventtype)
    * [SystemEventTypeInput](#systemeventtypeinput)
    * [TicketSortOptionsInput](#ticketsortoptionsinput)
    * [TicketTypeSortOptionsInput](#tickettypesortoptionsinput)
    * [UserStatus](#userstatus)
    * [UserStatusInput](#userstatusinput)
    * [VenuesSortOptionsInput](#venuessortoptionsinput)
    * [userSortByOptionsInput](#usersortbyoptionsinput)
  * [Scalars](#scalars)
    * [Boolean](#boolean)
    * [Date](#date)
    * [Float](#float)
    * [Int](#int)
    * [String](#string)

</details>

## Query 
All queries can be found here (queries are used to read data from the API). Click QueryViewer link below to see a list of all available queries.

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
<td colspan="2" valign="top"><strong>viewer</strong></td>
<td valign="top"><a href="#queryviewer">QueryViewer</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">token</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

## Mutation 
All mutations can be found here (mutations are used to change (mutate) data using the API). Click MutationViewer link below to see a list of all available mutations.

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
<td colspan="2" valign="top"><strong>login</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">username</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">password</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">programmaticAccess</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewer</strong></td>
<td valign="top"><a href="#mutationviewer">MutationViewer</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">token</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

## Objects

### Action

A type of action that can be performed by the user

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### AllocationGroup

Allocation group

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>remaining</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
</tbody>
</table>

### AllocationGroupConnection

Connection for AllocationGroup

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
<td valign="top">[<a href="#allocationgroup">AllocationGroup</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#allocationgrouppageinfo">AllocationGroupPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### AllocationGroupPageInfo

Page information for AllocationGroup

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### Artist

Artist type

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>remove</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.admin.

</td>
</tr>
</tbody>
</table>

### ArtistConnection

Connection for Artist

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
<td valign="top">[<a href="#artist">Artist</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#artistpageinfo">ArtistPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### ArtistPageInfo

Page information for Artist

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### Category

Category

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>genres</strong></td>
<td valign="top"><a href="#genreconnection">GenreConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### CategoryConnection

Connection for Category

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
<td valign="top">[<a href="#category">Category</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#categorypageinfo">CategoryPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### CategoryPageInfo

Page information for Category

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### ChannelFee

Fees applied per sale channel

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
<td colspan="2" valign="top"><strong>retailFee</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>phoneFee</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>boxOfficeFee</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Not yet supported. Roles: mosh.admin.

</td>
</tr>
</tbody>
</table>

### Client

Client

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>phone</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>encryptedId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.admin, client.any.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>clientRelationshipManager</strong></td>
<td valign="top"><a href="#clientrelationshipmanager">ClientRelationshipManager</a></td>
<td>

Roles: client.any.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>eventSettings</strong></td>
<td valign="top"><a href="#clienteventsettings">ClientEventSettings</a></td>
<td>

Roles: client.any.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">clientId</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>remove</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>users</strong></td>
<td valign="top"><a href="#userconnection">UserConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortBy</td>
<td valign="top"><a href="#usersortbyoptionsinput">userSortByOptionsInput</a></td>
<td></td>
</tr>
</tbody>
</table>

### ClientConnection

Connection for Client

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
<td valign="top">[<a href="#client">Client</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#clientpageinfo">ClientPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### ClientEventGuestCheckoutSettings

Client guest checkout settings

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
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>enabled</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.any.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>allowControl</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.any.

</td>
</tr>
</tbody>
</table>

### ClientEventImageSettings

Client Event Build Image Settings

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
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>enabled</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.any.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dimensions</strong></td>
<td valign="top"><a href="#imagedimension">ImageDimension</a></td>
<td>

Roles: client.any.

</td>
</tr>
</tbody>
</table>

### ClientEventSettings

Client Event Build Settings

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
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customImage</strong></td>
<td valign="top"><a href="#clienteventimagesettings">ClientEventImageSettings</a></td>
<td>

Roles: client.any.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>guestCheckout</strong></td>
<td valign="top"><a href="#clienteventguestcheckoutsettings">ClientEventGuestCheckoutSettings</a></td>
<td>

Roles: client.any.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>clientLoading</strong></td>
<td valign="top"><a href="#clientloadingflag">ClientLoadingFlag</a></td>
<td>

Describes which sale channel the rebate/client loading fee is available for. Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sendReminderEmailDaysAhead</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: client.any.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sendReminderEmail</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.any.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>autoSettle</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.any.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processingFee</strong></td>
<td valign="top"><a href="#orderfee">OrderFee</a></td>
<td>

Transaction fee applied to customer order. Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ticketFinePrint</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>purchasePolicy</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### ClientLoadingFlag

Client loading flag

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
<td colspan="2" valign="top"><strong>online</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Flag to indicate if a fee is applied to the total order value when purchasing ticket online. Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>phone</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Flag to indicate if a fee is applied to the total order value when purchasing ticket via customer services over the phone. Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>retail</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Flag to indicate if a fee is applied to the total order value when purchasing via a Retail outlet. Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>boxOffice</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Flag to indicate if a fee is applied to the total order value when purchasing via the Box Office. Roles: everyone.

</td>
</tr>
</tbody>
</table>

### ClientPageInfo

Page information for Client

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### ClientRelationshipManager

A person who manages a client account

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
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.any, client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>firstName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.any, client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.any, client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>phone</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.any, client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.any, client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.any, client.admin.

</td>
</tr>
</tbody>
</table>

### Country

Country

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
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>regions</strong></td>
<td valign="top"><a href="#regionconnection">RegionConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### CountryConnection

Connection for Country

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
<td valign="top">[<a href="#country">Country</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#countrypageinfo">CountryPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### CountryPageInfo

Page information for Country

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### Customer

Customer

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>firstName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address</strong></td>
<td valign="top"><a href="#customeraddress">CustomerAddress</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender</strong></td>
<td valign="top"><a href="#gender">Gender</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>telephone</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobile</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>birthDate</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>guest</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### CustomerAddress

Customer Address

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
<td colspan="2" valign="top"><strong>postcode</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
</tbody>
</table>

### CustomerServiceResponse

Response to a particular topic

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client</strong></td>
<td valign="top"><a href="#client">Client</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">clientId</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>response</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### DistanceFrom

Distance from location

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
<td colspan="2" valign="top"><strong>distance</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fromLatitude</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fromLongitude</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### EmailAddress

Email address

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
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>remove</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.admin.

</td>
</tr>
</tbody>
</table>

### EmailAddressConnection

Connection for EmailAddress

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
<td valign="top">[<a href="#emailaddress">EmailAddress</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#emailaddresspageinfo">EmailAddressPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### EmailAddressPageInfo

Page information for EmailAddress

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### Event

Event

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
<td colspan="2" valign="top"><strong>approved</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>previewId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>teaser</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>presenter</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>announcementDate</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>startDate</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>endDate</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>addressRequired</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sellingTickets</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>guestCheckout</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>autoSettle</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Auto settlement for event. Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>distance</strong></td>
<td valign="top"><a href="#distancefrom">DistanceFrom</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxTicketsPerOrder</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxTicketsPerCustomer</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ticketsRequireAttendeeName</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ticketsRequireAttendeeDob</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>waitlist</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>waitlistDisplayAlways</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>collectAttendeeData</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>allowPayByInstallment</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reissueFee</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ticketFinePrint</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>purchasePolicy</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useLatestEditor</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sendReminderEmail</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sendReminderEmailDaysAhead</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ageRestriction</strong></td>
<td valign="top"><a href="#agerestriction">AgeRestriction</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>published</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchable</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdDate</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>images</strong></td>
<td valign="top"><a href="#eventimageconnection">EventImageConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>remove</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>venue</strong></td>
<td valign="top"><a href="#venue">Venue</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>artists</strong></td>
<td valign="top"><a href="#artistconnection">ArtistConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ticketTypes</strong></td>
<td valign="top"><a href="#tickettypeconnection">TicketTypeConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">searchTerm</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortBy</td>
<td valign="top"><a href="#tickettypesortoptionsinput">TicketTypeSortOptionsInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>offerCodes</strong></td>
<td valign="top"><a href="#offercodeconnection">OfferCodeConnection</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">searchTerm</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortBy</td>
<td valign="top"><a href="#offercodesortoptionsinput">OfferCodeSortOptionsInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>questions</strong></td>
<td valign="top"><a href="#questionconnection">QuestionConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tags</strong></td>
<td valign="top"><a href="#tagconnection">TagConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>allocationGroups</strong></td>
<td valign="top"><a href="#allocationgroupconnection">AllocationGroupConnection</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client</strong></td>
<td valign="top"><a href="#client">Client</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportSettings</strong></td>
<td valign="top"><a href="#eventreportsettings">EventReportSettings</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processingFee</strong></td>
<td valign="top"><a href="#orderfee">OrderFee</a></td>
<td>

Transaction fee applied to customer order. Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>includeFeesInPrice</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Flag to indicate if a fee is displayed to customers or included in the ticket price. Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>clientLoading</strong></td>
<td valign="top"><a href="#clientloadingflag">ClientLoadingFlag</a></td>
<td>

Describes which sale channel the rebate/client loading fee is available for. Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>category</strong></td>
<td valign="top"><a href="#category">Category</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>genre</strong></td>
<td valign="top"><a href="#genre">Genre</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### EventConnection

Connection for Event

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
<td valign="top">[<a href="#event">Event</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#eventpageinfo">EventPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### EventImage

Event Image

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dimensions</strong></td>
<td valign="top"><a href="#imagedimension">ImageDimension</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uploadKey</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>remove</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>versions</strong></td>
<td valign="top"><a href="#eventimageversionconnection">EventImageVersionConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### EventImageConnection

Connection for EventImage

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
<td valign="top">[<a href="#eventimage">EventImage</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#eventimagepageinfo">EventImagePageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### EventImagePageInfo

Page information for EventImage

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### EventImageVersion

image version

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
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dimensions</strong></td>
<td valign="top"><a href="#imagedimension">ImageDimension</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### EventImageVersionConnection

Connection for EventImageVersion

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
<td valign="top">[<a href="#eventimageversion">EventImageVersion</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#eventimageversionpageinfo">EventImageVersionPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### EventImageVersionPageInfo

Page information for EventImageVersion

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### EventPageInfo

Page information for Event

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### EventReportSettings

Event Report Settings

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
<td colspan="2" valign="top"><strong>eventId</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sendDaily</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sendWeekly</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sendEndOfEvent</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sendSalesClose</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>doorListRecipientEmails</strong></td>
<td valign="top"><a href="#emailaddressconnection">EmailAddressConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>salesReportRecipientEmails</strong></td>
<td valign="top"><a href="#emailaddressconnection">EmailAddressConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>clientsWithReportingAccess</strong></td>
<td valign="top"><a href="#artistconnection">ArtistConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### FacebookPsid

Customer to Facebook PSID mapping

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customer</strong></td>
<td valign="top"><a href="#customer">Customer</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>psid</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
</tbody>
</table>

### FeatureToggle

A feature that can be toggled on or off

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### Fee

Fee

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
<td colspan="2" valign="top"><strong>additionalChannelFees</strong></td>
<td valign="top"><a href="#channelfee">ChannelFee</a></td>
<td>

Fee applied based on sale channel used when selling ticket.. Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>moshtixFee</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Moshtix fee. Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>clientFee</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Client fee. Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processingPercentage</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Percentage amount applied. Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processingFee</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ticketCost</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Ticket cost charged at settlement regardless of sale channel.. Roles: mosh.admin.

</td>
</tr>
</tbody>
</table>

### FeeTotal

Total fee amount for ticket price

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
<td colspan="2" valign="top"><strong>feeTotal</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>basePrice</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ticketPrice</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fee</strong></td>
<td valign="top"><a href="#fee">Fee</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
</tbody>
</table>

### Feedback

Feedback

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdDate</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>user</strong></td>
<td valign="top"><a href="#user">User</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>context</strong></td>
<td valign="top"><a href="#feedbackcontext">FeedbackContext</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>message</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
</tbody>
</table>

### FeedbackConnection

Connection for Feedback

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
<td valign="top">[<a href="#feedback">Feedback</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#feedbackpageinfo">FeedbackPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### FeedbackPageInfo

Page information for Feedback

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### Genre

Genre

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### GenreConnection

Connection for Genre

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
<td valign="top">[<a href="#genre">Genre</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#genrepageinfo">GenrePageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### GenrePageInfo

Page information for Genre

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### ImageDimension

Image Dimensions

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
<td colspan="2" valign="top"><strong>width</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>height</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### MenuItem

Menu item

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
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>icon</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>roles</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>children</strong></td>
<td valign="top"><a href="#menuitemconnection">MenuItemConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### MenuItemConnection

Connection for MenuItem

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
<td valign="top">[<a href="#menuitem">MenuItem</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#menuitempageinfo">MenuItemPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### MenuItemPageInfo

Page information for MenuItem

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### MultipleChoiceOption

Multiple Choice Option

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>option</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### MultipleChoiceOptionConnection

Connection for MultipleChoiceOption

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
<td valign="top">[<a href="#multiplechoiceoption">MultipleChoiceOption</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#multiplechoiceoptionpageinfo">MultipleChoiceOptionPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### MultipleChoiceOptionPageInfo

Page information for MultipleChoiceOption

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### MutationViewer

Root level object to include identification information for authentication

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
<td colspan="2" valign="top"><strong>saveArtist</strong></td>
<td valign="top"><a href="#artist">Artist</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">artist</td>
<td valign="top"><a href="#artistinput">ArtistInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>saveEvent</strong></td>
<td valign="top"><a href="#event">Event</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">event</td>
<td valign="top"><a href="#eventinput">EventInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>saveFacebookPsid</strong></td>
<td valign="top"><a href="#facebookpsid">FacebookPsid</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">facebookPsid</td>
<td valign="top"><a href="#facebookpsidinput">FacebookPsidInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>saveFeedback</strong></td>
<td valign="top"><a href="#feedback">Feedback</a></td>
<td>

Roles: authenticated.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">feedback</td>
<td valign="top"><a href="#feedbackinput">FeedbackInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>saveUserAction</strong></td>
<td valign="top"><a href="#useraction">UserAction</a></td>
<td>

Roles: authenticated.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">userAction</td>
<td valign="top"><a href="#useractioninput">UserActionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>saveOrder</strong></td>
<td valign="top"><a href="#order">Order</a></td>
<td>

Roles: authenticated.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order</td>
<td valign="top"><a href="#orderinput">OrderInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>saveWebhook</strong></td>
<td valign="top"><a href="#webhook">Webhook</a></td>
<td>

Roles: client.admin.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">webhook</td>
<td valign="top"><a href="#webhookinput">WebhookInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generateFileUploadLink</strong></td>
<td valign="top"><a href="#fileuploadlinktype">fileUploadLinkType</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">clientId</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">contentType</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generateFileUploadCredentials</strong></td>
<td valign="top"><a href="#fileuploadcredentials">fileUploadCredentials</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">clientId</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">purpose</td>
<td valign="top"><a href="#fileuploadpurposeinput">FileUploadPurposeInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>saveClient</strong></td>
<td valign="top"><a href="#client">Client</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">client</td>
<td valign="top"><a href="#clientinput">ClientInput</a></td>
<td></td>
</tr>
</tbody>
</table>

### OfferCode

Offer Code

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>offerStartDate</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>offerEndDate</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>revealHiddenTicket</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>allowEarlyPurchase</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maximumAllocation</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ticketTypes</strong></td>
<td valign="top"><a href="#tickettypeconnection">TicketTypeConnection</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortBy</td>
<td valign="top"><a href="#tickettypesortoptionsinput">TicketTypeSortOptionsInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>discountAmount</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
</tbody>
</table>

### OfferCodeConnection

Connection for OfferCode

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
<td valign="top">[<a href="#offercode">OfferCode</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#offercodepageinfo">OfferCodePageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### OfferCodePageInfo

Page information for OfferCode

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### Order

Order

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>channel</strong></td>
<td valign="top"><a href="#orderchannel">OrderChannel</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customer</strong></td>
<td valign="top"><a href="#customer">Customer</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tickets</strong></td>
<td valign="top"><a href="#ticketconnection">TicketConnection</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortBy</td>
<td valign="top"><a href="#ticketsortoptionsinput">TicketSortOptionsInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event</strong></td>
<td valign="top"><a href="#event">Event</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### OrderConnection

Connection for Order

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
<td valign="top">[<a href="#order">Order</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#orderpageinfo">OrderPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### OrderFee

Order Fee

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
<td colspan="2" valign="top"><strong>enabled</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Flag to indicate if a fee is applied to the total order value. Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Fee name. Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Fee amount. Roles: mosh.admin.

</td>
</tr>
</tbody>
</table>

### OrderPageInfo

Page information for Order

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### QueryViewer

Root level object to include identification information for authentication

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
<td colspan="2" valign="top"><strong>viewer</strong></td>
<td valign="top"><a href="#viewer">Viewer</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewerId</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Deprecated. Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewerUsername</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Deprecated. Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewerFirstName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Deprecated. Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewerLastName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Deprecated. Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewerToken</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Deprecated. Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewerRoles</strong></td>
<td valign="top">[<a href="#viewerrole">ViewerRole</a>]</td>
<td>

Deprecated. Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getClient</strong></td>
<td valign="top"><a href="#client">Client</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getClients</strong></td>
<td valign="top"><a href="#clientconnection">ClientConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">searchTerm</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortBy</td>
<td valign="top"><a href="#clientsortoptionsinput">ClientSortOptionsInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getEvents</strong></td>
<td valign="top"><a href="#eventconnection">EventConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">categoryIds</td>
<td valign="top">[<a href="#int">Int</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">clientIds</td>
<td valign="top">[<a href="#int">Int</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">eventStartDateFrom</td>
<td valign="top"><a href="#date">Date</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">eventStartDateTo</td>
<td valign="top"><a href="#date">Date</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">genreIds</td>
<td valign="top">[<a href="#int">Int</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">location</td>
<td valign="top"><a href="#eventlocationinput">EventLocationInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">publicOnly</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">searchableOnly</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">searchTerm</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortBy</td>
<td valign="top"><a href="#eventsortoptionsinput">EventSortOptionsInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">venueIds</td>
<td valign="top">[<a href="#int">Int</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">genreSearchTerm</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getEvent</strong></td>
<td valign="top"><a href="#event">Event</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getFeedbacks</strong></td>
<td valign="top"><a href="#feedbackconnection">FeedbackConnection</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortBy</td>
<td valign="top"><a href="#feedbacksortoptionsinput">FeedbackSortOptionsInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">createdDateFrom</td>
<td valign="top"><a href="#date">Date</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">createdDateTo</td>
<td valign="top"><a href="#date">Date</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getFeedback</strong></td>
<td valign="top"><a href="#feedback">Feedback</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getMenuItems</strong></td>
<td valign="top"><a href="#menuitemconnection">MenuItemConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">clientId</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getCategories</strong></td>
<td valign="top"><a href="#categoryconnection">CategoryConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getTicketType</strong></td>
<td valign="top"><a href="#tickettype">TicketType</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getTicketTypes</strong></td>
<td valign="top"><a href="#tickettypeconnection">TicketTypeConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">searchTerm</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortBy</td>
<td valign="top"><a href="#tickettypesortoptionsinput">TicketTypeSortOptionsInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">eventId</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offerCodeId</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">publicOnly</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getArtists</strong></td>
<td valign="top"><a href="#artistconnection">ArtistConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">searchTerm</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortBy</td>
<td valign="top"><a href="#artistsortoptionsinput">ArtistSortOptionsInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getArtist</strong></td>
<td valign="top"><a href="#artist">Artist</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getVenues</strong></td>
<td valign="top"><a href="#venueconnection">VenueConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">addressLookupFailed</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">locationDataAvailable</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">searchTerm</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortBy</td>
<td valign="top"><a href="#venuessortoptionsinput">VenuesSortOptionsInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getVenue</strong></td>
<td valign="top"><a href="#venue">Venue</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getCustomerServiceResponse</strong></td>
<td valign="top"><a href="#customerserviceresponse">CustomerServiceResponse</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">name</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">clientId</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getOrder</strong></td>
<td valign="top"><a href="#order">Order</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getOrders</strong></td>
<td valign="top"><a href="#orderconnection">OrderConnection</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortBy</td>
<td valign="top"><a href="#ordersortoptionsinput">OrderSortOptionsInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getTicket</strong></td>
<td valign="top"><a href="#ticket">Ticket</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getTicketPrice</strong></td>
<td valign="top"><a href="#feetotal">FeeTotal</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">clientId</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">price</td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">moshtixFee</td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">clientFee</td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">addOn</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">complimentary</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">saleChannel</td>
<td valign="top"><a href="#salechannelinput">SaleChannelInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">phoneFee</td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">retailFee</td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">boxOfficeFee</td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">ticketCost</td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getTicketFees</strong></td>
<td valign="top"><a href="#feetotal">FeeTotal</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">ticketPrice</td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">clientId</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getTickets</strong></td>
<td valign="top"><a href="#ticketconnection">TicketConnection</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortBy</td>
<td valign="top"><a href="#ticketsortoptionsinput">TicketSortOptionsInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getSkins</strong></td>
<td valign="top"><a href="#skinconnection">SkinConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">clientId</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortBy</td>
<td valign="top"><a href="#skinsortoptionsinput">SkinSortOptionsInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getCustomer</strong></td>
<td valign="top"><a href="#customer">Customer</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">email</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getCountries</strong></td>
<td valign="top"><a href="#countryconnection">CountryConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">searchTerm</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortBy</td>
<td valign="top"><a href="#countrysortoptionsinput">CountrySortOptionsInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getWebhooks</strong></td>
<td valign="top"><a href="#webhookconnection">WebhookConnection</a></td>
<td>

Roles: client.admin.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">clientId</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getWebhook</strong></td>
<td valign="top"><a href="#webhook">Webhook</a></td>
<td>

Roles: client.admin.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### Question

Question

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
<td colspan="2" valign="top"><strong>isMultipleChoice</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>question</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>options</strong></td>
<td valign="top"><a href="#multiplechoiceoptionconnection">MultipleChoiceOptionConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### QuestionConnection

Connection for Question

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
<td valign="top">[<a href="#question">Question</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#questionpageinfo">QuestionPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### QuestionPageInfo

Page information for Question

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### Region

Region

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### RegionConnection

Connection for Region

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
<td valign="top">[<a href="#region">Region</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#regionpageinfo">RegionPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### RegionPageInfo

Page information for Region

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### Skin

Skin type

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### SkinConnection

Connection for Skin

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
<td valign="top">[<a href="#skin">Skin</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#skinpageinfo">SkinPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### SkinPageInfo

Page information for Skin

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### Tag

Tag

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>remove</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.admin.

</td>
</tr>
</tbody>
</table>

### TagConnection

Connection for Tag

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
<td valign="top">[<a href="#tag">Tag</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#tagpageinfo">TagPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### TagPageInfo

Page information for Tag

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### Ticket

Ticket

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>firstName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdDate</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ticketType</strong></td>
<td valign="top"><a href="#tickettype">TicketType</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>order</strong></td>
<td valign="top"><a href="#order">Order</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client</strong></td>
<td valign="top"><a href="#client">Client</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event</strong></td>
<td valign="top"><a href="#event">Event</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>status</strong></td>
<td valign="top"><a href="#statusoptions">StatusOptions</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ticketNumber</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ticketDescription</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>barcode</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: mosh.admin, client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>unitCost</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>bookingFee</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
</tbody>
</table>

### TicketConnection

Connection for Ticket

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
<td valign="top">[<a href="#ticket">Ticket</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#ticketpageinfo">TicketPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### TicketPageInfo

Page information for Ticket

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### TicketType

Ticket type

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
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hidden</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>suppressDistribution</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>addOn</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>addOnAvailableSeparately</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>complimentary</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hard</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hardDisplayName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hardDisplayPrice</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>salesStartDate</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>salesCloseDate</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ticketPrice</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ticketOnlineFee</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Total online fee amount. Readonly. Roles: client.admin, client.editor, mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ticketOnlinePrice</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Total online price. Readonly. Roles: client.admin, client.editor, mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxPerOrder</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxPerCustomer</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minPerOrder</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>increment</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ticketOrdinal</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fees</strong></td>
<td valign="top"><a href="#fee">Fee</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>remove</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event</strong></td>
<td valign="top"><a href="#event">Event</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>allocationGroup</strong></td>
<td valign="top"><a href="#allocationgroup">AllocationGroup</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>saleChannels</strong></td>
<td valign="top"><a href="#tickettypesalechannel">TicketTypeSaleChannel</a></td>
<td>

Roles: client.admin, mosh.admin, client.editor.

</td>
</tr>
</tbody>
</table>

### TicketTypeConnection

Connection for TicketType

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
<td valign="top">[<a href="#tickettype">TicketType</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#tickettypepageinfo">TicketTypePageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### TicketTypePageInfo

Page information for TicketType

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### TicketTypeSaleChannel

Ticket type sale channel

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
<td colspan="2" valign="top"><strong>online</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>boxOffice</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>retail</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>phone</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### User

User

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>username</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>firstName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>salt</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>passwordHash</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isCustomer</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>allowProgrammaticAccess</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>status</strong></td>
<td valign="top"><a href="#userstatus">UserStatus</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>confirmationKey</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: mosh.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>roles</strong></td>
<td valign="top"><a href="#viewerroleconnection">ViewerRoleConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
</tbody>
</table>

### UserAction

A list of actions carried out be the current viewer.

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action</strong></td>
<td valign="top"><a href="#action">Action</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>date</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### UserActionConnection

Connection for UserAction

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
<td valign="top">[<a href="#useraction">UserAction</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#useractionpageinfo">UserActionPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### UserActionPageInfo

Page information for UserAction

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### UserConnection

Connection for User

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
<td valign="top">[<a href="#user">User</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#userpageinfo">UserPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### UserPageInfo

Page information for User

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### Venue

Venue

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
<td colspan="2" valign="top"><strong>address</strong></td>
<td valign="top"><a href="#venueaddress">VenueAddress</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>imageUrl</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>location</strong></td>
<td valign="top"><a href="#venuelocation">VenueLocation</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timeZoneOffsetFromUTC</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### VenueAddress

Venue Address

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
<td colspan="2" valign="top"><strong>country</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>locality</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>line1</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>line2</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postCode</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>region</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### VenueConnection

Connection for Venue

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
<td valign="top">[<a href="#venue">Venue</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#venuepageinfo">VenuePageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### VenueLocation

Venue Location

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
<td colspan="2" valign="top"><strong>latitude</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>longitude</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>addressLookupFailed</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

flag to identify if a latitude longitude value can be found for the address stored against the venue. Roles: mosh.admin.

</td>
</tr>
</tbody>
</table>

### VenuePageInfo

Page information for Venue

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### Viewer

A viewer

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>username</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>firstName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>token</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>roles</strong></td>
<td valign="top"><a href="#viewerroleconnection">ViewerRoleConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>featureToggles</strong></td>
<td valign="top"><a href="#viewerfeaturetoggleconnection">ViewerFeatureToggleConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>userActions</strong></td>
<td valign="top"><a href="#useractionconnection">UserActionConnection</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### ViewerFeatureToggle

A list of feature toggles for the current viewer.

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
<td colspan="2" valign="top"><strong>featureToggle</strong></td>
<td valign="top"><a href="#featuretoggle">FeatureToggle</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### ViewerFeatureToggleConnection

Connection for ViewerFeatureToggle

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
<td valign="top">[<a href="#viewerfeaturetoggle">ViewerFeatureToggle</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#viewerfeaturetogglepageinfo">ViewerFeatureTogglePageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### ViewerFeatureTogglePageInfo

Page information for ViewerFeatureToggle

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### ViewerRole

A viewer role

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
<td colspan="2" valign="top"><strong>clientId</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### ViewerRoleConnection

Connection for ViewerRole

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
<td valign="top">[<a href="#viewerrole">ViewerRole</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#viewerrolepageinfo">ViewerRolePageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### ViewerRolePageInfo

Page information for ViewerRole

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### Webhook

Webhook

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
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client</strong></td>
<td valign="top"><a href="#client">Client</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Template used to generate webhook URL. Valid merge fields are @eventType, @webhookId, @contextId.. Roles: client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headers</strong></td>
<td valign="top"><a href="#webhookheaderconnection">WebhookHeaderConnection</a></td>
<td>

Roles: client.admin.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>body</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Template used to generate webhook request body. Valid merge fields are @eventType, @webhookId, @contextId.. Roles: client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>systemEventTypes</strong></td>
<td valign="top"><a href="#webhooksystemeventtypeconnection">WebhookSystemEventTypeConnection</a></td>
<td>

Roles: client.admin.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageIndex</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pageSize</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">sortByDirection</td>
<td valign="top"><a href="#sortbydirectioninput">SortByDirectionInput</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>enabled</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: client.admin.

</td>
</tr>
</tbody>
</table>

### WebhookConnection

Connection for Webhook

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
<td valign="top">[<a href="#webhook">Webhook</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#webhookpageinfo">WebhookPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### WebhookHeader

Webhook header

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### WebhookHeaderConnection

Connection for WebhookHeader

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
<td valign="top">[<a href="#webhookheader">WebhookHeader</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#webhookheaderpageinfo">WebhookHeaderPageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### WebhookHeaderPageInfo

Page information for WebhookHeader

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### WebhookPageInfo

Page information for Webhook

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### WebhookSystemEventType

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
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>systemEventType</strong></td>
<td valign="top"><a href="#systemeventtype">SystemEventType</a></td>
<td>

Roles: client.admin.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### WebhookSystemEventTypeConnection

Connection for WebhookSystemEventType

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
<td valign="top">[<a href="#webhooksystemeventtype">WebhookSystemEventType</a>]</td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="#webhooksystemeventtypepageinfo">WebhookSystemEventTypePageInfo</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### WebhookSystemEventTypePageInfo

Page information for WebhookSystemEventType

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
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageIndex</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageSize</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Roles: everyone.

</td>
</tr>
</tbody>
</table>

### fileUploadCredentials

All the parameters required for the upload of a file directly to an S3 bucket

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
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>bucket</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>region</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>keyStart</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>acl</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>policy</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>algorithm</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>credential</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>date</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>signature</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
</tbody>
</table>

### fileUploadLinkType

File upload signed url type

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
<td colspan="2" valign="top"><strong>globalId</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: everyone.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>key</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Roles: client.admin, client.editor.

</td>
</tr>
</tbody>
</table>

## Enums

### AgeRestriction

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>OVER18</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>UNDER18</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ALL</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>OTHER</strong></td>
<td></td>
</tr>
</tbody>
</table>

### AgeRestrictionInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>OVER18</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>UNDER18</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ALL</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>OTHER</strong></td>
<td></td>
</tr>
</tbody>
</table>

### ArtistSortOptionsInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>ID</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NAME</strong></td>
<td></td>
</tr>
</tbody>
</table>

### ClientSortOptionsInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>ID</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NAME</strong></td>
<td></td>
</tr>
</tbody>
</table>

### CountrySortOptionsInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>ID</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NAME</strong></td>
<td></td>
</tr>
</tbody>
</table>

### EventSortOptionsInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>ID</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NAME</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>CREATEDDATE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>STARTDATE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>DISTANCE</strong></td>
<td></td>
</tr>
</tbody>
</table>

### FeedbackContext

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>EventEditor</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>McrSatisfaction</strong></td>
<td></td>
</tr>
</tbody>
</table>

### FeedbackContextInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>EventEditor</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>McrSatisfaction</strong></td>
<td></td>
</tr>
</tbody>
</table>

### FeedbackSortOptionsInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>CreatedDate</strong></td>
<td></td>
</tr>
</tbody>
</table>

### FileUploadPurposeInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>EVENTDESCRIPTION</strong></td>
<td></td>
</tr>
</tbody>
</table>

### Gender

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>MALE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>FEMALE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NON_SPECIFIC</strong></td>
<td></td>
</tr>
</tbody>
</table>

### GenderInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>MALE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>FEMALE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NON_SPECIFIC</strong></td>
<td></td>
</tr>
</tbody>
</table>

### OfferCodeSortOptionsInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>ID</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>TITLE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>CREATEDDATE</strong></td>
<td></td>
</tr>
</tbody>
</table>

### OrderChannel

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>BOX_OFFICE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>WEB</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>MOBILE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>PHONE_BOOKING</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>RETAIL</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>FACEBOOK</strong></td>
<td></td>
</tr>
</tbody>
</table>

### OrderChannelInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>BOX_OFFICE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>WEB</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>MOBILE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>PHONE_BOOKING</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>RETAIL</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>FACEBOOK</strong></td>
<td></td>
</tr>
</tbody>
</table>

### OrderSortOptionsInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>ID</strong></td>
<td></td>
</tr>
</tbody>
</table>

### SaleChannelInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>BOXOFFICE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ONLINE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>PHONE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>RETAIL</strong></td>
<td></td>
</tr>
</tbody>
</table>

### SkinSortOptionsInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>ID</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NAME</strong></td>
<td></td>
</tr>
</tbody>
</table>

### SortByDirectionInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>ASC</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>DESC</strong></td>
<td></td>
</tr>
</tbody>
</table>

### StatusOptions

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>VALID</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>PAYMENT_PENDING</strong></td>
<td></td>
</tr>
</tbody>
</table>

### StatusOptionsInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>VALID</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>PAYMENT_PENDING</strong></td>
<td></td>
</tr>
</tbody>
</table>

### SystemEventType

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>TICKET_SAVED</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ORDER_SAVED</strong></td>
<td></td>
</tr>
</tbody>
</table>

### SystemEventTypeInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>TICKET_SAVED</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ORDER_SAVED</strong></td>
<td></td>
</tr>
</tbody>
</table>

### TicketSortOptionsInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>ID</strong></td>
<td></td>
</tr>
</tbody>
</table>

### TicketTypeSortOptionsInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>ID</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>TITLE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>CREATEDDATE</strong></td>
<td></td>
</tr>
</tbody>
</table>

### UserStatus

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>WAITING_CONFIRMATION</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ENABLED</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>DISABLED</strong></td>
<td></td>
</tr>
</tbody>
</table>

### UserStatusInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>WAITING_CONFIRMATION</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ENABLED</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>DISABLED</strong></td>
<td></td>
</tr>
</tbody>
</table>

### VenuesSortOptionsInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>ID</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NAME</strong></td>
<td></td>
</tr>
</tbody>
</table>

### userSortByOptionsInput

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>ID</strong></td>
<td></td>
</tr>
</tbody>
</table>

## Scalars

### Boolean

The `Boolean` scalar type represents `true` or `false`.

### Date

Date custom scalar type

### Float

The `Float` scalar type represents signed double-precision fractional values as specified by [IEEE 754](http://en.wikipedia.org/wiki/IEEE_floating_point). 

### Int

The `Int` scalar type represents non-fractional signed whole numeric values. Int can represent values between -(2^31) and 2^31 - 1. 

### String

The `String` scalar type represents textual data, represented as UTF-8 character sequences. The String type is most often used by GraphQL to represent free-form human-readable text.

