---
title: Diferenças de propriedade entre o Azure AD Graph e o Microsoft Graph
description: Descreve as diferenças de propriedade entre os recursos de gráfico do AD do Azure (entidades) e o Microsoft Graph para ajudar a migrar aplicativos adequadamente.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 006c1e42ae0530c3c50aa7e432b215a9da4c2ca4
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37622551"
---
# <a name="property-differences-between-azure-ad-graph-and-microsoft-graph"></a>Diferenças de propriedade entre o Azure AD Graph e o Microsoft Graph

Este artigo faz parte da *etapa 1: revisar as diferenças de API* do [processo de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md).

Em geral, a melhor maneira de comparar a API do Azure AD Graph com o Microsoft Graph é comparar os metadados subjacentes para cada serviço, especialmente as descrições de recursos:

- [Metadados do Azure AD Graph](https://graph.windows.net/microsoft.com/$metadata?api-version=1.6)
- [Metadados da versão beta do Microsoft Graph](https://graph.microsoft.com/beta /$metadata)
- [Metadados do Microsoft Graph v 1.0](https://graph.microsoft.comv/1.0/$metadata)

Aqui, as diferenças de propriedade entre recursos são realçadas. Se uma propriedade não é mostrada na lista, ela já está disponível na [versão v 1.0](/graph/api/overview?view=graph-rest-1.0) do Microsoft Graph, com exatamente o mesmo nome que no Azure ad Graph.

Como o usuário e o grupo são usados com frequência, estes recursos aparecem primeiro.  Outros recursos aparecem em ordem alfabética.

## <a name="user-property-differences"></a>Diferenças de Propriedade do usuário

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br>propriedade|Comentários|
|---|---|---|
| **appRoleAssignments** | versão &nbsp; - &nbsp; beta **appRoleAssignments** <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **CreationType** | versão &nbsp; - &nbsp; beta _ainda não disponível_ <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_| |
| **deletedTimestamp**| versão &nbsp; - &nbsp; beta **deleteddatetime à** <br> v 1.0 &nbsp; - &nbsp; **deleteddatetime à** | |
| **dirSyncEnabled** | versão &nbsp; - &nbsp;beta **onPremisesSyncEnabled** <br> v 1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** | |
| **facsimileTelephoneNumber** | versão &nbsp; - &nbsp; beta **fax** <br> v 1.0 &nbsp; - &nbsp; **fax** | |
| **imutávelid** | versão &nbsp; - &nbsp;beta **onPremisesImmutableId** <br> v 1.0 &nbsp; - &nbsp; **onPremisesImmutableId**  | |
| **iscomprometed** | versão &nbsp; - &nbsp; beta _não disponível_ <br> v 1.0 &nbsp; - &nbsp; _não disponível_ | A API de [proteção de identidades](/graph/api/resources/identityprotection-root?view=graph-rest-beta) do Microsoft Graph fornece funcionalidade mais sofisticada. |
| **lastDirSyncDateTime** | versão &nbsp; - &nbsp;beta **onPremisesLastSyncDateTime** <br> v 1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** | |
| **processadores** | versão &nbsp; - &nbsp; beta **mobilePhone** <br> v 1.0 &nbsp; - &nbsp; **mobilePhone** | |
| **oAuth2PermissionGrants** | versão &nbsp; - &nbsp; beta **oAuth2PermissionGrants** <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ ||
| **provisioningErrors** | versão &nbsp; - &nbsp; beta _não disponível_ <br> v 1.0 &nbsp; - &nbsp; _não disponível_ | Essa propriedade e suas informações são preteridas.  No entanto, uma nova propriedade que descreve qualquer erro de provisionamento relacionado ao AD Connect pode ser encontrada no **onPremisesProvisioningErrors** |
| **refreshTokensValidFromDateTime** | versão&nbsp;-&nbsp;beta**signinSessionsValidFromDateTime**<br>v 1.0&nbsp;-&nbsp;_ainda não está disponível_ | |
| **signinNames** | &nbsp; - &nbsp; **identidades beta/signInType** <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | Essa propriedade agora é parte do recurso [objectidentity](/graph/api/resources/objectIdentity?view=graph-rest-beta) .|
| **telephoneNumber** | versão &nbsp; - &nbsp; beta **businessPhones** <br> v 1.0 &nbsp; - &nbsp; **businessPhones** | |
| **thumbnailPhoto** | &nbsp; - &nbsp; **foto**beta, fotos <br> &nbsp; - &nbsp; **foto**v 1.0, fotos | A foto de miniatura do Azure AD não está disponível por meio do Microsoft Graph.  Em vez disso, use a [API de foto](/graph/api/resources/profilephoto?view=graph-rest-1.0) . |
| **useridentities** | &nbsp; - &nbsp; **identidades** beta <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **userState** | versão &nbsp; - &nbsp; beta **externalUserState** <br> v 1.0 &nbsp; - &nbsp; **externalUserState** | |
| **userStateChangedOn** | versão&nbsp;-&nbsp;beta**externalUserStateChangeDateTime**<br>v 1.0&nbsp;-&nbsp;**externalUserStateChangeDateTime** | |

## <a name="group-property-differences"></a>Diferenças de propriedade de grupo

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **dirSyncEnabled** | versão &nbsp; - &nbsp;beta **onPremisesSyncEnabled** <br> v 1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** | |
| **imutávelid** | versão &nbsp; - &nbsp;beta **onPremisesImmutableId** <br> v 1.0 &nbsp; - &nbsp; **onPremisesImmutableId** | |
| **lastDirSyncDateTime** | versão&nbsp;-&nbsp;beta**onPremisesLastSyncDateTime**<br>v 1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** | |
| **onPremisesDomainName** | versão &nbsp; - &nbsp; beta _ainda não disponível_ <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | Planejado, mas ainda não disponível. |
| **onPremisesNetBiosName** | versão &nbsp; - &nbsp; beta _ainda não disponível_ <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | Planejado, mas ainda não disponível. |
| **onPremisesSamAccountName** | versão &nbsp; - &nbsp; beta _ainda não disponível_ <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | Planejado, mas ainda não disponível. |
| **provisioningErrors** | versão &nbsp; - &nbsp; beta _não disponível_ <br> v 1.0 &nbsp; - &nbsp; _não disponível_ | Essa propriedade e suas informações são preteridas.  No entanto, uma nova propriedade que descreve qualquer erro de provisionamento relacionado ao AD Connect pode ser encontrada no **onPremisesProvisioningErrors** |

## <a name="application-property-differences"></a>Diferenças de propriedades do aplicativo

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **acceptMappedClaims**  | &nbsp; - &nbsp; **API beta/acceptMappedClaims** <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | acceptMappedClaims agora é parte do novo recurso de API. |
| **addIns** | versão &nbsp; - &nbsp; beta _ainda não disponível_ <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_  | |
| **applicationTemplateId** | versão &nbsp; - &nbsp; beta _ainda não disponível_ <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **availableToOtherTenants** | versão &nbsp; - &nbsp; beta **signInAudience** <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **errorUrl**| versão &nbsp; - &nbsp;beta _não disponível_ <br> v 1.0 &nbsp; - &nbsp; _não disponível_   | Essa propriedade foi preterida.|
| **homepage**| &nbsp; - &nbsp; **página inicial/Web** beta <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | homepage agora faz parte do novo recurso da Web.|
| **informationalUrls**| &nbsp; - &nbsp; **informações** beta <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **knownClientApplications**| &nbsp;-&nbsp;**API beta/knownClientApplications** <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | knownClientApplications agora é parte do novo recurso de API. |
| **logoutUrl**| &nbsp; - &nbsp; **Web Beta/logoutUrl** <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | logoutUrl agora é parte do recurso Web. |
| **logoUrl**| &nbsp; - &nbsp; **informações beta/logoUrl** <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | logoUrl agora é parte do novo recurso de informações. |
| **é**| versão &nbsp; - &nbsp;beta _não disponível_ <br> v 1.0 &nbsp; - &nbsp; _não disponível_   | Essa propriedade foi preterida.|
| **oauth2AllowIdTokenImplicitFlow** | &nbsp;-beta&nbsp;**Web/implicitGrantSettings/enableIdTokenIssuance**<br>v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | Renomeado e agora faz parte do novo recurso implicitGrantSettings. |
| **oauth2AllowImplicitFlow**| &nbsp;-&nbsp;**Web Beta/oauth2AllowImplicitFlow**<br>v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | oauth2AllowImplicitFlow agora é parte do novo recurso da Web. |
| **Oauth2allowurlpathmatching e**| versão &nbsp; - &nbsp;beta _não disponível_ <br> v 1.0 &nbsp; - &nbsp; _não disponível_   | Essa propriedade foi preterida.|
| **oauth2Permissions**| &nbsp;-&nbsp;**API beta/oauth2PermissionScopes**<br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | Renomeado e agora parte do novo recurso de API. |
| **oauth2RequirePostResponse**| versão &nbsp; - &nbsp;beta _não disponível_ <br> v 1.0 &nbsp; - &nbsp; _não disponível_   | Essa propriedade foi preterida.|
| **publicClient**| versão &nbsp; - &nbsp; beta **isFallbackPublicClient** <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | Essa propriedade agora tem um novo significado &nbsp; - &nbsp; que contém as configurações de cliente público como redirectUris. Determinando se o aplicativo é um cliente público ou confidencial, ou se não está agora pronto automaticamente, com a propriedade isFallbackPublicClient manipulando um caso especial que não pode ser determinado automaticamente.|
| **recordConsentConditions**| versão &nbsp; - &nbsp;beta _não disponível_ <br> v 1.0 &nbsp; - &nbsp; _não disponível_   | Essa propriedade foi preterida.|
| **replyUrls**| &nbsp;-&nbsp;**Web Beta/redirectUris**<br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | Além de ser renomeado, redirectUris agora faz parte do novo recurso da Web. | |
| **samlMetadataUrl**| versão &nbsp; - &nbsp; beta _ainda não disponível_  <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_  | |
| **extensãoproperties**| &nbsp; - &nbsp; **extensões** beta <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **Pontos de extremidade**|  versão &nbsp; - &nbsp; beta _não disponível_  <br> v 1.0 &nbsp; - &nbsp; _não disponível_  | Essa propriedade foi preterida, mas está planejada para o servicePrincipalName.|

## <a name="approleassignment-differences"></a>Diferenças do AppRoleAssignment

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **creationTimestamp** | versão &nbsp; - &nbsp;beta **creationTimestamp** <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | Ele será renomeado como createdDateTime.|
| **id** | versão &nbsp; - &nbsp;beta **appRoleId** <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |

## <a name="contact-property-differences"></a>Diferenças de propriedade de contato

O recurso de contato do Azure AD Graph foi renomeado como orgContact no Microsoft Graph.  Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **city** | &nbsp;-&nbsp;**endereços beta (cidade)** <br> endereços v &nbsp; - &nbsp; 1.0 **(cidade)**  | A propriedade City é parte da coleção de recursos addresses. |
| **country** | &nbsp;-&nbsp;**** endereços&nbsp;beta **(countryOrRegion)**<br> &nbsp;-&nbsp;**** endereços&nbsp;v 1.0 **(countryOrRegion)**  | A propriedade countryOrRegion é parte da coleção de recursos addresses. |
| **dirSyncEnabled** | versão &nbsp; - &nbsp;beta **onPremisesSyncEnabled** <br> v 1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled**   | |
| **facsimileTelephoneNumber** | &nbsp;-&nbsp;**** telefones&nbsp;beta **(businessFax)** <br> &nbsp; - &nbsp; **** telefones&nbsp;v 1.0 **(businessFax)** | Agora, parte da coleção Phones, que oferece suporte a Mobile, Business e businessFax. |
| **physicalDeliveryOfficeName** | versão &nbsp; - &nbsp;beta **officeLocation** <br> v 1.0 &nbsp; - &nbsp; **officeLocation** | |
| **postalCode** | &nbsp;-&nbsp;**** endereços&nbsp;beta **(PostalCode)**<br> &nbsp; - &nbsp; **** endereços&nbsp;v 1.0 **(PostalCode)** | A propriedade postalCode é parte da coleção de recursos addresses. |
| **provisioningErrors** | versão &nbsp; - &nbsp; Beta não disponível <br> v 1.0 &nbsp; - &nbsp; não disponível | Essa propriedade e suas informações são preteridas.  No entanto, uma nova propriedade que descreve qualquer erro de provisionamento relacionado ao AD Connect pode ser encontrada no **onPremisesProvisioningErrors**. Atualmente, isso só está disponível na versão beta. |
| **sipProxyAddress** |  &nbsp; - &nbsp; **imendereços** beta<br> &nbsp; - &nbsp; **endereços** v 1.0  | |
| **state** | &nbsp; - &nbsp; **** endereços&nbsp;beta **(estado)**<br> &nbsp; - &nbsp; **** endereços&nbsp;v 1.0 **(estado)**  | A propriedade State é parte da coleção de recursos addresses. |
| **streetAddress** | &nbsp; - &nbsp; **** endereços&nbsp;beta **(rua)**<br> &nbsp; - &nbsp; **** endereços&nbsp;v 1.0 **(rua)**  | A propriedade Street é parte da coleção de recursos addresses. |
| **telephoneNumber** | &nbsp;-&nbsp;**** telefones&nbsp;beta **(negócios)** <br> v 1.0 &nbsp; - &nbsp; **phones**&nbsp;**(Business)** | Agora, parte da coleção Phones, que oferece suporte a Mobile, Business e businessFax. |
| **thumbnailPhoto** | versão &nbsp; - &nbsp; _beta&nbsp;ainda&nbsp;não disponível_&nbsp;<br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |

## <a name="contract-property-differences"></a>Diferenças de propriedade de contrato

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **customerContextId** | &nbsp; - &nbsp; **CustomerID** beta <br> v 1.0 &nbsp; - &nbsp; **CustomerID**  |  |

## <a name="device-property-differences"></a>Diferenças de propriedades de dispositivos

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **approximateLastLogonTimestamp** | versão&nbsp;-&nbsp;beta**approximateLastSignInDateTime** <br> v 1.0 &nbsp; - &nbsp; **approximateLastSignInDateTime** |  |
| **complianceExpiryTime** | versão&nbsp;-&nbsp;beta**complianceExpirationDateTime** <br> v 1.0 &nbsp; - &nbsp; **complianceExpirationDateTime** |  |
| **deviceObjectVersion** |  versão&nbsp;-&nbsp;beta**deviceVersion** <br> v 1.0 &nbsp; - &nbsp; **deviceVersion** |  |
| **deviceOSType** | &nbsp;-&nbsp;**OperatingSystem** beta <br> v 1.0 &nbsp; - &nbsp; **OperatingSystem** |  |
| **deviceOSVersion** | versão&nbsp;-&nbsp;beta**operatingSystemVersion** <br> v 1.0 &nbsp; - &nbsp; **operatingSystemVersion** |  |
| **devicePhysicalIds** | versão&nbsp;-&nbsp;beta**physicalIds** <br> v 1.0 &nbsp; - &nbsp; **physicalIds** |  |
| **deviceTrustType** | &nbsp;-&nbsp;**TrustType** beta <br> v 1.0 &nbsp; - &nbsp; **TrustType** |  |
| **dirSyncEnabled** |  versão&nbsp;-&nbsp;beta**onPremisesSyncEnabled** <br> v 1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** |  |
| **lastDirSyncTime** |  versão&nbsp;-&nbsp;beta**onPremisesLastSyncDateTime** <br> v 1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** |  |

## <a name="directoryobjectreference-property-differences"></a>Diferenças da propriedade DirectoryObjectReference

O recurso directoryObjectReference do Azure AD Graph foi renomeado para directoryObjectPartnerReference no Microsoft Graph.  Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **externalContextId** | versão&nbsp;-&nbsp;beta**externalPartnerTenantId** <br> v 1.0 &nbsp; - &nbsp; **externalPartnerTenantId** |  |

## <a name="domain-property-differences"></a>Diferenças de propriedade de domínio

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **name** | &nbsp;-&nbsp;**ID** da versão beta <br> &nbsp; - &nbsp; **ID** do v 1.0 | No Microsoft Graph, o identificador exclusivo (ID) contém o nome de domínio; a `name` propriedade não existe. |
| **forceDeleteState** |  &nbsp;-&nbsp;**estado** beta <br> &nbsp; - &nbsp; **estado** v 1.0 | No gráfico do Azure AD, há forceDelete separadas e propriedades de estado do domínio.  No Microsoft Graph, todos os Estados de domínio são tratados pela propriedade State. |
| **isDefaultForCloudRedirections** | versão&nbsp;-&nbsp;_beta&nbsp;ainda&nbsp;não disponível_&nbsp;<br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |

## <a name="oauth2permissionsgrant-property-differences"></a>Diferenças da propriedade OAuth2PermissionsGrant

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **expiryTime** | versão&nbsp;-&nbsp;beta**expiryTime** <br> v 1.0&nbsp;-&nbsp;_&nbsp;ainda&nbsp;não está disponível_ | Essa propriedade não é usada e provavelmente será removida no Microsoft Graph. |
| **startTime** | versão&nbsp;-&nbsp;beta**inicial** <br> v 1.0&nbsp;-&nbsp;_&nbsp;ainda&nbsp;não está disponível_  | Essa propriedade não é usada e provavelmente será removida no Microsoft Graph. |

## <a name="policy-property-differences"></a>Diferenças de propriedade de política

Atualmente, o recurso de política no Microsoft Graph (disponível apenas na visualização) é muito semelhante ao Azure AD Graph.  No entanto, ele mudará para que haja tipos de política nomeados (como tokenIssuancePolicy ou tokenLifetimePolicy), em vez de um tipo de recurso de política genérico.

## <a name="serviceendpoint-property-differences"></a>Diferenças de Propriedade ServiceEndpoint

O recurso ServiceEndpoint do Azure AD Graph é renomeado como ponto de extremidade no Microsoft Graph.

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **função** | &nbsp;-&nbsp;**recurso** beta<br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **serviceId** | &nbsp;-&nbsp;**provedor** de versão beta<br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **serviceName** | &nbsp;-&nbsp;**ProviderName** beta<br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **resourceId** | versão&nbsp;-&nbsp;beta**providerResourceId**<br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **URI** | &nbsp;-&nbsp;**URI** beta<br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |

## <a name="serviceprincipal-property-differences"></a>Diferenças de propriedade de servicePrincipalName

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **applicationTemplateId** | versão &nbsp; - &nbsp; beta _ainda não disponível_ <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **appOwnerTenantId** | versão&nbsp;-&nbsp;beta**appOwnerOrganizationId** <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **informationalUrls**| versão&nbsp;-&nbsp;beta_ainda não disponível_ <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **preferredSingleSignOnMode** | versão&nbsp;-&nbsp;beta_ainda não disponível_ <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **preferredTokenSigningKeyEndDateTime** | versão&nbsp;-&nbsp;beta_ainda não disponível_ <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **samlSingleSignOnSettings** | versão&nbsp;-&nbsp;beta_ainda não disponível_ <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **servicePrincipalName** | versão&nbsp;-&nbsp;beta_ainda não disponível_ <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **signInAudience** | versão&nbsp;-&nbsp;beta_ainda não disponível_ <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **tokenEncryptionKeyId** | versão&nbsp;-&nbsp;beta_ainda não disponível_ <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **Pontos de extremidade** | versão&nbsp;-&nbsp;beta_ainda não disponível_ <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |

## <a name="tenantdetails-property-differences"></a>Diferenças da propriedade TenantDetails

O recurso TenantDetails do Azure AD Graph é renomeado para a organização no Microsoft Graph.  Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **companyLastDirSyncTime** | versão&nbsp;-&nbsp;beta**onPremisesLastSyncDateTime** <br> v 1.0&nbsp;-&nbsp;**onPremisesLastSyncDateTime** |  |
| **dirSyncEnabled** | versão&nbsp;-&nbsp;beta**onPremisesSyncEnabled** <br> v 1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** |  |
| **provisioningErrors** | versão&nbsp;-&nbsp;beta_não disponível_ <br> v 1.0&nbsp;-&nbsp;_não disponível_ | Essa propriedade e suas informações são preteridas.|
| **telephoneNumber** | versão&nbsp;-&nbsp;beta**businessPhones** <br> v 1.0&nbsp;-&nbsp;**businessPhones** |  |

## <a name="trustedcasforpasswordlessauth-property-differences"></a>Diferenças da propriedade TrustedCasForPasswordlessAuth

O recurso TrustedCasForPasswordlessAuth do Azure AD Graph foi renomeado como [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedauthconfiguration?view=graph-rest-beta)e só está disponível no ponto de extremidade beta do Microsoft Graph. Não há diferenças de propriedade; no entanto, há diferenças no tipo de recurso **certificateAuthority** usado pela propriedade **certificateAuthorities** .

### <a name="certificateauthorityinformation"></a>CertificateAuthorityInformation

O gráfico do Azure AD CertificateAuthorityInformation é renomeado como **certificateAuthority** no Microsoft Graph. A seguir estão as diferenças de propriedade.

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **authoritytype** | versão&nbsp;-&nbsp;beta**isRootAuthority**<br> v 1.0 &nbsp; - &nbsp; **isRootAuthority** | O tipo dessa propriedade também foi alterado em um Boolean. Anteriormente, essa propriedade deve ser definida como "RootAuthority" ou "IntermediateAuthority". A definição da nova propriedade como **true** equivale a "RootAuthority". |
| **crlDistributionPoint** | versão&nbsp;-&nbsp;beta**certificateRevocationListUrl** <br> v 1.0&nbsp;-&nbsp;**certificateRevocationListUrl** | |
| **deltaCrlDistributionPoint** | versão&nbsp;-&nbsp;beta**deltaCertificateRevocationListUrl** <br> v 1.0&nbsp;-&nbsp;**deltaCertificateRevocationListUrl** | |
| **trustedCertificate** | &nbsp;-&nbsp;**certificado** beta <br> v 1.0&nbsp;-&nbsp;**deltaCertificateRevocationListUrl** | |
| **trustedIssuer** | &nbsp;-&nbsp;**emissor** beta<br> &nbsp;-&nbsp;**emissor** de v 1.0 | |
| **trustedIssuerSki** | versão&nbsp;-&nbsp;beta**issuerSki**<br> v 1.0 &nbsp; - &nbsp; **issuerSki** | |

## <a name="next-steps"></a>Próximas etapas

- Saiba mais sobre as [diferenças de método](migrate-azure-ad-graph-method-differences.md) entre o Azure ad Graph e o Microsoft Graph.
- Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .
- Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.
