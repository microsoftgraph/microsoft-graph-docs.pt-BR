---
title: Tipo de recurso internalDomainFederation
description: Representa as configurações dos domínios em um locatário que são federados com Azure AD.
author: akgoel23
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: eb5788ebd83810834d19fe9500f13f11df9f6554
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447393"
---
# <a name="internaldomainfederation-resource-type"></a>Tipo de recurso internalDomainFederation

Namespace: microsoft.graph

Representa configurações de domínios de locatário que são federados com Azure AD. Use esse recurso para definir as configurações de federação ao configurar a federação com Azure AD. Para obter informações sobre federação, consulte [O que é federação com Azure AD?](/azure/active-directory/hybrid/whatis-fed).


Herda [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Criar federationConfiguration](../api/domain-post-federationconfiguration.md)|[internalDomainFederation](../resources/internaldomainfederation.md)|Crie um novo [objeto internalDomainFederation](../resources/internaldomainfederation.md) .|
|[Obter internalDomainFederation](../api/internaldomainfederation-get.md)|[internalDomainFederation](../resources/internaldomainfederation.md)|Leia as propriedades e as relações de um [objeto internalDomainFederation](../resources/internaldomainfederation.md) .|
|[Atualizar internalDomainFederation](../api/internaldomainfederation-update.md)|[internalDomainFederation](../resources/internaldomainfederation.md)|Atualize as propriedades de um [objeto internalDomainFederation](../resources/internaldomainfederation.md) .|
|[Excluir internalDomainFederation](../api/internaldomainfederation-delete.md)|Nenhum|[Exclua um objeto internalDomainFederation](../resources/internaldomainfederation.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|activeSignInUri|Cadeia de caracteres|URL do ponto de extremidade usado por clientes ativos ao autenticar com domínios federados configurados para logon único no Azure Active Directory (Azure AD). Corresponde à propriedade **ActiveLogOnUri** do [cmdlet Set-MsolDomainFederationSettings MSOnline v1 do PowerShell](/powershell/module/msonline/set-msoldomainfederationsettings).|
|displayName|String|O nome de exibição do IdP (provedor de identidade federada). Herdado de [identityProviderBase](../resources/identityproviderbase.md).|
|federatedIdpMfaBehavior|federatedIdpMfaBehavior|Determina se Azure AD aceita a MFA executada pelo IdP federado quando um usuário federado acessa um aplicativo que é regido por uma política de acesso condicional que requer MFA. Os valores possíveis são: `acceptIfMfaDoneByFederatedIdp`, `enforceMfaByFederatedIdp`, `rejectMfaByFederatedIdp`, `unknownFutureValue`. Para obter mais informações, consulte [valores federatedIdpMfaBehavior](#federatedidpmfabehavior-values).|
|id|Cadeia de caracteres|O identificador do provedor de identidade federada. Herdado da [entidade](../resources/entity.md).|
|isSignedAuthenticationRequestRequired|Booliano|Se`true`, quando as solicitações de autenticação SAML forem enviadas para o IdP do SAML federado, Azure AD assinará essas solicitações usando a chave de assinatura orgID. Se `false` (padrão), as solicitações de autenticação SAML enviadas ao IdP federado não serão assinadas.|
|issuerUri|Cadeia de caracteres|URI do emissor do servidor de federação. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|metadataExchangeUri|Cadeia de caracteres|URI do ponto de extremidade de troca de metadados usado para autenticação de aplicativos cliente avançados. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|nextSigningCertificate|Cadeia de caracteres|Certificado de autenticação de token de fallback usado para assinar tokens quando o certificado de assinatura primário expira. Formatado como cadeias de caracteres codificadas em Base64 da parte pública do certificado de autenticação de token do IdP federado. Precisa ser compatível com a classe X509Certificate2. Assim como o signingCertificate, a propriedade nextSigningCertificate será usada se uma substituição for necessária fora da atualização de substituição automática, um novo serviço de federação será configurado ou se o novo certificado de assinatura de token não estiver presente nas propriedades de federação depois que o certificado do serviço de federação for atualizado.|
|passiveSignInUri|Cadeia de caracteres|URI para o qual os clientes baseados na Web são direcionados ao entrar Azure AD serviços. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|preferredAuthenticationProtocol|authenticationProtocol|Protocolo de autenticação preferencial. Os valores possíveis são: `wsFed`, `saml`, `unknownFutureValue`. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|promptLoginBehavior|promptLoginBehavior|Define o comportamento preferencial para o prompt de entrada. Os valores possíveis são: `translateToFreshPasswordAuthentication`, `nativeSupport`, `disabled`, `unknownFutureValue`.|
|signingCertificate|Cadeia de caracteres|Certificado atual usado para assinar tokens passados para o plataforma de identidade da Microsoft. O certificado é formatado como uma cadeia de caracteres codificada em Base64 da parte pública do certificado de assinatura de token do IdP federado e deve ser compatível com a classe X509Certificate2. <br>Essa propriedade é usada nos seguintes cenários: <li> Se uma substituição for necessária fora da atualização de registro automático <li> Um novo serviço de federação está sendo configurado <li> Se o novo certificado de assinatura de token não estiver presente nas propriedades de federação depois que o certificado do serviço de federação tiver sido atualizado.<br>Azure AD atualiza certificados por meio de um processo de registro automático no qual ele tenta recuperar um novo certificado dos metadados do serviço de federação, 30 dias antes da expiração do certificado atual. Se um novo certificado não estiver disponível, o Azure AD monitorará os metadados diariamente e atualizará as configurações de federação para o domínio quando um novo certificado estiver disponível. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|signingCertificateUpdateStatus|[signingCertificateUpdateStatus](../resources/signingcertificateupdatestatus.md)|Fornece o status e o carimbo de data/hora da última atualização do certificado de assinatura.|
|signOutUri|String|URI para o qual os clientes são redirecionados ao sair Azure AD serviços. Corresponde à propriedade **LogOffUri** do [cmdlet Set-MsolDomainFederationSettings MSOnline v1 do PowerShell](/powershell/module/msonline/set-msoldomainfederationsettings).|

### <a name="federatedidpmfabehavior-values"></a>Valores federatedIdpMfaBehavior

| Member | Descrição |
| :--- | :--- |
| acceptIfMfaDoneByFederatedIdp | Azure AD aceita MFA executada pelo provedor de identidade federada. Se o provedor de identidade federada não tiver executado a MFA, Azure AD executará a MFA. |
| enforceMfaByFederatedIdp | Azure AD aceita MFA executada pelo provedor de identidade federada. Se o provedor de identidade federada não tiver executado a MFA, ele redirecionará a solicitação para o provedor de identidade federada para executar a MFA. |
| rejectMfaByFederatedIdp | Azure AD sempre executa a MFA e rejeita a MFA executada pelo provedor de identidade federada. |

>[!NOTE]
>**federatedIdpMfaBehavior** é uma versão evoluida da propriedade **SupportsMfa** do [cmdlet Do PowerShell Set-MsolDomainFederationSettings MSOnline v1](/powershell/module/msonline/set-msoldomainfederationsettings). 
>+ Não há suporte **para a alternância entre federatedIdpMfaBehavior** e **SupportsMfa** .
>+ Quando **a propriedade federatedIdpMfaBehavior** é definida, Azure AD ignora a **configuração SupportsMfa**.
>+ Se a **propriedade federatedIdpMfaBehavior** nunca for definida, Azure AD continuará respeitando a configuração **SupportsMfa**.
>+ Se nem **federatedIdpMfaBehavior** nem **SupportsMfa** estiver definido, Azure AD padrão será o `acceptIfMfaDoneByFederatedIdp` comportamento.

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.internalDomainFederation",
  "baseType": "microsoft.graph.samlOrWsFedProvider",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.internalDomainFederation",
  "id": "String (identifier)",
  "displayName": "String",
  "issuerUri": "String",
  "metadataExchangeUri": "String",
  "signingCertificate": "String",
  "passiveSignInUri": "String",
  "preferredAuthenticationProtocol": "String",
  "activeSignInUri": "String",
  "signOutUri": "String",
  "promptLoginBehavior": "String",
  "isSignedAuthenticationRequestRequired": "Boolean",
  "nextSigningCertificate": "String",
  "signingCertificateUpdateStatus": {
    "certificateUpdateResult": "String",
    "@odata.type": "microsoft.graph.signingCertificateUpdateStatus"
  },
  "federatedIdpMfaBehavior": "String"
}
```

