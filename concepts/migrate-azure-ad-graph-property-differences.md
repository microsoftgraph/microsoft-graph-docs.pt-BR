---
title: Diferenças de propriedade entre o Azure AD Graph e o Microsoft Graph
description: Descreve as diferenças de propriedade entre os recursos de gráfico do AD do Azure (entidades) e o Microsoft Graph para ajudar a migrar aplicativos adequadamente.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e2f8ba237cd86ab2361c98f5b51afaa77d2b7f50
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630213"
---
# <a name="property-differences-between-azure-ad-graph-and-microsoft-graph"></a>Diferenças de propriedade entre o Azure AD Graph e o Microsoft Graph

Este artigo faz parte da *etapa 1:* revisar as diferenças de API do [processo de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md).

Em geral, a melhor maneira de comparar a API do Azure AD Graph com o Microsoft Graph é comparar os metadados subjacentes para cada serviço, especialmente as descrições de recursos:

- [Metadados do Azure AD Graph](https://graph.windows.net/microsoft.com/$metadata?api-version=1.6)
- [Metadados da versão beta do Microsoft Graph](https://graph.microsoft.com/beta /$metadata)
- [Metadados do Microsoft Graph v 1.0](https://graph.microsoft.comv/1.0/$metadata)

Aqui, as diferenças de propriedade entre recursos são realçadas. Se uma propriedade não é mostrada na lista, ela já está disponível na [versão v 1.0](/graph/api/overview?view=graph-rest-1.0) do Microsoft Graph, com exatamente o mesmo nome que no Azure ad Graph.

Como o usuário e o grupo são usados com frequência, estes recursos aparecem primeiro.  Outros recursos aparecem em ordem alfabética.

## <a name="user-property-differences"></a>Diferenças de Propriedade do usuário

|Gráfico do Azure AD <br>(v 1.6) Propriedade |Microsoft Graph<br>propriedade|Comments|
|---|---|---|
| **appRoleAssignments** | Beta- **appRoleAssignments** <br> v 1.0- _ainda não disponível_ | |
| **CreationType** | Beta- _ainda não disponível_ <br> v 1.0- _ainda não disponível_| |
| **deletedTimestamp**| Beta- **deleteddatetime à** <br> v 1.0- **deleteddatetime à** | |
| **dirSyncEnabled** | versão &nbsp; - &nbsp;beta **onPremisesSyncEnabled** <br> v 1.0- **onPremisesSyncEnabled** | |
| **facsimileTelephoneNumber** | Beta- **fax** <br> v 1.0- **fax** | |
| **imutávelid** | versão &nbsp; - &nbsp;beta **onPremisesImmutableId** <br> v 1.0- **onPremisesImmutableId**  | |
| **iscomprometed** | Beta- _não disponível_ <br> v 1.0- _não disponível_ | A API de [proteção](/graph/api/resources/identityprotection-root?view=graph-rest-beta) de identidades do Microsoft Graph fornece funcionalidade mais sofisticada. |
| **lastDirSyncDateTime** | versão &nbsp; - &nbsp;beta **onPremisesLastSyncDateTime** <br> v 1.0- **onPremisesLastSyncDateTime** | |
| **processadores** | Beta- **mobilePhone** <br> v 1.0- **mobilePhone** | |
| **oAuth2PermissionGrants** | Beta- **oAuth2PermissionGrants** <br> v 1.0- _ainda não disponível_ ||
| **provisioningErrors** | versão &nbsp; - &nbsp;beta **onPremisesProvisioningErrors** <br> v 1.0- **onPremisesProvisioningErrors** | |
| **refreshTokensValidFromDateTime** | versão&nbsp;-&nbsp;beta**signinSessionsValidFromDateTime**<br>v 1.0&nbsp;-&nbsp;_ainda não está disponível_ | |
| **signinNames** | Beta- _ainda não disponível_ <br> v 1.0- _ainda não disponível_ | |
| **telephoneNumber** | Beta- **businessPhones** <br> v 1.0- **businessPhones** | |
| **thumbnailPhoto** | Beta- **foto**, fotos <br> v 1.0- **foto**, fotos | A foto de miniatura do Azure AD não está disponível por meio do Microsoft Graph.  Em vez disso, use a [API de foto](/graph/api/resources/profilephoto?view=graph-rest-1.0) . |
| **useridentities** | Beta- _ainda não disponível_ <br> v 1.0- _ainda não disponível_ | |
| **userState** | Beta- **externalUserState** <br> v 1.0- **externalUserState** | |
| **userStateChangedOn** | versão&nbsp;-&nbsp;beta**externalUserStateChangeDateTime**<br>v 1.0&nbsp;-&nbsp;**externalUserStateChangeDateTime** | |

## <a name="group-property-differences"></a>Diferenças de propriedade de grupo

|Gráfico do Azure AD <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comments|
|---|---|---|
| **dirSyncEnabled** | versão &nbsp; - &nbsp;beta **onPremisesSyncEnabled** <br> v 1.0- **onPremisesSyncEnabled** | |
| **imutávelid** | versão &nbsp; - &nbsp;beta **onPremisesImmutableId** <br> v 1.0- **onPremisesImmutableId** | |
| **lastDirSyncDateTime** | versão&nbsp;-&nbsp;beta**onPremisesLastSyncDateTime**<br>v 1.0- **onPremisesLastSyncDateTime** | |
| **onPremisesDomainName** | Beta- _ainda não disponível_ <br> v 1.0- _ainda não disponível_ | Planejado, mas ainda não disponível. |
| **onPremisesNetBiosName** | Beta- _ainda não disponível_ <br> v 1.0- _ainda não disponível_ | Planejado, mas ainda não disponível. |
| **onPremisesSamAccountName** | Beta- _ainda não disponível_ <br> v 1.0- _ainda não disponível_ | Planejado, mas ainda não disponível. |
| **provisioningErrors** | versão&nbsp;-&nbsp;beta**onPremisesProvisioningErrors**<br> v 1.0- **onPremisesProvisioningErrors** | |

## <a name="application-property-differences"></a>Diferenças de propriedades do aplicativo

|Gráfico do Azure AD <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comments|
|---|---|---|
| **acceptMappedClaims**  | &nbsp; - &nbsp; **API beta/acceptMappedClaims** <br> v 1.0- _ainda não disponível_ | acceptMappedClaims agora é parte do novo recurso de API. |
| **addIns** | Beta- _ainda não disponível_ <br> v 1.0- _ainda não disponível_  | |
| **applicationTemplateId** | Beta- _ainda não disponível_ <br> v 1.0- _ainda não disponível_ | |
| **availableToOtherTenants** | versão &nbsp; - &nbsp; beta **agora** <br> v 1.0- _ainda não disponível_ | |
| **errorUrl**| versão &nbsp; - &nbsp;beta _não disponível_ <br> v 1.0- _não disponível_ | Essa propriedade foi preterida.|
| **homepage**| &nbsp; - &nbsp; **página inicial/Web** beta <br> v 1.0- _ainda não disponível_ | homepage agora faz parte do novo recurso da Web.|
| **informationalUrls**| &nbsp; - &nbsp; **informações** beta <br> v 1.0- _ainda não disponível_ | |
| **knownClientApplications**| &nbsp;-&nbsp;**API beta/knownClientApplications** <br> v 1.0- _ainda não disponível_ | knownClientApplications agora é parte do novo recurso de API. |
| **logoutUrl**| &nbsp; - &nbsp; **Web Beta/logoutUrl** <br> v 1.0- _ainda não disponível_ | logoutUrl agora é parte do recurso Web. |
| **logoUrl**| &nbsp; - &nbsp; **informações beta/logoUrl** <br> v 1.0- _ainda não disponível_ | logoUrl agora é parte do novo recurso de informações. |
| **é**| versão &nbsp; - &nbsp;beta _não disponível_ <br> v 1.0- _não disponível_ | Essa propriedade foi preterida.|
| **oauth2AllowIdTokenImplicitFlow** | &nbsp;-beta&nbsp;**Web/implicitGrantSettings/enableIdTokenIssuance**<br>v 1.0- _ainda não disponível_ | Renomeado e agora faz parte do novo recurso implicitGrantSettings. |
| **oauth2AllowImplicitFlow**| &nbsp;-&nbsp;**Web Beta/oauth2AllowImplicitFlow**<br>v 1.0- _ainda não disponível_ | oauth2AllowImplicitFlow agora é parte do novo recurso da Web. |
| **Oauth2allowurlpathmatching e**| versão &nbsp; - &nbsp;beta _não disponível_ <br> v 1.0- _não disponível_ | Essa propriedade foi preterida.|
| **oauth2Permissions**| &nbsp;-&nbsp;**API beta/oauth2PermissionScopes**<br> v 1.0- _ainda não disponível_ | Renomeado e agora parte do novo recurso de API. |
| **oauth2RequirePostResponse**| versão &nbsp; - &nbsp;beta _não disponível_ <br> v 1.0- _não disponível_ | Essa propriedade foi preterida.|
| **publicClient**| versão &nbsp; - &nbsp; beta **isFallbackPublicClient** <br> v 1.0- _ainda não disponível_ | Essa propriedade agora tem um novo significado, que contém as configurações de cliente público como redirectUris. Determinando se o aplicativo é um cliente público ou confidencial, ou se não está agora pronto automaticamente, com a propriedade isFallbackPublicClient manipulando um caso especial que não pode ser determinado automaticamente.|
| **recordConsentConditions**| versão &nbsp; - &nbsp;beta _não disponível_ <br> v 1.0- _não disponível_ | Essa propriedade foi preterida.|
| **replyUrls**| &nbsp;-&nbsp;**Web Beta/redirectUris**<br> v 1.0- _ainda não disponível_ | Além de ser renomeado, redirectUris agora faz parte do novo recurso da Web. | |
| **samlMetadataUrl**| Beta- _ainda não disponível_  <br> v 1.0- _ainda não disponível_  | |
| **extensãoproperties**| &nbsp; - &nbsp; **extensões** beta <br> v 1.0- _ainda não disponível_ | Essa propriedade foi preterida. |
| **Pontos de extremidade**|  Beta- _ainda não disponível_  <br> v 1.0- _ainda não disponível_  | |

## <a name="approleassignment-differences"></a>Diferenças do AppRoleAssignment

|Gráfico do Azure AD <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comments|
|---|---|---|
| **creationTimestamp** | versão &nbsp; - &nbsp;beta **creationTimestamp** <br> v 1.0- _ainda não disponível_ | Ele será renomeado como createdDateTime.|
| **id** | versão &nbsp; - &nbsp;beta **appRoleId** <br> v 1.0- _ainda não disponível_ | |

## <a name="contact-property-differences"></a>Diferenças de propriedade de contato

O recurso de contato do Azure AD Graph foi renomeado como orgContact no Microsoft Graph.  Aqui estão as diferenças de propriedade:

|Gráfico do Azure AD <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comments|
|---|---|---|
| **city** | &nbsp;-&nbsp;**endereços beta (cidade)** <br> v 1.0- _ainda não disponível_  | A propriedade City é parte da coleção de recursos addresses. |
| **country** | &nbsp;-&nbsp;**** endereços&nbsp;beta **(countryOrRegion)**<br> v 1.0- _ainda não disponível_  | A propriedade countryOrRegion é parte da coleção de recursos addresses. |
| **dirSyncEnabled** | versão &nbsp; - &nbsp;beta **onPremisesSyncEnabled** <br> v 1.0- _ainda não disponível_  | |
| **facsimileTelephoneNumber** | &nbsp;-&nbsp;**** telefones&nbsp;beta **(businessFax)** <br> v 1.0- _ainda não disponível_ | Agora, parte da coleção Phones, que oferece suporte a Mobile, Business e businessFax. |
| **physicalDeliveryOfficeName** | versão &nbsp; - &nbsp;beta **officeLocation** <br> v 1.0- **officeLocation** | |
| **postalCode** | &nbsp;-&nbsp;**** endereços&nbsp;beta **(PostalCode)**<br> v 1.0- _ainda não disponível_  | A propriedade postalCode é parte da coleção de recursos addresses. |
| **provisioningErrors** | versão&nbsp;-&nbsp;beta**onPremisesProvisioningErrors**<br> v 1.0- _ainda não disponível_  | |
| **sipProxyAddress** |  &nbsp; - &nbsp; **** imendereços beta<br> v 1.0- _ainda não disponível_  | |
| **state** | &nbsp; - &nbsp; **** endereços&nbsp;beta **(estado)**<br> v 1.0- _ainda não disponível_  | A propriedade State é parte da coleção de recursos addresses. |
| **streetAddress** | &nbsp; - &nbsp; **** endereços&nbsp;beta **(rua)**<br> v 1.0- _ainda não disponível_  | A propriedade Street é parte da coleção de recursos addresses. |
| **telephoneNumber** | &nbsp;-&nbsp;**** telefones&nbsp;beta **(negócios)** <br> v 1.0- _ainda não disponível_ | Agora, parte da coleção Phones, que oferece suporte a Mobile, Business e businessFax. |
| **thumbnailPhoto** | versão &nbsp; - &nbsp; _beta&nbsp;ainda&nbsp;não disponível_&nbsp;<br> v 1.0- _ainda não disponível_ | |

## <a name="contract-property-differences"></a>Diferenças de propriedade de contrato

|Gráfico do Azure AD <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comments|
|---|---|---|
| **customerContextId** | &nbsp; - &nbsp; **CustomerID** beta <br> v 1.0- **CustomerID**  |  |

## <a name="device-property-differences"></a>Diferenças de propriedades de dispositivos

|Gráfico do Azure AD <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comments|
|---|---|---|
| **approximateLastLogonTimestamp** | versão&nbsp;-&nbsp;beta**approximateLastSignInDateTime** <br> v 1.0- **approximateLastSignInDateTime** |  |
| **complianceExpiryTime** | versão&nbsp;-&nbsp;beta**complianceExpirationDateTime** <br> v 1.0- **complianceExpirationDateTime** |  |
| **deviceObjectVersion** |  versão&nbsp;-&nbsp;beta**deviceVersion** <br> v 1.0- **deviceVersion** |  |
| **deviceOSType** | &nbsp;-&nbsp;**OperatingSystem** beta <br> v 1.0- **OperatingSystem** |  |
| **deviceOSVersion** | versão&nbsp;-&nbsp;beta**operatingSystemVersion** <br> v 1.0- **operatingSystemVersion** |  |
| **devicePhysicalIds** | versão&nbsp;-&nbsp;beta**physicalIds** <br> v 1.0- **physicalIds** |  |
| **deviceTrustType** | &nbsp;-&nbsp;**TrustType** beta <br> v 1.0- **TrustType** |  |
| **dirSyncEnabled** |  versão&nbsp;-&nbsp;beta**onPremisesSyncEnabled** <br> v 1.0- **onPremisesSyncEnabled** |  |
| **lastDirSyncTime** |  versão&nbsp;-&nbsp;beta**onPremisesLastSyncDateTime** <br> v 1.0- **onPremisesLastSyncDateTime** |  |

## <a name="directoryobjectreference-property-differences"></a>Diferenças da propriedade DirectoryObjectReference

O recurso directoryObjectReference do Azure AD Graph foi renomeado para directoryObjectPartnerReference no Microsoft Graph.  Aqui estão as diferenças de propriedade:

|Gráfico do Azure AD <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comments|
|---|---|---|
| **externalContextId** | versão&nbsp;-&nbsp;beta**externalPartnerTenantId** <br> v 1.0- **externalPartnerTenantId** |  |

## <a name="domain-property-differences"></a>Diferenças de propriedade de domínio

|Gráfico do Azure AD <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comments|
|---|---|---|
| **name** | &nbsp;-&nbsp;**ID** da versão beta <br> v 1.0- **ID** | No Microsoft Graph, o identificador exclusivo (ID) contém o nome de domínio; a `name` propriedade não existe. |
| **forceDeleteState** |  &nbsp;-&nbsp;**estado** beta <br> v 1.0- **estado** | No gráfico do Azure AD, há forceDelete separadas e propriedades de estado do domínio.  No Microsoft Graph, todos os Estados de domínio são tratados pela propriedade State. |
| **isDefaultForCloudRedirections** | versão&nbsp;-&nbsp;_beta&nbsp;ainda&nbsp;não disponível_&nbsp;<br> v 1.0- _ainda não disponível_ | |

## <a name="oauth2permissionsgrant-property-differences"></a>Diferenças da propriedade OAuth2PermissionsGrant

|Gráfico do Azure AD <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comments|
|---|---|---|
| **expiryTime** | versão&nbsp;-&nbsp;beta**expiryTime** <br> v 1.0&nbsp;-&nbsp;_&nbsp;ainda&nbsp;não está disponível_ | Essa propriedade não é usada e provavelmente será removida no Microsoft Graph. |
| **startTime** | versão&nbsp;-&nbsp;beta**inicial** <br> v 1.0&nbsp;-&nbsp;_&nbsp;ainda&nbsp;não está disponível_  | Essa propriedade não é usada e provavelmente será removida no Microsoft Graph. |

## <a name="policy-property-differences"></a>Diferenças de propriedade de política

Atualmente, o recurso de política no Microsoft Graph (disponível apenas na visualização) é muito semelhante ao Azure AD Graph.  No entanto, ele mudará para que haja tipos de política nomeados (como tokenIssuancePolicy ou tokenLifetimePolicy), em vez de um tipo de recurso de política genérico.

## <a name="serviceendpoint-property-differences"></a>Diferenças de Propriedade ServiceEndpoint

O recurso ServiceEndpoint do Azure AD Graph é renomeado como ponto de extremidade no Microsoft Graph.

|Gráfico do Azure AD <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comments|
|---|---|---|
| **função** | &nbsp;-&nbsp;**recurso** beta<br> v 1.0- _ainda não disponível_ | |
| **serviceId** | &nbsp;-&nbsp;**provedor** de versão beta<br> v 1.0- _ainda não disponível_ | |
| **serviceName** | &nbsp;-&nbsp;**ProviderName** beta<br> v 1.0- _ainda não disponível_ | |
| **resourceId** | versão&nbsp;-&nbsp;beta**providerResourceId**<br> v 1.0- _ainda não disponível_ | |
| **URI** | &nbsp;-&nbsp;**URI** beta<br> v 1.0- _ainda não disponível_ | |

## <a name="serviceprincipal-property-differences"></a>Diferenças de propriedade de servicePrincipalName

|Gráfico do Azure AD <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comments|
|---|---|---|
| **applicationTemplateId** | Beta- _ainda não disponível_ <br> v 1.0- _ainda não disponível_ | |
| **appOwnerTenantId** | versão&nbsp;-&nbsp;beta**appOwnerOrganizationId** <br> v 1.0- _ainda não disponível_ | |
| **informationalUrls**| versão&nbsp;-&nbsp;beta_ainda não disponível_ <br> v 1.0- _ainda não disponível_ | |
| **preferredSingleSignOnMode** | versão&nbsp;-&nbsp;beta_ainda não disponível_ <br> v 1.0- _ainda não disponível_ | |
| **preferredTokenSigningKeyEndDateTime** | versão&nbsp;-&nbsp;beta_ainda não disponível_ <br> v 1.0- _ainda não disponível_ | |
| **samlSingleSignOnSettings** | versão&nbsp;-&nbsp;beta_ainda não disponível_ <br> v 1.0- _ainda não disponível_ | |
| **servicePrincipalName** | versão&nbsp;-&nbsp;beta_ainda não disponível_ <br> v 1.0- _ainda não disponível_ | |
| **signInAudience** | versão&nbsp;-&nbsp;beta_ainda não disponível_ <br> v 1.0- _ainda não disponível_ | |
| **tokenEncryptionKeyId** | versão&nbsp;-&nbsp;beta_ainda não disponível_ <br> v 1.0- _ainda não disponível_ | |
| **Pontos de extremidade** | versão&nbsp;-&nbsp;beta_ainda não disponível_ <br> v 1.0- _ainda não disponível_ | |

## <a name="tenantdetails-property-differences"></a>Diferenças da propriedade TenantDetails

O recurso TenantDetails do Azure AD Graph é renomeado para a organização no Microsoft Graph.  Aqui estão as diferenças de propriedade:

|Gráfico do Azure AD <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comments|
|---|---|---|
| **companyLastDirSyncTime** | versão&nbsp;-&nbsp;beta**onPremisesLastSyncDateTime** <br>v 1.0- **onPremisesLastSyncDateTime** |  |
| **dirSyncEnabled** | versão&nbsp;-&nbsp;beta**onPremisesSyncEnabled** <br> v 1.0- **onPremisesSyncEnabled** |  |
| **provisoningErrors** | versão&nbsp;-&nbsp;_beta&nbsp;ainda&nbsp;não disponível_<br> v 1.0- _ainda não disponível_ | |
| **telephoneNumber** | versão&nbsp;-&nbsp;beta**businessPhones** <br> v 1.0- **businessPhones** |  |

## <a name="trustedcasforpasswordlessauth-property-differences"></a>Diferenças da propriedade TrustedCasForPasswordlessAuth

O recurso TrustedCasForPasswordlessAuth do Azure AD Graph foi renomeado para certificateBasedAuthConfiguration no Microsoft Graph.  Não há diferenças de propriedade.

## <a name="next-steps"></a>Próximos passos

- Saiba mais sobre as [diferenças de método](migrate-azure-ad-graph-method-differences.md) entre o Azure ad Graph e o Microsoft Graph.
- Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .
- Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.
