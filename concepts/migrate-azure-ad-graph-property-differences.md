---
title: Diferenças de propriedade entre o Azure AD Graph e o Microsoft Graph
description: Descreve as diferenças de propriedade entre os recursos do Azure AD Graph (entidades) e o Microsoft Graph, para ajudar a migrar os aplicativos de acordo.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 3f80a54a3dd887293dff22f6ceb976b6d8c9e780
ms.sourcegitcommit: 096bad7aaaa5d9b5ce698a524cb21f4070c7b4d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2022
ms.locfileid: "62056320"
---
# <a name="property-differences-between-azure-ad-graph-and-microsoft-graph"></a>Diferenças de propriedade entre o Azure AD Graph e o Microsoft Graph

Este artigo faz parte da *etapa 1: analisar as* diferenças de API do processo para [migrar aplicativos.](migrate-azure-ad-graph-planning-checklist.md)

Em geral, a melhor maneira de comparar a API Azure Active Directory (Azure AD) Graph com o Microsoft Graph é comparar os metadados subjacentes para cada serviço, especialmente as descrições de recursos:

- [Metadados do Azure AD Graph metadados](https://graph.windows.net/microsoft.com/$metadata?api-version=1.6)
- [Metadados beta Graph Microsoft](https://graph.microsoft.com/beta/$metadata)
- [Metadados do Microsoft Graph v1.0](https://graph.microsoft.com/v1.0/$metadata)

Este artigo destaca as diferenças de propriedade entre recursos. Se uma propriedade não for mostrada nesta lista, ela já estará disponível na [versão v1.0](/graph/api/overview) do Microsoft Graph, com exatamente o mesmo nome do Azure AD Graph.

Como os [recursos do](#user-property-differences) usuário [e](#group-property-differences) do grupo são usados com tanta frequência, eles são listados primeiro. Outros recursos são listados em ordem alfabética.

## <a name="user-property-differences"></a>Diferenças de propriedade do usuário

O recurso de usuário do  Azure AD Graph herda de **DirectoryObject**; ele foi renomeado para usuário no Microsoft Graph e herda de **directoryObject**.  Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>Propriedade (v1.6) |Microsoft Graph<br>propriedade|Comentários|
|---|---|---|
| **deletedTimestamp**| beta &nbsp; - &nbsp; **deletedDateTime** <br> v1.0 &nbsp; - &nbsp; **deletedDateTime** | |
| **dirSyncEnabled** | beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** | |
| **facsimileTelephoneNumber** | &nbsp; - &nbsp; **faxnumber** beta <br> faxNumber v1.0 &nbsp; - &nbsp;  | |
| **immutableId** | beta &nbsp; - &nbsp; **onPremisesImmutableId** <br> v1.0 &nbsp; - &nbsp; **onPremisesImmutableId**  | |
| **isCompromised** | beta &nbsp; - &nbsp; _Não disponível_ <br> v1.0 &nbsp; - &nbsp; _Não disponível_ | A API Graph [de proteção de identidade](/graph/api/resources/identityprotection-root?view=graph-rest-beta&preserve-view=true) da Microsoft fornece funcionalidades mais sofisticadas. |
| **lastDirSyncDateTime** | beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime** <br> v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** | |
| **mobile** | beta &nbsp; - &nbsp; **mobilePhone** <br> v1.0 &nbsp; - &nbsp; **mobilePhone** | |
| **provisioningErrors** | beta &nbsp; - &nbsp; _Não disponível_ <br> v1.0 &nbsp; - &nbsp; _Não disponível_ | Essa propriedade e suas informações são preterida.  No entanto, uma nova propriedade que descreve qualquer erro de provisionamento Conexão AD pode ser encontrada em **onPremisesProvisioningErrors** |
| **refreshTokensValidFromDateTime** | beta &nbsp; - &nbsp; **signinSessionsValidFromDateTime**<br>v1.0 &nbsp; - &nbsp; **signinSessionsValidFromDateTime** | |
| **signinNames** | beta &nbsp; - &nbsp; **identities/signInType** <br> identidades &nbsp; - v1.0/signInType &nbsp;  | Essa propriedade agora faz parte do [recurso objectIdentity.](/graph/api/resources/objectIdentity)|
| **telephoneNumber** | beta &nbsp; - &nbsp; **businessPhones** <br> v1.0 &nbsp; - &nbsp; **businessPhones** | |
| **thumbnailPhoto** | foto beta &nbsp; - &nbsp; , fotos <br> v1.0 &nbsp; - &nbsp; **photo**, photos | A foto em miniatura do Azure AD não está disponível por meio do Microsoft Graph.  Em vez [disso, use a API de](/graph/api/resources/profilephoto) fotos. |
| **userIdentities** | identidades &nbsp; - beta &nbsp;  <br> identidades v1.0 &nbsp; - &nbsp;  | Consulte [objectIdentity](/graph/api/resources/objectIdentity) resource type para obter mais detalhes.|
| **userState** | beta &nbsp; - &nbsp; **externalUserState** <br> v1.0 &nbsp; - &nbsp; **externalUserState** | |
| **userStateChangedOn** | beta &nbsp; - &nbsp; **externalUserStateChangeDateTime**<br>v1.0 &nbsp; - &nbsp; **externalUserStateChangeDateTime** | |

## <a name="group-property-differences"></a>Diferenças de propriedades de grupo

O recurso Graph **group** do Azure AD herda de **DirectoryObject**; ele foi renomeado para agrupar no Microsoft Graph e herda de **directoryObject**.  Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>Propriedade (v1.6) |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **dirSyncEnabled** | beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** | |
| **immutableId** | beta &nbsp; - &nbsp; **onPremisesImmutableId** <br> v1.0 &nbsp; - &nbsp; **onPremisesImmutableId** | |
| **lastDirSyncDateTime** | beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime**<br>v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** | |
| **provisioningErrors** | beta &nbsp; - &nbsp; _Não disponível_ <br> v1.0 &nbsp; - &nbsp; _Não disponível_ | Essa propriedade e suas informações são preterida.  No entanto, uma nova propriedade que descreve qualquer erro de provisionamento Conexão AD pode ser encontrada em **onPremisesProvisioningErrors** |

## <a name="application-property-differences"></a>Diferenças de propriedades do aplicativo

O recurso aplicativo do Azure AD Graph herda de **DirectoryObject**; ele foi renomeado para aplicativo no Microsoft Graph e herda de **directoryObject**.   Aqui estão as diferenças de propriedade:


| Azure AD Graph. <br>Propriedade (v1.6) | Microsoft Graph<br> propriedade                                                                                                                          | Comentários                                                                                                                                                                                                                                                                                                                     |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **acceptMappedClaims**             | api &nbsp; - &nbsp; **beta/acceptMappedClaims** <br> &nbsp; - &nbsp; **api/acceptMappedClaims** v1.0                                                       | acceptMappedClaims agora faz parte do novo recurso de api.                                                                                                                                                                                                                                                                      |
| **availableToOtherTenants**        | beta &nbsp; - &nbsp; **signInAudience** <br> v1.0 &nbsp; - &nbsp; **signInAudience**                                                                      | O valor padrão para availableToOtherTenants `false` é `AzureADMyOrg` (significando ) enquanto para signInAudience é `AzureADandPersonalMicrosoftAccount` .                                                                                                                                                                                                                                                                                                                              |
| **errorUrl**                       | beta &nbsp; - &nbsp; _não disponível_ <br> v1.0 &nbsp; - &nbsp; _não disponível_                                                                              | Essa propriedade é preterida.                                                                                                                                                                                                                                                                                                 |
| **homepage**                       | beta &nbsp; - &nbsp; **web/homePageUrl** <br> v1.0 &nbsp; - &nbsp; **web/homePageUrl**                                                                     | homepage agora faz parte do novo recurso Web.                                                                                                                                                                                                                                                                                |
| **informationalUrls**              | informações &nbsp; - &nbsp; **beta** <br> informações v1.0 &nbsp; - &nbsp;                                                                                            |                                                                                                                                                                                                                                                                                                                              |
| **knownClientApplications**        | api &nbsp; - &nbsp; **beta/knownClientApplications** <br> api &nbsp; - v1.0/knownClientApplications &nbsp;                                                | knownClientApplications agora faz parte do novo recurso de api.                                                                                                                                                                                                                                                                 |
| **logoutUrl**                      | beta &nbsp; - &nbsp; **web/logoutUrl** <br> v1.0 &nbsp; - &nbsp; **web/logoutUrl**                                                                         | logoutUrl agora faz parte do recurso Web.                                                                                                                                                                                                                                                                                   |
| **logoUrl**                        | beta &nbsp; - &nbsp; **info/logoUrl** <br> v1.0 &nbsp; - &nbsp; **info/logoUrl**                                                                           | logoUrl agora faz parte do novo recurso de informações.                                                                                                                                                                                                                                                                                |
| **mainLogo**                       | logotipo &nbsp; - &nbsp; **beta** <br> logotipo v1.0 &nbsp; - &nbsp;                                                                                             |                                                                                                                                                                                                                                                                                                                              |
| **oauth2AllowIdTokenImplicitFlow** | beta &nbsp; - &nbsp; **web/implicitGrantSettings/enableIdTokenIssuance**<br>v1.0 &nbsp; - &nbsp; **web/implicitGrantSettings/enableIdTokenIssuance**         | Renomeado e agora parte do novo recurso implicitGrantSettings.                                                                                                                                                                                                                                                             |
| **oauth2AllowImplicitFlow**        | beta &nbsp; - &nbsp; **web/implicitGrantSettings/enableAccessTokenIssuance**<br>v1.0 &nbsp; - &nbsp; **web/implicitGrantSettings/enableAccessTokenIssuance** | Renomeado e agora parte do novo recurso implicitGrantSettings.                                                                                                                                                                                                                                                             |
| **oauth2AllowUrlPathMatching**     | beta &nbsp; - &nbsp; _não disponível_ <br> v1.0 &nbsp; - &nbsp; _não disponível_                                                                              | Essa propriedade é preterida.                                                                                                                                                                                                                                                                                                 |
| **oauth2Permissions**              | api &nbsp; - &nbsp; **beta/oauth2PermissionScopes**<br> &nbsp; - &nbsp; **api/oauth2PermissionScopes** v1.0                                                  | Renomeado e agora parte do novo recurso de api.                                                                                                                                                                                                                                                                                |
| **publicClient**                   | beta &nbsp; - &nbsp; **isFallbackPublicClient** <br> v1.0 &nbsp; - &nbsp; **éFallbackPublicClient**                                                      | Essa propriedade agora tem um novo significado que contém as configurações do cliente &nbsp; - &nbsp; público, como redirectUris. Determinar se o aplicativo é um cliente público ou confidencial agora é feito automaticamente, com a propriedade isFallbackPublicClient manipulando um caso especial que não pode ser determinado automaticamente. |
| **recordConsentConditions**        | beta &nbsp; - &nbsp; _não disponível_ <br> v1.0 &nbsp; - &nbsp; _não disponível_                                                                              | Essa propriedade é preterida.                                                                                                                                                                                                                                                                                                 |
| **replyUrls**                      | beta &nbsp; - &nbsp; **web/redirectUris**, **publicClient/redirectUris**<br> v1.0 &nbsp; - &nbsp; **Web/redirectUris**, **publicClient/redirectUris**        | Além de ser renomeado, redirectUris agora faz parte dos novos recursos Web e publicClient. Isso permite que os desenvolvedores usem URIs específicas para seus clientes públicos e web (como um aplicativo instalado em um dispositivo de área de trabalho).                                                                                           |
| **samlMetadataUrl**                | beta &nbsp; - &nbsp; _Ainda não disponível_  <br> v1.0 &nbsp; - &nbsp; _Ainda não disponível_                                                                  |                                                                                                                                                                                                                                                                                                                              |
| **serviceEndpoints**               | beta &nbsp; - &nbsp; _Não disponível_  <br> v1.0 &nbsp; - &nbsp; _Não disponível_                                                                          | Essa propriedade é preterida, mas é planejada para servicePrincipal.                                                                                                                                                                                                                                                            |

## <a name="approleassignment-differences"></a>Diferenças de AppRoleAssignment

O recurso Graph **AppRoleAssignment** do Azure AD herda de **DirectoryObject;** ele foi renomeado para **appRoleAssignment** no Microsoft Graph e herda de **directoryObject**. Aqui estão as diferenças de propriedade:


|Azure AD Graph. <br>Propriedade (v1.6) |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **creationTimestamp** | beta &nbsp; - &nbsp; **creationTimestamp** <br> v1.0 &nbsp; - &nbsp; **createdDateTime** | |
| **id** | beta &nbsp; - &nbsp; **appRoleId** <br> v1.0 &nbsp; - &nbsp; **appRoleId** | |

## <a name="contact-property-differences"></a>Diferenças de propriedade de contato

O recurso de contato do  Azure AD Graph herda de **DirectoryObject**; ele foi renomeado para **orgContact** no Microsoft Graph e herda de **directoryObject**. Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>Propriedade (v1.6) |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **city** | endereços beta &nbsp; - &nbsp; **(cidade)** <br> endereços v1.0 &nbsp; - &nbsp; **(cidade)**  | A propriedade city faz parte da coleção de recursos de endereços. |
| **country** | endereços beta &nbsp; - &nbsp;  &nbsp; **(countryOrRegion)**<br> endereços v1.0 &nbsp; - &nbsp;  &nbsp; **(countryOrRegion)**  | A propriedade countryOrRegion faz parte da coleção de recursos de endereços. |
| **dirSyncEnabled** | beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled**   | |
| **facsimileTelephoneNumber** | telefones beta &nbsp; - &nbsp;  &nbsp; **(businessFax)** <br> telefones v1.0 &nbsp; - &nbsp;  &nbsp; **(businessFax)** | Agora parte da coleção phones, que dá suporte a dispositivos móveis, comerciais e businessFax. |
| **physicalDeliveryOfficeName** | beta &nbsp; - &nbsp; **officeLocation** <br> v1.0 &nbsp; - &nbsp; **officeLocation** | |
| **postalCode** | endereços beta &nbsp; - &nbsp;  &nbsp; **(postalCode)**<br> endereços v1.0 &nbsp; - &nbsp;  &nbsp; **(postalCode)** | A propriedade postalCode faz parte da coleção de recursos de endereços. |
| **provisioningErrors** | beta &nbsp; - &nbsp; não disponível <br> v1.0 &nbsp; - &nbsp; não disponível | Essa propriedade e suas informações são preterida.  No entanto, uma nova propriedade que descreve qualquer erro de provisionamento relacionado Conexão AD pode ser encontrada em **onPremisesProvisioningErrors**. Atualmente, isso só está disponível na versão beta. |
| **sipProxyAddress** |  beta &nbsp; - &nbsp; **imAddresses**<br> v1.0 &nbsp; - &nbsp; **imAddresses**  | |
| **state** | endereços beta &nbsp; - &nbsp;  &nbsp; **(estado)**<br> endereços v1.0 &nbsp; - &nbsp;  &nbsp; **(estado)**  | A propriedade state faz parte da coleção de recursos de endereços. |
| **streetAddress** | endereços beta &nbsp; - &nbsp;  &nbsp; **(rua)**<br> endereços v1.0 &nbsp; - &nbsp;  &nbsp; **(rua)**  | A propriedade street faz parte da coleção de recursos de endereços. |
| **telephoneNumber** | telefones beta &nbsp; - &nbsp;  &nbsp; **(negócios)** <br> telefones v1.0 &nbsp; - &nbsp;  &nbsp; **(negócios)** | Agora parte da coleção phones, que dá suporte a dispositivos móveis, comerciais e businessFax. |
| **thumbnailPhoto** | beta &nbsp; - &nbsp; _Ainda &nbsp; não &nbsp; disponível_&nbsp;<br> v1.0 &nbsp; - &nbsp; _Ainda não disponível_ | |

## <a name="contract-property-differences"></a>Diferenças de propriedades de contrato

O recurso contrato do Azure AD Graph herda de **DirectoryObject**; ele foi renomeado para contrato no Microsoft Graph e herda de **directoryObject**.   Aqui estão as diferenças de propriedade:


|Azure AD Graph. <br>Propriedade (v1.6) |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **customerContextId** | beta &nbsp; - &nbsp; **customerId** <br> v1.0 &nbsp; - &nbsp; **customerId**  |  |

## <a name="device-property-differences"></a>Diferenças de propriedade de dispositivo

O recurso dispositivo do Azure AD Graph herda de **DirectoryObject**; ele foi renomeado para dispositivo no Microsoft Graph e herda de **directoryObject**.   Aqui estão as diferenças de propriedade:


|Azure AD Graph. <br>Propriedade (v1.6) |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **approximateLastLogonTimestamp** | beta &nbsp; - &nbsp; **approximateLastSignInDateTime** <br> v1.0 &nbsp; - &nbsp; **approximateLastSignInDateTime** |  |
| **complianceExpiryTime** | conformidade &nbsp; - &nbsp; **betaExpirationDateTime** <br> conformidade &nbsp; - v1.0ExpirationDateTime &nbsp;  |  |
| **deviceObjectVersion** |  beta &nbsp; - &nbsp; **deviceVersion** <br> v1.0 &nbsp; - &nbsp; **deviceVersion** |  |
| **deviceOSType** | beta &nbsp; - &nbsp; **operatingSystem** <br> v1.0 &nbsp; - &nbsp; **operatingSystem** |  |
| **deviceOSVersion** | beta &nbsp; - &nbsp; **operatingSystemVersion** <br> v1.0 &nbsp; - &nbsp; **operatingSystemVersion** |  |
| **devicePhysicalIds** | beta &nbsp; - &nbsp; **physicalIds** <br> v1.0 &nbsp; - &nbsp; **physicalIds** |  |
| **deviceTrustType** | beta &nbsp; - &nbsp; **trustType** <br> v1.0 &nbsp; - &nbsp; **trustType** |  |
| **dirSyncEnabled** |  beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** |  |
| **lastDirSyncTime** |  beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime** <br> v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** |  |

## <a name="directoryobject-property-differences"></a>Diferenças de propriedade DirectoryObject

O recurso Graph **DirectoryObject** do Azure AD foi renomeado para **directoryObject** no Microsoft Graph. As alterações em suas propriedades também serão vistas em outros recursos que herdam **de DirectoryObject**. Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>Propriedade (v1.6) |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **deletionTimestamp** | beta &nbsp; - &nbsp; **deletedDateTime** <br> v1.0 &nbsp; - &nbsp; **deletedDateTime** | Enquanto **deletionTimestamp** era um tipo DateTime, **deletedDateTime** é um tipo DateTimeOffset.  |
| **objectId** | id beta &nbsp; - &nbsp;  <br> id v1.0 &nbsp; - &nbsp;  | A **propriedade id** no Microsoft Graph é herdada do [recurso entity.](/graph/api/resources/entity) |
| **objectType** | beta &nbsp; - &nbsp; *Não disponível* <br> v1.0 &nbsp; - &nbsp; *Não disponível* | Essa propriedade não é usada no Microsoft Graph. Em vez disso, o Microsoft Graph retorna a **propriedade @odata.type,** mas somente para APIs que podem retornar objetos de diferentes tipos ou tipos derivados. Por exemplo, a API [de](/graph/api/group-list-members) membros do grupo lista pode retornar membros que são [usuários,](/graph/api/resources/user) [grupos,](/graph/api/resources/group)entidades de [serviço,](/graph/api/resources/serviceprincipal)contatos organizacionais ou [dispositivos](/graph/api/resources/orgcontact). [](/graph/api/resources/device) Para usuários, o **@odata.type** é `#microsoft.graph.user` . |

## <a name="directoryobjectreference-property-differences"></a>Diferenças de propriedade DirectoryObjectReference

O recurso Graph **DirectoryObjectReference** do Azure AD herda de **DirectoryObject**; ele foi renomeado para **directoryObjectPartnerReference** no Microsoft Graph e herda de **directoryObject**. Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>Propriedade (v1.6) |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **externalContextId** | beta &nbsp; - &nbsp; **externalPartnerTenantId** <br> v1.0 &nbsp; - &nbsp; **externalPartnerTenantId** |  |

## <a name="domain-property-differences"></a>Diferenças de propriedades de domínio

O recurso domínio do Azure AD Graph foi renomeado para **domínio** no Microsoft Graph.  Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>Propriedade (v1.6) |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **name** | id beta &nbsp; - &nbsp;  <br> id v1.0 &nbsp; - &nbsp;  | No Microsoft Graph, o identificador exclusivo (id) contém o nome de domínio; a `name` propriedade não existe. |
| **forceDeleteState** |  estado &nbsp; - &nbsp; **beta** <br> estado v1.0 &nbsp; - &nbsp;  | No Azure AD Graph, há propriedades forceDelete e estado de domínio separadas.  No Microsoft Graph, todos os estados de domínio são manipulados pela propriedade state. |
| **isDefaultForCloudRedirections** | beta &nbsp; - &nbsp; _Ainda &nbsp; não &nbsp; disponível_&nbsp;<br> v1.0 &nbsp; - &nbsp; _Ainda não disponível_ | |

## <a name="oauth2permissionsgrant-property-differences"></a>Diferenças de propriedade OAuth2PermissionsGrant

O recurso do Azure AD Graph **OAuth2PermissionsGrant** foi renomeado para **oAuth2PermissionsGrant** no Microsoft Graph. Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>Propriedade (v1.6) |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **expiryTime** | beta &nbsp; - &nbsp; **expiryTime** <br> v1.0 &nbsp; - &nbsp; _Removido_ | Essa propriedade não é usada e é removida no Microsoft Graph v1.0. |
| **startTime** | beta &nbsp; - &nbsp; **startTime** <br> v1.0 &nbsp; - &nbsp; _Removido_  | Essa propriedade não é usada e é removida no Microsoft Graph v1.0. |

## <a name="policy-property-differences"></a>Diferenças de propriedade de política

No Microsoft Graph, há tipos de política nomeados (como **tokenIssuancePolicy** ou **tokenLifetimePolicy**) em vez de um tipo de recurso de política genérico. Mais detalhes estão disponíveis na visão geral [da política.](/graph/api/resources/policy-overview)

## <a name="serviceendpoint-property-differences"></a>Diferenças de propriedade ServiceEndpoint

O recurso Graph **ServiceEndpoint** do Azure AD herda de **DirectoryObject**; ele foi renomeado para ponto de extremidade no Microsoft Graph e herda de **directoryObject**.  Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>Propriedade (v1.6) |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **serviceId** | beta &nbsp; - &nbsp; **providerId**<br> v1.0 &nbsp; - &nbsp; **providerId** | |
| **serviceName** | beta &nbsp; - &nbsp; **providerName**<br> v1.0 &nbsp; - &nbsp; **providerName** | |
| **resourceId** | provedor &nbsp; - &nbsp; **betaResourceId**<br> provedor &nbsp; - v1.0ResourceId &nbsp;  | |

## <a name="serviceprincipal-property-differences"></a>Diferenças de propriedade ServicePrincipal

O recurso Graph **ServicePrincipal** do Azure AD herda de **DirectoryObject**; ele foi renomeado para **servicePrincipal** no Microsoft Graph e herda de **directoryObject**. Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>Propriedade (v1.6) |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **appOwnerTenantId** | beta &nbsp; - &nbsp; **appOwnerOrganizationId** <br> v1.0 &nbsp; - &nbsp; **appOwnerOrganizationId** | Renomeado. |
| **informationalUrls**| informações &nbsp; - &nbsp; **beta** <br> informações v1.0 &nbsp; - &nbsp;  | |
| **oauth2Permissions** | beta &nbsp; - &nbsp; **publishedPermissionScopes** <br> v1.0 &nbsp; - &nbsp; **oauth2PermissionScopes** | Renomeado. |
| **preferredTokenSigningKeyEndDateTime** | beta &nbsp; - &nbsp; _Ainda não disponível_ <br> v1.0 &nbsp; -  _Ainda não disponível_ | |
| **signInAudience** | beta &nbsp; - &nbsp; _Ainda não disponível_ <br> v1.0 &nbsp; -  _Ainda não disponível_ | |
| **serviceEndpoints** | ponto &nbsp; - &nbsp; **de extremidade** beta <br> ponto de extremidade v1.0 &nbsp; - &nbsp;  | Renomeado. |

## <a name="tenantdetails-property-differences"></a>Diferenças de propriedade TenantDetails

O recurso Graph **TenantDetail** do Azure AD herda de **DirectoryObject**; ele foi renomeado para organização no Microsoft Graph e herda de **directoryObject**.  Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>Propriedade (v1.6) |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **companyLastDirSyncTime** | beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime** <br> v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** |  |
| **dirSyncEnabled** | beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** |  |
| **provisioningErrors** | beta &nbsp; - &nbsp; _Não disponível_ <br> v1.0 &nbsp; - &nbsp; _Não disponível_ | Essa propriedade e suas informações são preterida.|
| **telephoneNumber** | beta &nbsp; - &nbsp; **businessPhones** <br> v1.0 &nbsp; - &nbsp; **businessPhones** |  |

## <a name="trustedcasforpasswordlessauth-property-differences"></a>Diferenças de propriedade TrustedCasForPasswordlessAuth

O recurso do Azure AD Graph **TrustedCasForPasswordlessAuth** foi renomeado para [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedauthconfiguration). Não há diferenças de propriedade; no entanto, há diferenças no tipo de recurso **certificateAuthority** usado pela **propriedade certificateAuthorities.**

### <a name="certificateauthorityinformation-property-differences"></a>Diferenças de propriedade CertificateAuthorityInformation

O certificado do Azure AD Graph **CertificateAuthorityInformation** foi renomeado para **certificateAuthority** no Microsoft Graph. A seguir estão as diferenças de propriedade.

|Azure AD Graph. <br>Propriedade (v1.6) |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **authorityType** | beta &nbsp; - &nbsp; **isRootAuthority**<br> v1.0 &nbsp; - &nbsp; **isRootAuthority** | O tipo dessa propriedade também foi alterado para um Boolean. Anteriormente, essa propriedade precisava ser definida como "RootAuthority" ou "IntermediateAuthority". Definir a nova propriedade como **true** é equivalente a "RootAuthority". |
| **crlDistributionPoint** | beta &nbsp; - &nbsp; **certificateRevocationListUrl** <br> v1.0 &nbsp; - &nbsp; **certificateRevocationListUrl** | |
| **deltaCrlDistributionPoint** | beta &nbsp; - &nbsp; **deltaCertificateRevocationListUrl** <br> v1.0 &nbsp; - &nbsp; **deltaCertificateRevocationListUrl** | |
| **trustedCertificate** | certificado &nbsp; - beta &nbsp;  <br> v1.0 &nbsp; - &nbsp; **deltaCertificateRevocationListUrl** | |
| **trustedIssuer** | emissor &nbsp; - beta &nbsp; <br> emissor v1.0 &nbsp; - &nbsp;  | |
| **trustedIssuerSki** | beta &nbsp; - &nbsp; **issuerSki**<br> emissor v1.0Ski &nbsp; - &nbsp;  | |

## <a name="next-steps"></a>Próximas etapas

- Saiba mais [sobre as diferenças de](migrate-azure-ad-graph-method-differences.md) método entre o Azure AD Graph e o Microsoft Graph.
- Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.

