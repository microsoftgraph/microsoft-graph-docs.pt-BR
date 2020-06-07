---
title: Diferenças de propriedade entre o Azure AD Graph e o Microsoft Graph
description: Descreve as diferenças de propriedade entre os recursos de gráfico do AD do Azure (entidades) e o Microsoft Graph para ajudar a migrar aplicativos adequadamente.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 401d6391f68a756d9d5ac7a2176b8ff9d5c7b7eb
ms.sourcegitcommit: 53a57f19a5b16029b540e61ddfba6c2b4e45cfc5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2020
ms.locfileid: "44593636"
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
| **deletedTimestamp**| versão beta &nbsp; - &nbsp; **deleteddatetime à** <br> v 1.0 &nbsp; - &nbsp; **deleteddatetime à** | |
| **dirSyncEnabled** | versão beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v 1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** | |
| **facsimileTelephoneNumber** | versão beta &nbsp; - &nbsp; **fax** <br> v 1.0 &nbsp; - &nbsp; **fax** | |
| **imutávelid** | versão beta &nbsp; - &nbsp; **onPremisesImmutableId** <br> v 1.0 &nbsp; - &nbsp; **onPremisesImmutableId**  | |
| **iscomprometed** | versão beta &nbsp; - &nbsp; _não disponível_ <br> v 1.0 &nbsp; - &nbsp; _não disponível_ | A API de [proteção de identidades](/graph/api/resources/identityprotection-root?view=graph-rest-beta) do Microsoft Graph fornece funcionalidade mais sofisticada. |
| **lastDirSyncDateTime** | versão beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime** <br> v 1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** | |
| **processadores** | versão beta &nbsp; - &nbsp; **mobilePhone** <br> v 1.0 &nbsp; - &nbsp; **mobilePhone** | |
| **provisioningErrors** | versão beta &nbsp; - &nbsp; _não disponível_ <br> v 1.0 &nbsp; - &nbsp; _não disponível_ | Essa propriedade e suas informações são preteridas.  No entanto, uma nova propriedade que descreve qualquer erro de provisionamento relacionado ao AD Connect pode ser encontrada no **onPremisesProvisioningErrors** |
| **refreshTokensValidFromDateTime** | versão beta &nbsp; - &nbsp; **signinSessionsValidFromDateTime**<br>v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **signinNames** | &nbsp; - &nbsp; **identidades beta/signInType** <br> v 1.0 &nbsp; - &nbsp; **Identities/signInType** | Essa propriedade agora é parte do recurso [objectidentity](/graph/api/resources/objectIdentity?view=graph-rest-1.0) .|
| **telephoneNumber** | versão beta &nbsp; - &nbsp; **businessPhones** <br> v 1.0 &nbsp; - &nbsp; **businessPhones** | |
| **thumbnailPhoto** | &nbsp; - &nbsp; **foto**beta, fotos <br> foto v 1.0 &nbsp; - &nbsp; **photo**, fotos | A foto de miniatura do Azure AD não está disponível por meio do Microsoft Graph.  Em vez disso, use a [API de foto](/graph/api/resources/profilephoto?view=graph-rest-1.0) . |
| **useridentities** | &nbsp; - &nbsp; **identidades** beta <br> &nbsp; - &nbsp; **identidades** v 1.0 | Confira o tipo de recurso [objectidentity](/graph/api/resources/objectIdentity?view=graph-rest-1.0) para obter mais detalhes.|
| **userState** | versão beta &nbsp; - &nbsp; **externalUserState** <br> v 1.0 &nbsp; - &nbsp; **externalUserState** | |
| **userStateChangedOn** | versão beta &nbsp; - &nbsp; **externalUserStateChangeDateTime**<br>v 1.0 &nbsp; - &nbsp; **externalUserStateChangeDateTime** | |

## <a name="group-property-differences"></a>Diferenças de propriedade de grupo

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **dirSyncEnabled** | versão beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v 1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** | |
| **imutávelid** | versão beta &nbsp; - &nbsp; **onPremisesImmutableId** <br> v 1.0 &nbsp; - &nbsp; **onPremisesImmutableId** | |
| **lastDirSyncDateTime** | versão beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime**<br>v 1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** | |
| **onPremisesDomainName** | versão beta &nbsp; - &nbsp; onPremisesDomainName <br> v 1.0 &nbsp; - &nbsp; onPremisesDomainName | |
| **onPremisesNetBiosName** | versão beta &nbsp; - &nbsp; onPremisesNetBiosName <br> v 1.0 &nbsp; - &nbsp; onPremisesNetBiosName | |
| **onPremisesSamAccountName** | versão beta &nbsp; - &nbsp; onPremisesSamAccountName <br> v 1.0 &nbsp; - &nbsp; onPremisesSamAccountName |  |
| **provisioningErrors** | versão beta &nbsp; - &nbsp; _não disponível_ <br> v 1.0 &nbsp; - &nbsp; _não disponível_ | Essa propriedade e suas informações são preteridas.  No entanto, uma nova propriedade que descreve qualquer erro de provisionamento relacionado ao AD Connect pode ser encontrada no **onPremisesProvisioningErrors** |

## <a name="application-property-differences"></a>Diferenças de propriedades do aplicativo

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **acceptMappedClaims**  | &nbsp; - &nbsp; **API beta/acceptMappedClaims** <br> v 1.0 &nbsp; - &nbsp; **API/acceptMappedClaims** | acceptMappedClaims agora é parte do novo recurso de API. |
| **availableToOtherTenants** | versão beta &nbsp; - &nbsp; **signInAudience** <br> v 1.0 &nbsp; - &nbsp; **signInAudience** | |
| **errorUrl**| versão beta &nbsp; - &nbsp; _não disponível_ <br> v 1.0 &nbsp; - &nbsp; _não disponível_   | Essa propriedade foi preterida.|
| **Home Page**| &nbsp; - &nbsp; **Web Beta/homePageUrl** <br> v 1.0 &nbsp; - &nbsp; **Web/homePageUrl** | homepage agora faz parte do novo recurso da Web.|
| **informationalUrls**| &nbsp; - &nbsp; **informações** beta <br> &nbsp; - &nbsp; **informações sobre** o v 1.0 | |
| **knownClientApplications**| &nbsp; - &nbsp; **API beta/knownClientApplications** <br> v 1.0 &nbsp; - &nbsp; **API/knownClientApplications** | knownClientApplications agora é parte do novo recurso de API. |
| **logoutUrl**| &nbsp; - &nbsp; **Web Beta/logoutUrl** <br> v 1.0 &nbsp; - &nbsp; **Web/logoutUrl** | logoutUrl agora é parte do recurso Web. |
| **logoUrl**| &nbsp; - &nbsp; **informações beta/logoUrl** <br> v 1.0 &nbsp; - &nbsp; **info/logoUrl** | logoUrl agora é parte do novo recurso de informações. |
| **é**| &nbsp; - &nbsp; **logotipo** beta <br> &nbsp; - &nbsp; **logotipo** v 1.0   | |
| **oauth2AllowIdTokenImplicitFlow** | Beta &nbsp; - &nbsp; **Web/implicitGrantSettings/enableIdTokenIssuance**<br>v 1.0 &nbsp; - &nbsp; **Web/implicitGrantSettings/enableIdTokenIssuance** | Renomeado e agora faz parte do novo recurso implicitGrantSettings. |
| **oauth2AllowImplicitFlow**| Beta &nbsp; - &nbsp; **Web/implicitGrantSettings/enableAccessTokenIssuance**<br>v 1.0 &nbsp; - &nbsp; **Web/implicitGrantSettings/enableAccessTokenIssuance** | Renomeado e agora faz parte do novo recurso implicitGrantSettings. |
| **Oauth2allowurlpathmatching e**| versão beta &nbsp; - &nbsp; _não disponível_ <br> v 1.0 &nbsp; - &nbsp; _não disponível_   | Essa propriedade foi preterida.|
| **oauth2Permissions**| &nbsp; - &nbsp; **API beta/oauth2PermissionScopes**<br> v 1.0 &nbsp; - &nbsp; **API/oauth2PermissionScopes** | Renomeado e agora parte do novo recurso de API. |
| **publicClient**| versão beta &nbsp; - &nbsp; **isFallbackPublicClient** <br> v 1.0 &nbsp; - &nbsp; **isFallbackPublicClient** | Essa propriedade agora tem um novo significado &nbsp; - &nbsp; que contém as configurações de cliente público como redirectUris. Determinando se o aplicativo é um cliente público ou confidencial, ou se não está agora pronto automaticamente, com a propriedade isFallbackPublicClient manipulando um caso especial que não pode ser determinado automaticamente.|
| **recordConsentConditions**| versão beta &nbsp; - &nbsp; _não disponível_ <br> v 1.0 &nbsp; - &nbsp; _não disponível_   | Essa propriedade foi preterida.|
| **replyUrls**| Beta &nbsp; - &nbsp; **Web/redirectUris**, **publicClient/redirectUris**<br> v 1.0 &nbsp; - &nbsp; **Web/redirectUris**, **publicClient/redirectUris** | Além de ser renomeado, o redirectUris agora faz parte dos novos recursos da Web e do publicClient. Isso permite que os desenvolvedores usem URIs específicos para seus clientes Web e públicos (como um aplicativo instalado em um dispositivo de área de trabalho). | |
| **samlMetadataUrl**| versão beta &nbsp; - &nbsp; _ainda não disponível_  <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_  | |
| **Pontos de extremidade**|  versão beta &nbsp; - &nbsp; _não disponível_  <br> v 1.0 &nbsp; - &nbsp; _não disponível_  | Essa propriedade foi preterida, mas está planejada para o servicePrincipalName.|

## <a name="approleassignment-differences"></a>Diferenças do AppRoleAssignment

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **creationTimestamp** | versão beta &nbsp; - &nbsp; **creationTimestamp** <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | Ele será renomeado como createdDateTime.|
| **id** | versão beta &nbsp; - &nbsp; **appRoleId** <br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |

## <a name="contact-property-differences"></a>Diferenças de propriedade de contato

O recurso de contato do Azure AD Graph foi renomeado como orgContact no Microsoft Graph.  Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **city** | &nbsp; - &nbsp; **endereços beta (cidade)** <br> endereços v 1.0 &nbsp; - &nbsp; **(cidade)**  | A propriedade City é parte da coleção de recursos addresses. |
| **países** | &nbsp; - &nbsp; **endereços**beta &nbsp; **(countryOrRegion)**<br> endereços v 1.0 &nbsp; - &nbsp; **addresses** &nbsp; **(countryOrRegion)**  | A propriedade countryOrRegion é parte da coleção de recursos addresses. |
| **dirSyncEnabled** | versão beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v 1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled**   | |
| **facsimileTelephoneNumber** | &nbsp; - &nbsp; **telefones**beta &nbsp; **(businessFax)** <br> telefones v 1.0 &nbsp; - &nbsp; **phones** &nbsp; **(businessFax)** | Agora, parte da coleção Phones, que oferece suporte a Mobile, Business e businessFax. |
| **physicalDeliveryOfficeName** | versão beta &nbsp; - &nbsp; **officeLocation** <br> v 1.0 &nbsp; - &nbsp; **officeLocation** | |
| **postalCode** | &nbsp; - &nbsp; **endereços**beta &nbsp; **(PostalCode)**<br> endereços v 1.0 &nbsp; - &nbsp; **addresses** &nbsp; **(PostalCode)** | A propriedade postalCode é parte da coleção de recursos addresses. |
| **provisioningErrors** | versão beta &nbsp; - &nbsp; não disponível <br> v 1.0 &nbsp; - &nbsp; não disponível | Essa propriedade e suas informações são preteridas.  No entanto, uma nova propriedade que descreve qualquer erro de provisionamento relacionado ao AD Connect pode ser encontrada no **onPremisesProvisioningErrors**. Atualmente, isso só está disponível na versão beta. |
| **sipProxyAddress** |  &nbsp; - &nbsp; **imendereços** beta<br> &nbsp; - &nbsp; **endereços** v 1.0  | |
| **state** | &nbsp; - &nbsp; **endereços**beta &nbsp; **(estado)**<br> endereços v 1.0 &nbsp; - &nbsp; **addresses** &nbsp; **(estado)**  | A propriedade State é parte da coleção de recursos addresses. |
| **streetAddress** | &nbsp; - &nbsp; **endereços**beta &nbsp; **(rua)**<br> endereços v 1.0 &nbsp; - &nbsp; **addresses** &nbsp; **(rua)**  | A propriedade Street é parte da coleção de recursos addresses. |
| **telephoneNumber** | &nbsp; - &nbsp; **telefones**beta &nbsp; **(negócios)** <br> v 1.0 &nbsp; - &nbsp; **phones** &nbsp; **(Business)** | Agora, parte da coleção Phones, que oferece suporte a Mobile, Business e businessFax. |
| **thumbnailPhoto** | versão beta &nbsp; - &nbsp; _ &nbsp; ainda não &nbsp; disponível_&nbsp;<br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |

## <a name="contract-property-differences"></a>Diferenças de propriedade de contrato

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **customerContextId** | &nbsp; - &nbsp; **CustomerID** beta <br> v 1.0 &nbsp; - &nbsp; **CustomerID**  |  |

## <a name="device-property-differences"></a>Diferenças de propriedades de dispositivos

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **approximateLastLogonTimestamp** | versão beta &nbsp; - &nbsp; **approximateLastSignInDateTime** <br> v 1.0 &nbsp; - &nbsp; **approximateLastSignInDateTime** |  |
| **complianceExpiryTime** | versão beta &nbsp; - &nbsp; **complianceExpirationDateTime** <br> v 1.0 &nbsp; - &nbsp; **complianceExpirationDateTime** |  |
| **deviceObjectVersion** |  versão beta &nbsp; - &nbsp; **deviceVersion** <br> v 1.0 &nbsp; - &nbsp; **deviceVersion** |  |
| **deviceOSType** | &nbsp; - &nbsp; **OperatingSystem** beta <br> v 1.0 &nbsp; - &nbsp; **OperatingSystem** |  |
| **deviceOSVersion** | versão beta &nbsp; - &nbsp; **operatingSystemVersion** <br> v 1.0 &nbsp; - &nbsp; **operatingSystemVersion** |  |
| **devicePhysicalIds** | versão beta &nbsp; - &nbsp; **physicalIds** <br> v 1.0 &nbsp; - &nbsp; **physicalIds** |  |
| **deviceTrustType** | &nbsp; - &nbsp; **TrustType** beta <br> v 1.0 &nbsp; - &nbsp; **TrustType** |  |
| **dirSyncEnabled** |  versão beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v 1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** |  |
| **lastDirSyncTime** |  versão beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime** <br> v 1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** |  |

## <a name="directoryobjectreference-property-differences"></a>Diferenças da propriedade DirectoryObjectReference

O recurso directoryObjectReference do Azure AD Graph foi renomeado para directoryObjectPartnerReference no Microsoft Graph.  Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **externalContextId** | versão beta &nbsp; - &nbsp; **externalPartnerTenantId** <br> v 1.0 &nbsp; - &nbsp; **externalPartnerTenantId** |  |

## <a name="domain-property-differences"></a>Diferenças de propriedade de domínio

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **name** | &nbsp; - &nbsp; **ID** da versão beta <br> &nbsp; - &nbsp; **ID** do v 1.0 | No Microsoft Graph, o identificador exclusivo (ID) contém o nome de domínio; a `name` propriedade não existe. |
| **forceDeleteState** |  &nbsp; - &nbsp; **estado** beta <br> &nbsp; - &nbsp; **estado** v 1.0 | No gráfico do Azure AD, há forceDelete separadas e propriedades de estado do domínio.  No Microsoft Graph, todos os Estados de domínio são tratados pela propriedade State. |
| **isDefaultForCloudRedirections** | versão beta &nbsp; - &nbsp; _ &nbsp; ainda não &nbsp; disponível_&nbsp;<br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |

## <a name="oauth2permissionsgrant-property-differences"></a>Diferenças da propriedade OAuth2PermissionsGrant

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **expiryTime** | versão beta &nbsp; - &nbsp; **expiryTime** <br> v 1.0 &nbsp; - &nbsp; _ &nbsp; ainda não &nbsp; está disponível_ | Essa propriedade não é usada e provavelmente será removida no Microsoft Graph. |
| **startTime** | versão beta &nbsp; - &nbsp; **inicial** <br> v 1.0 &nbsp; - &nbsp; _ &nbsp; ainda não &nbsp; está disponível_  | Essa propriedade não é usada e provavelmente será removida no Microsoft Graph. |

## <a name="policy-property-differences"></a>Diferenças de propriedade de política

No Microsoft Graph, há tipos de política nomeados (como tokenIssuancePolicy ou tokenLifetimePolicy), em vez de um tipo de recurso de política genérico. Mais detalhes estão disponíveis na [visão geral da política](/graph/api/resources/policy-overview?view=graph-rest-beta). As políticas ainda não estão disponíveis na v 1.0.

## <a name="serviceendpoint-property-differences"></a>Diferenças de Propriedade ServiceEndpoint

O recurso ServiceEndpoint do Azure AD Graph é renomeado como ponto de extremidade no Microsoft Graph.

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **função** | &nbsp; - &nbsp; **recurso** beta<br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **serviceId** | &nbsp; - &nbsp; **provedor** de versão beta<br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **serviceName** | &nbsp; - &nbsp; **ProviderName** beta<br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **Identificação** | versão beta &nbsp; - &nbsp; **providerResourceId**<br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |
| **URI** | &nbsp; - &nbsp; **URI** beta<br> v 1.0 &nbsp; - &nbsp; _ainda não está disponível_ | |

## <a name="serviceprincipal-property-differences"></a>Diferenças de propriedade de servicePrincipalName

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **appOwnerTenantId** | versão beta &nbsp; - &nbsp; **appOwnerOrganizationId** <br> v 1.0 &nbsp; - &nbsp; **appOwnerOrganizationId** | Renomeado. |
| **informationalUrls**| &nbsp; - &nbsp; **informações** beta <br> &nbsp; - &nbsp; **informações sobre** o v 1.0 | |
| **oauth2Permissions** | versão beta &nbsp; - &nbsp; **publishedPermissionScopes** <br> v 1.0 &nbsp; - &nbsp; **oauth2PermissionScopes** | Renomeado. |
| **preferredTokenSigningKeyEndDateTime** | versão beta &nbsp; - &nbsp; _ainda não disponível_ <br> v 1.0 &nbsp; -  _ainda não está disponível_ | |
| **signInAudience** | versão beta &nbsp; - &nbsp; _ainda não disponível_ <br> v 1.0 &nbsp; -  _ainda não está disponível_ | |
| **Pontos de extremidade** | &nbsp; - &nbsp; **ponto de extremidade** beta <br> ponto de &nbsp; - &nbsp; **extremidade** v 1.0 | Renomeado. |

## <a name="tenantdetails-property-differences"></a>Diferenças da propriedade TenantDetails

O recurso TenantDetails do Azure AD Graph é renomeado para a organização no Microsoft Graph.  Aqui estão as diferenças de propriedade:

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **companyLastDirSyncTime** | versão beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime** <br> v 1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** |  |
| **dirSyncEnabled** | versão beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v 1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** |  |
| **provisioningErrors** | versão beta &nbsp; - &nbsp; _não disponível_ <br> v 1.0 &nbsp; - &nbsp; _não disponível_ | Essa propriedade e suas informações são preteridas.|
| **telephoneNumber** | versão beta &nbsp; - &nbsp; **businessPhones** <br> v 1.0 &nbsp; - &nbsp; **businessPhones** |  |

## <a name="trustedcasforpasswordlessauth-property-differences"></a>Diferenças da propriedade TrustedCasForPasswordlessAuth

O recurso TrustedCasForPasswordlessAuth do Azure AD Graph foi renomeado como [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedauthconfiguration?view=graph-rest-beta)e só está disponível no ponto de extremidade beta do Microsoft Graph. Não há diferenças de propriedade; no entanto, há diferenças no tipo de recurso **certificateAuthority** usado pela propriedade **certificateAuthorities** .

### <a name="certificateauthorityinformation"></a>CertificateAuthorityInformation

O gráfico do Azure AD CertificateAuthorityInformation é renomeado como **certificateAuthority** no Microsoft Graph. A seguir estão as diferenças de propriedade.

|Azure AD Graph. <br>(v 1.6) Propriedade |Microsoft Graph<br> propriedade|Comentários|
|---|---|---|
| **authoritytype** | versão beta &nbsp; - &nbsp; **isRootAuthority**<br> v 1.0 &nbsp; - &nbsp; **isRootAuthority** | O tipo dessa propriedade também foi alterado em um Boolean. Anteriormente, essa propriedade deve ser definida como "RootAuthority" ou "IntermediateAuthority". A definição da nova propriedade como **true** equivale a "RootAuthority". |
| **crlDistributionPoint** | versão beta &nbsp; - &nbsp; **certificateRevocationListUrl** <br> v 1.0 &nbsp; - &nbsp; **certificateRevocationListUrl** | |
| **deltaCrlDistributionPoint** | versão beta &nbsp; - &nbsp; **deltaCertificateRevocationListUrl** <br> v 1.0 &nbsp; - &nbsp; **deltaCertificateRevocationListUrl** | |
| **trustedCertificate** | &nbsp; - &nbsp; **certificado** beta <br> v 1.0 &nbsp; - &nbsp; **deltaCertificateRevocationListUrl** | |
| **trustedIssuer** | &nbsp; - &nbsp; **emissor** beta<br> &nbsp; - &nbsp; **emissor** de v 1.0 | |
| **trustedIssuerSki** | versão beta &nbsp; - &nbsp; **issuerSki**<br> v 1.0 &nbsp; - &nbsp; **issuerSki** | |

## <a name="next-steps"></a>Próximas etapas

- Saiba mais sobre as [diferenças de método](migrate-azure-ad-graph-method-differences.md) entre o Azure ad Graph e o Microsoft Graph.
- Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .
- Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.
