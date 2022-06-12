---
title: Diferenças de propriedade entre Azure AD Graph e o Microsoft Graph
description: Descreve as diferenças de propriedade entre Azure AD Graph (entidades) e o Microsoft Graph, para ajudar a migrar aplicativos adequadamente.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: ba7a61b132b004f7ba07ccdae8ae8b00bb537ef3
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034674"
---
# <a name="property-differences-between-azure-ad-graph-and-microsoft-graph"></a>Diferenças de propriedade entre Azure AD Graph e o Microsoft Graph

Este artigo faz parte da *etapa 1: examinar as diferenças de API* do [processo para migrar aplicativos](migrate-azure-ad-graph-planning-checklist.md).

Em geral, a melhor maneira de comparar o Azure Active Directory (Azure AD) API do Graph com o Microsoft Graph é comparar os metadados subjacentes para cada serviço, especialmente as descrições de recursos:

- [Azure AD Graph metadados](https://graph.windows.net/microsoft.com/$metadata?api-version=1.6)
- [Metadados beta Graph Microsoft](https://graph.microsoft.com/beta/$metadata)
- [Metadados do Microsoft Graph v1.0](https://graph.microsoft.com/v1.0/$metadata)

Este artigo destaca as diferenças de propriedade entre os recursos. Se uma propriedade não for mostrada nesta lista, ela já estará disponível na versão [v1.0](/graph/api/overview) do Microsoft Graph, com exatamente o mesmo nome do Azure AD Graph.

Como os [recursos de](#user-property-differences) usuário [e](#group-property-differences) grupo são usados com tanta frequência, eles são listados primeiro. Outros recursos são listados em ordem alfabética.

## <a name="user-property-differences"></a>Diferenças de propriedade do usuário

O Azure AD Graph **user** é herdado de **DirectoryObject**; ele foi renomeado para usuário no Microsoft Graph  e herda de **directoryObject**. Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>(v1.6) property |Microsoft Graph<br>propriedade|Comentários|
|---|---|---|
| **deletedTimestamp**| beta  &nbsp;-&nbsp; **deletedDateTime** <br> v1.0 &nbsp;-&nbsp; **deletedDateTime** | |
| **dirSyncEnabled** | beta &nbsp;-&nbsp;**onPremisesSyncEnabled** <br> v1.0 &nbsp;-&nbsp; **onPremisesSyncEnabled** | |
| **facsimileTelephoneNumber** | **faxNumber beta** &nbsp;-&nbsp; <br> **faxNumber** v1.0 &nbsp;-&nbsp; | |
| **immutableId** | beta &nbsp;-&nbsp;**onPremisesImmutableId** <br> v1.0 &nbsp;-&nbsp; **onPremisesImmutableId**  | |
| **isCompromised** | beta  &nbsp;-&nbsp; _Não disponível_ <br> v1.0 &nbsp;-&nbsp; _Não disponível_ | A API Graph [proteção de identidade do](/graph/api/resources/identityprotection-root?view=graph-rest-beta&preserve-view=true) Microsoft Graph fornece funcionalidades mais sofisticadas. |
| **lastDirSyncDateTime** | beta &nbsp;-&nbsp;**onPremisesLastSyncDateTime** <br> v1.0 &nbsp;-&nbsp; **onPremisesLastSyncDateTime** | |
| **Móvel** | beta  &nbsp;-&nbsp; **mobilePhone** <br> v1.0 &nbsp;-&nbsp; **mobilePhone** | |
| **passwordProfile/enforceChangePasswordPolicy** | beta  &nbsp;-&nbsp; **passwordProfile/forceChangePasswordNextSignIn** <br> v1.0 &nbsp;-&nbsp; **passwordProfile/forceChangePasswordNextSignIn** | |
| **passwordProfile/forceChangePasswordNextLogin** | beta  &nbsp;-&nbsp; **passwordProfile/forceChangePasswordNextSignInWithMfa** <br> v1.0 &nbsp;-&nbsp; **passwordProfile/forceChangePasswordNextSignInWithMfa** | |
| **provisioningErrors** | beta &nbsp;-&nbsp; _Não disponível_ <br> v1.0 &nbsp;-&nbsp; _Não disponível_ | Essa propriedade e suas informações foram preteridas.  No entanto, uma nova propriedade que descreve todos os erros de provisionamento relacionados Conexão AD pode ser encontrada em **onPremisesProvisioningErrors** |
| **refreshTokensValidFromDateTime** | beta&nbsp;-&nbsp;**signinSessionsValidFromDateTime**<br>v1.0&nbsp;-&nbsp;**signinSessionsValidFromDateTime** | |
| **signinNames** | beta &nbsp;-&nbsp; **identities/signInType** <br> identidades v1.0 &nbsp;-&nbsp; **/signInType** | Essa propriedade agora faz parte do recurso [objectIdentity](/graph/api/resources/objectIdentity) .|
| **telephoneNumber** | beta  &nbsp;-&nbsp; **businessPhones** <br> **businessPhones** v1.0 &nbsp;-&nbsp; | |
| **thumbnailPhoto** | foto **beta**&nbsp;-&nbsp;, fotos <br> foto v1.0 &nbsp;-&nbsp; **,** fotos | A Azure AD em miniatura não está disponível por meio do Microsoft Graph.  Em vez disso [, use a API de](/graph/api/resources/profilephoto) fotos. |
| **userIdentities** | **identidades beta** &nbsp;-&nbsp; <br> Identidades v1.0 &nbsp;-&nbsp; | Consulte [o tipo de recurso objectIdentity](/graph/api/resources/objectIdentity) para obter mais detalhes.|
| **Userstate** | beta  &nbsp;-&nbsp; **externalUserState** <br> v1.0 &nbsp;-&nbsp; **externalUserState** | |
| **userStateChangedOn** | beta&nbsp;-&nbsp;**externalUserStateChangeDateTime**<br>v1.0&nbsp;-&nbsp;**externalUserStateChangeDateTime** | |

## <a name="group-property-differences"></a>Diferenças de propriedade de grupo

O Azure AD Graph **de** grupo é herdado de **DirectoryObject**; ele foi renomeado para agrupar no  Microsoft Graph e herda de **directoryObject**. Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>(v1.6) property |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **dirSyncEnabled** | beta &nbsp;-&nbsp;**onPremisesSyncEnabled** <br> v1.0 &nbsp;-&nbsp; **onPremisesSyncEnabled** | |
| **immutableId** | beta &nbsp;-&nbsp;**onPremisesImmutableId** <br> v1.0 &nbsp;-&nbsp; **onPremisesImmutableId** | |
| **lastDirSyncDateTime** | beta&nbsp;-&nbsp;**onPremisesLastSyncDateTime**<br>v1.0&nbsp;-&nbsp;**onPremisesLastSyncDateTime** | |
| **provisioningErrors** | beta &nbsp;-&nbsp; _Não disponível_ <br> v1.0 &nbsp;-&nbsp; _Não disponível_ | Essa propriedade e suas informações foram preteridas.  No entanto, uma nova propriedade que descreve todos os erros de provisionamento relacionados Conexão AD pode ser encontrada em **onPremisesProvisioningErrors** |

## <a name="application-property-differences"></a>Diferenças de propriedade do aplicativo

O Azure AD Graph **application** é herdado de **DirectoryObject**; ele foi renomeado para aplicativo no Microsoft Graph  e herda de **directoryObject**. Aqui estão as diferenças de propriedade:


| Azure AD Graph. <br>(v1.6) property | Microsoft Graph<br> propriedade                                                                                                                          | Comentários                                                                                                                                                                                                                                                                                                                     |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **acceptMappedClaims**             | beta &nbsp;-&nbsp;**api/acceptMappedClaims** <br> v1.0 &nbsp;-&nbsp; **api/acceptMappedClaims**                                                       | acceptMappedClaims agora faz parte do novo recurso de API.                                                                                                                                                                                                                                                                      |
| **availableToOtherTenants**        | beta &nbsp;-&nbsp; **signInAudience** <br> v1.0 &nbsp;-&nbsp; **signInAudience**                                                                      | O valor padrão para availableToOtherTenants é `false` (ou `AzureADMyOrg`seja), enquanto para signInAudience é `AzureADandPersonalMicrosoftAccount`.                                                                                                                                                                                                                                                                                                                              |
| **errorUrl**                       | beta &nbsp;-&nbsp;_não disponível_ <br> v1.0 &nbsp;-&nbsp;  _não disponível_                                                                            | Essa propriedade foi preterida.                                                                                                                                                                                                                                                                                                 |
| **homepage**                       | beta &nbsp;-&nbsp;**web/homePageUrl** <br> v1.0 &nbsp;-&nbsp; **web/homePageUrl**                                                                     | A home page agora faz parte do novo recurso da Web.                                                                                                                                                                                                                                                                                |
| **informationalUrls**              | informações **beta** &nbsp;-&nbsp; <br> Informações da v1.0 &nbsp;-&nbsp;                                                                                           |                                                                                                                                                                                                                                                                                                                              |
| **knownClientApplications**        | api beta&nbsp;-&nbsp;**/knownClientApplications** <br> api v1.0 &nbsp;-&nbsp;**/knownClientApplications**                                               | knownClientApplications agora faz parte do novo recurso de API.                                                                                                                                                                                                                                                                 |
| **logoutUrl**                      | beta &nbsp;-&nbsp;**web/logoutUrl** <br> v1.0 &nbsp;-&nbsp; **web/logoutUrl**                                                                         | logoutUrl agora faz parte do recurso da Web.                                                                                                                                                                                                                                                                                   |
| **logoUrl**                        | beta &nbsp;-&nbsp;**info/logoUrl** <br> v1.0 &nbsp;-&nbsp; **info/logoUrl**                                                                           | logoUrl agora faz parte do novo recurso de informações.                                                                                                                                                                                                                                                                                |
| **mainLogo**                       | logotipo **beta** &nbsp;-&nbsp; <br> Logotipo da v1.0 &nbsp;-&nbsp;                                                                                            |                                                                                                                                                                                                                                                                                                                              |
| **oauth2AllowIdTokenImplicitFlow** | beta&nbsp;-&nbsp;**web/implicitGrantSettings/enableIdTokenIssuance**<br>v1.0 &nbsp;-&nbsp;**web/implicitGrantSettings/enableIdTokenIssuance**         | Renomeado e agora parte do novo recurso implicitGrantSettings.                                                                                                                                                                                                                                                             |
| **oauth2AllowImplicitFlow**        | beta&nbsp;-&nbsp;**web/implicitGrantSettings/enableAccessTokenIssuance**<br>v1.0 &nbsp;-&nbsp;**web/implicitGrantSettings/enableAccessTokenIssuance** | Renomeado e agora parte do novo recurso implicitGrantSettings.                                                                                                                                                                                                                                                             |
| **oauth2AllowUrlPathMatching**     | beta &nbsp;-&nbsp;_não disponível_ <br> v1.0 &nbsp;-&nbsp;  _não disponível_                                                                            | Essa propriedade foi preterida.                                                                                                                                                                                                                                                                                                 |
| **oauth2Permissions**              | beta&nbsp;-&nbsp;**api/oauth2PermissionScopes**<br> v1.0 &nbsp;-&nbsp;**api/oauth2PermissionScopes**                                                  | Renomeado e agora parte do novo recurso de API.                                                                                                                                                                                                                                                                                |
| **publicClient**                   | beta &nbsp;-&nbsp; **isFallbackPublicClient** <br> v1.0 &nbsp;-&nbsp; **isFallbackPublicClient**                                                      | Essa propriedade agora tem um novo significado que &nbsp;-&nbsp; contém as configurações públicas do cliente, como redirectUris. Determinar se o aplicativo é um cliente público ou confidencial agora é feito automaticamente, com a propriedade isFallbackPublicClient tratando um caso especial que não pode ser determinado automaticamente. |
| **recordConsentConditions**        | beta &nbsp;-&nbsp;_não disponível_ <br> v1.0 &nbsp;-&nbsp;  _não disponível_                                                                            | Essa propriedade foi preterida.                                                                                                                                                                                                                                                                                                 |
| **replyUrls**                      | beta&nbsp;-&nbsp;**web/redirectUris**, **publicClient/redirectUris**<br> v1.0 &nbsp;-&nbsp;**web/redirectUris**, **publicClient/redirectUris**        | Além de ser renomeado, redirectUris agora faz parte dos novos recursos web e publicClient. Isso permite que os desenvolvedores usem URIs específicos para seus clientes Web e públicos (como um aplicativo instalado em um dispositivo de área de trabalho).                                                                                           |
| **samlMetadataUrl**                | beta  &nbsp;-&nbsp; **samlMetadataUrl** <br> v1.0 &nbsp;-&nbsp; _Ainda não disponível_                                                                  |                                                                                                                                                                                                                                                                                                                              |
| **serviceEndpoints**               | beta  &nbsp;-&nbsp; _Não disponível_  <br> v1.0 &nbsp;-&nbsp; _Não disponível_                                                                          | Essa propriedade foi preterida, mas está planejada para servicePrincipal.                                                                                                                                                                                                                                                            |

## <a name="approleassignment-differences"></a>Diferenças de AppRoleAssignment

O Azure AD Graph **appRoleAssignment** herda de **DirectoryObject**; ele foi renomeado para **appRoleAssignment** no Microsoft Graph e herda de **directoryObject**. Aqui estão as diferenças de propriedade:


|Azure AD Graph. <br>(v1.6) property |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **creationTimestamp** | beta &nbsp;-&nbsp;**creationTimestamp** <br> v1.0 &nbsp;-&nbsp;**createdDateTime** | |
| **id** | **appRoleId** beta &nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp;**appRoleId** | |

## <a name="contact-property-differences"></a>Diferenças de propriedade de contato

O Azure AD Graph **contacto** herda de **DirectoryObject**; ele foi renomeado para **orgContact** no Microsoft Graph e herda de **directoryObject**. Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>(v1.6) property |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **city** | endereço beta&nbsp;-&nbsp;**/cidade** <br> endereços **/** cidade v1.0 &nbsp;-&nbsp;  | A **propriedade city** faz parte da coleção **de recursos de** endereços. |
| **País** | endereços beta&nbsp;-&nbsp;**/countryOrRegion**<br> endereços v1.0&nbsp;-&nbsp;**/countryOrRegion**  | A **propriedade countryOrRegion** faz parte da coleção de **recursos** de endereços. |
| **dirSyncEnabled** | beta &nbsp;-&nbsp;**onPremisesSyncEnabled** <br> v1.0 &nbsp;-&nbsp;**onPremisesSyncEnabled**   | |
| **facsimileTelephoneNumber** | telefones beta&nbsp;-&nbsp;**/businessFax** <br> telefones v1.0 &nbsp;-&nbsp;**/businessFax** | Agora faz parte da coleção **de telefones** que dá suporte a vários tipos de telefone. |
| **physicalDeliveryOfficeName** | **officeLocation** beta &nbsp;-&nbsp; <br> **officeLocation** v1.0 &nbsp;-&nbsp; | |
| **postalCode** | endereços beta&nbsp;-&nbsp;**/postalCode**<br> endereços v1.0 &nbsp;-&nbsp;**/postalCode** | A **propriedade postalCode** faz parte da coleção de **recursos** de endereços. |
| **provisioningErrors** | beta &nbsp;-&nbsp; não disponível <br> v1.0 &nbsp;-&nbsp; não disponível | Essa propriedade e suas informações foram preteridas.  No entanto, uma nova propriedade que descreve todos os erros de provisionamento relacionados Conexão AD pode ser encontrada em **onPremisesProvisioningErrors**. Atualmente, isso só está disponível em `beta`. |
| **sipProxyAddress** |  beta &nbsp;-&nbsp;**imAddresses**<br> v1.0 &nbsp;-&nbsp;**imAddresses**  | |
| **state** | endereços &nbsp;-&nbsp;**beta/estado**<br> endereços **/** estado v1.0 &nbsp;-&nbsp;  | A **propriedade de** estado faz parte da coleção **de recursos** de endereços. |
| **streetAddress** | endereços &nbsp;-&nbsp;**beta/rua**<br> endereços **/** rua v1.0 &nbsp;-&nbsp;  | A **propriedade** street faz parte da coleção **de recursos de** endereços. |
| **telephoneNumber** | beta&nbsp;-&nbsp;**phones/business** <br> telefones/**negócios** v1.0 &nbsp;-&nbsp; | Agora faz parte da coleção **de telefones** que dá suporte a vários tipos de telefone. |
| **thumbnailPhoto** | beta &nbsp;-&nbsp;_Ainda&nbsp;não&nbsp;disponível_&nbsp;<br> v1.0 &nbsp;-&nbsp; _Ainda não disponível_ | |

## <a name="contract-property-differences"></a>Diferenças de propriedade do contrato

O Azure AD Graph **de** contrato é herdado de **DirectoryObject**; ele foi renomeado para contrato no Microsoft  Graph e herda de **directoryObject**. Aqui estão as diferenças de propriedade:


|Azure AD Graph. <br>(v1.6) property |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **customerContextId** | customerId beta &nbsp;-&nbsp; <br> customerId v1.0 &nbsp;-&nbsp;  |  |

## <a name="device-property-differences"></a>Diferenças de propriedade do dispositivo

O Azure AD Graph **de** dispositivo herda de **DirectoryObject**; ele foi renomeado para dispositivo no Microsoft Graph  e herda de **directoryObject**. Aqui estão as diferenças de propriedade:


|Azure AD Graph. <br>(v1.6) property |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **approximateLastLogonTimestamp** | beta&nbsp;-&nbsp;**approximateLastSignInDateTime** <br> v1.0 &nbsp;-&nbsp; **approximateLastSignInDateTime** |  |
| **complianceExpiryTime** | beta&nbsp;-&nbsp;**complianceExpirationDateTime** <br> v1.0 &nbsp;-&nbsp; **complianceExpirationDateTime** |  |
| **deviceObjectVersion** |  deviceVersion beta&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; **deviceVersion** |  |
| **deviceOSType** | beta&nbsp;-&nbsp;**operatingSystem** <br> v1.0 &nbsp;-&nbsp; **operatingSystem** |  |
| **deviceOSVersion** | beta&nbsp;-&nbsp;**operatingSystemVersion** <br> v1.0 &nbsp;-&nbsp; **operatingSystemVersion** |  |
| **devicePhysicalIds** | beta&nbsp;-&nbsp;**physicalIds** <br> v1.0 &nbsp;-&nbsp; **physicalIds** |  |
| **deviceTrustType** | beta&nbsp;-&nbsp;**trustType** <br> trustType v1.0 &nbsp;-&nbsp; |  |
| **dirSyncEnabled** |  beta&nbsp;-&nbsp;**onPremisesSyncEnabled** <br> v1.0 &nbsp;-&nbsp; **onPremisesSyncEnabled** |  |
| **lastDirSyncTime** |  beta&nbsp;-&nbsp;**onPremisesLastSyncDateTime** <br> v1.0 &nbsp;-&nbsp; **onPremisesLastSyncDateTime** |  |

## <a name="directoryobject-property-differences"></a>Diferenças de propriedade DirectoryObject

O Azure AD Graph **directoryObject** foi renomeado para **directoryObject** no Microsoft Graph. As alterações em suas propriedades também serão vistas em outros recursos que herdam de **DirectoryObject**. Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>(v1.6) property |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **deletionTimestamp** | beta&nbsp;-&nbsp;**deletedDateTime** <br> v1.0 &nbsp;-&nbsp; **deletedDateTime** | Enquanto **deletionTimestamp** era um tipo DateTime, **deletedDateTime** é um tipo DateTimeOffset.  |
| **Objectid** | **id** beta&nbsp;-&nbsp; <br> id v1.0 &nbsp;-&nbsp; | A **propriedade ID** no Microsoft Graph é herdada do recurso [de](/graph/api/resources/entity) entidade. |
| **objectType** | beta&nbsp;-&nbsp;*Não disponível* <br> v1.0 &nbsp;-&nbsp; *Não disponível* | Essa propriedade não é usada no Microsoft Graph. Em vez disso, o Microsoft Graph retorna **a propriedade @odata.type**, mas somente para APIs que podem retornar objetos de tipos diferentes ou tipos derivados. Por exemplo, a API [de](/graph/api/group-list-members) membros do grupo de lista pode retornar membros que são [usuários](/graph/api/resources/user), [grupos](/graph/api/resources/group), [entidades de serviço](/graph/api/resources/serviceprincipal), [contatos organizacionais](/graph/api/resources/orgcontact) ou [dispositivos](/graph/api/resources/device). Para usuários, **o @odata.type** é `#microsoft.graph.user`. |

## <a name="directoryobjectreference-property-differences"></a>Diferenças de propriedade DirectoryObjectReference

O recurso Azure AD Graph **DirectoryObjectReference** herda de **DirectoryObject**; ele foi renomeado para **directoryObjectPartnerReference** no Microsoft Graph e herda de **directoryObject**. Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>(v1.6) property |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **externalContextId** | beta&nbsp;-&nbsp;**externalPartnerTenantId** <br> v1.0 &nbsp;-&nbsp; **externalPartnerTenantId** |  |

## <a name="domain-property-differences"></a>Diferenças de propriedade de domínio

O Azure AD Graph **domínio** foi renomeado para **domínio** no Microsoft Graph. Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>(v1.6) property |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **name** | **id** beta&nbsp;-&nbsp; <br> id v1.0 &nbsp;-&nbsp; | No Microsoft Graph, o identificador exclusivo (id) contém o nome de domínio; `name` a propriedade não existe. |
| **forceDeleteState** |  estado **beta**&nbsp;-&nbsp; <br> Estado v1.0 &nbsp;-&nbsp; | No Azure AD Graph, há propriedades de estado de domínio e forceDelete separadas.  No Microsoft Graph, todos os estados de domínio são manipulados pela propriedade de estado. |
| **isDefaultForCloudRedirections** | beta&nbsp;-&nbsp;_Ainda&nbsp;não&nbsp;disponível_&nbsp;<br> v1.0 &nbsp;-&nbsp; _Ainda não disponível_ | |

## <a name="oauth2permissionsgrant-property-differences"></a>Diferenças de propriedade OAuth2PermissionsGrant

O Azure AD Graph **recurso OAuth2PermissionsGrant** foi renomeado para **oAuth2PermissionsGrant** no Microsoft Graph. Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>(v1.6) property |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **expiryTime** | beta&nbsp;-&nbsp;**expiryTime** <br> v1.0&nbsp;-&nbsp; Removido | Essa propriedade não é usada e é removida no Microsoft Graph v1.0. |
| **Starttime** | beta&nbsp;-&nbsp;**startTime** <br> v1.0&nbsp;-&nbsp; Removido  | Essa propriedade não é usada e é removida no Microsoft Graph v1.0. |

## <a name="policy-property-differences"></a>Diferenças de propriedade de política

No Microsoft Graph, há tipos de política nomeados (como **tokenIssuancePolicy** ou **tokenLifetimePolicy**) em vez de um tipo de recurso de política genérico. Mais detalhes estão disponíveis na visão geral [da política](/graph/api/resources/policy-overview).

## <a name="serviceendpoint-property-differences"></a>Diferenças de propriedade do ServiceEndpoint

O Azure AD Graph **serviceEndpoint** herda de **DirectoryObject**; ele foi renomeado para ponto de extremidade no Microsoft  Graph e herda de **directoryObject**. Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>(v1.6) property |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **serviceId** | providerId beta&nbsp;-&nbsp;<br> providerId v1.0 &nbsp;-&nbsp; | |
| **serviceName** | beta&nbsp;-&nbsp;**providerName**<br> v1.0 &nbsp;-&nbsp;**providerName** | |
| **resourceId** | beta&nbsp;-&nbsp;**providerResourceId**<br> v1.0 &nbsp;-&nbsp;**providerResourceId** | |

## <a name="serviceprincipal-property-differences"></a>Diferenças de propriedade servicePrincipal

O Azure AD Graph **ServicePrincipal** herda de **DirectoryObject**; ele foi renomeado para **servicePrincipal** no Microsoft Graph e herda de **directoryObject**. Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>(v1.6) property |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **appOwnerTenantId** | beta&nbsp;-&nbsp;**appOwnerOrganizationId** <br> v1.0 &nbsp;-&nbsp;**appOwnerOrganizationId** | Renomeado. |
| **informationalUrls**| informações **beta** &nbsp;-&nbsp; <br> Informações da v1.0 &nbsp;-&nbsp; | |
| **oauth2Permissions** | beta  &nbsp;-&nbsp;**publishedPermissionScopes** <br> v1.0  &nbsp;-&nbsp;**oauth2PermissionScopes** | Renomeado. |
| **preferredTokenSigningKeyEndDateTime** | beta&nbsp;-&nbsp;_Ainda não disponível_ <br> v1.0 &nbsp;- _Ainda não disponível_ | |
| **signInAudience** | beta&nbsp;-&nbsp;_Ainda não disponível_ <br> v1.0 &nbsp;- _Ainda não disponível_ | |
| **serviceEndpoints** | ponto **de extremidade beta**&nbsp;-&nbsp; <br> Ponto de extremidade v1.0 &nbsp;-&nbsp; | Renomeado. |

## <a name="tenantdetails-property-differences"></a>Diferenças de propriedade TenantDetails

O Azure AD Graph **TenantDetail** herda de **DirectoryObject**; ele foi renomeado para organização no Microsoft Graph e  herda de **directoryObject**. Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>(v1.6) property |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **companyLastDirSyncTime** | beta&nbsp;-&nbsp;**onPremisesLastSyncDateTime** <br> v1.0&nbsp;-&nbsp;**onPremisesLastSyncDateTime** |  |
| **dirSyncEnabled** | beta&nbsp;-&nbsp;**onPremisesSyncEnabled** <br> v1.0 &nbsp;-&nbsp; **onPremisesSyncEnabled** |  |
| **provisioningErrors** | beta&nbsp;-&nbsp;_Não disponível_ <br> v1.0&nbsp;-&nbsp;_Não disponível_ | Essa propriedade e suas informações foram preteridas.|
| **telephoneNumber** | beta&nbsp;-&nbsp;**businessPhones** <br> **businessPhones** v1.0&nbsp;-&nbsp; |  |

## <a name="trustedcasforpasswordlessauth-property-differences"></a>Diferenças de propriedade TrustedCasForPasswordlessAuth

O Azure AD Graph **trustedCasForPasswordlessAuth** foi renomeado para [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedauthconfiguration). Não há diferenças de propriedade; no entanto, há diferenças no tipo de recurso **certificateAuthority** usado pela **propriedade certificateAuthorities** .

### <a name="certificateauthorityinformation-property-differences"></a>Diferenças de propriedade CertificateAuthorityInformation

O Azure AD Graph **CertificateAuthorityInformation** foi renomeado para **certificateAuthority** no Microsoft Graph. A seguir estão as diferenças de propriedade.

|Azure AD Graph. <br>(v1.6) property |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **authorityType** | beta&nbsp;-&nbsp;**isRootAuthority**<br> v1.0 &nbsp;-&nbsp;**isRootAuthority** | O tipo dessa propriedade também foi alterado para um booliano. Anteriormente, essa propriedade precisava ser definida como "RootAuthority" ou "IntermediateAuthority". Definir a nova propriedade como **true** é equivalente a "RootAuthority". |
| **crlDistributionPoint** | beta&nbsp;-&nbsp;**certificateRevocationListUrl** <br> v1.0&nbsp;-&nbsp;**certificateRevocationListUrl** | |
| **deltaCrlDistributionPoint** | beta&nbsp;-&nbsp;**deltaCertificateRevocationListUrl** <br> v1.0&nbsp;-&nbsp;**deltaCertificateRevocationListUrl** | |
| **trustedCertificate** | **certificado beta**&nbsp;-&nbsp; <br> v1.0&nbsp;-&nbsp;**deltaCertificateRevocationListUrl** | |
| **trustedIssuer** | **emissor beta**&nbsp;-&nbsp;<br> Emissor da v1.0&nbsp;-&nbsp; | |
| **trustedIssuerSki** | beta&nbsp;-&nbsp;**issuerSki**<br> **issuerSki** v1.0 &nbsp;-&nbsp; | |

## <a name="next-steps"></a>Próximas etapas

- Saiba mais [sobre as diferenças de](migrate-azure-ad-graph-method-differences.md) método entre Azure AD Graph e o Microsoft Graph.
- Examine a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.

