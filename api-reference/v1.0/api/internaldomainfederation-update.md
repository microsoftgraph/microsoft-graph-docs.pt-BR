---
title: Atualizar internalDomainFederation
description: Atualize as propriedades de um objeto internalDomainFederation.
author: akgoel23
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5498cc69bde517632af1bc481240f962be03b1a3
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447401"
---
# <a name="update-internaldomainfederation"></a>Atualizar internalDomainFederation
Namespace: microsoft.graph

Atualize as propriedades de um [objeto internalDomainFederation](../resources/internaldomainfederation.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Domain.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|Domain.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /domains/{domainsId}/federationConfiguration/{internalDomainFederationId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|activeSignInUri|Cadeia de caracteres|URL do ponto de extremidade usado por clientes ativos ao autenticar com domínios federados configurados para logon único no Azure Active Directory (Azure AD). Corresponde à propriedade **ActiveLogOnUri** do [cmdlet Set-MsolDomainFederationSettings MSOnline v1 do PowerShell](/powershell/module/msonline/set-msoldomainfederationsettings).|
|displayName|Cadeia de caracteres|O nome de exibição do IdP (provedor de identidade federada). |
|federatedIdpMfaBehavior|federatedIdpMfaBehavior|Determina se Azure AD aceita a MFA executada pelo IdP federado quando um usuário federado acessa um aplicativo que é regido por uma política de acesso condicional que requer MFA. Os valores possíveis são: `acceptIfMfaDoneByFederatedIdp`, `enforceMfaByFederatedIdp`, `rejectMfaByFederatedIdp`, `unknownFutureValue`. Para obter mais informações, consulte [valores federatedIdpMfaBehavior](#federatedidpmfabehavior-values).|
|isSignedAuthenticationRequestRequired|Booliano|Se`true`, quando as solicitações de autenticação SAML forem enviadas para o IdP do SAML federado, Azure AD assinará essas solicitações usando a chave de assinatura orgID. Se `false` (padrão), as solicitações de autenticação SAML enviadas ao IdP federado não serão assinadas.|
|issuerUri|Cadeia de caracteres|URI do emissor do servidor de federação.|
|metadataExchangeUri|String|URI do ponto de extremidade de troca de metadados usado para autenticação de aplicativos cliente avançados.|
|nextSigningCertificate|Cadeia de caracteres|Certificado de autenticação de token de fallback usado para assinar tokens quando o certificado de assinatura primário expira. Formatado como cadeias de caracteres codificadas em Base64 da parte pública do certificado de autenticação de token do IdP federado. Precisa ser compatível com a classe X509Certificate2. Assim como o **signingCertificate**, a propriedade **nextSigningCertificate** será usada se uma substituição for necessária fora da atualização de substituição automática, um novo serviço de federação será configurado ou se o novo certificado de assinatura de token não estiver presente nas propriedades de federação depois que o certificado do serviço de federação for atualizado.|
|passiveSignInUri|Cadeia de caracteres|URI para o qual os clientes baseados na Web são direcionados ao entrar Azure AD serviços. |
|preferredAuthenticationProtocol|authenticationProtocol|Protocolo de autenticação preferencial. Os valores possíveis são: `wsFed`, `saml`, `unknownFutureValue`. |
|promptLoginBehavior|promptLoginBehavior|Define o comportamento preferencial para o prompt de entrada. Os valores possíveis são: `translateToFreshPasswordAuthentication`, `nativeSupport`, `disabled`, `unknownFutureValue`.|
|signingCertificate|Cadeia de caracteres|Certificado atual usado para assinar tokens passados para o plataforma de identidade da Microsoft. O certificado é formatado como uma cadeia de caracteres codificada em Base64 da parte pública do certificado de assinatura de token do IdP federado e deve ser compatível com a classe X509Certificate2. <br>Essa propriedade é usada nos seguintes cenários: <li> Se uma substituição for necessária fora da atualização de registro automático <li> Um novo serviço de federação está sendo configurado <li> Se o novo certificado de assinatura de token não estiver presente nas propriedades de federação depois que o certificado do serviço de federação tiver sido atualizado.<br>Azure AD atualiza certificados por meio de um processo de registro automático no qual ele tenta recuperar um novo certificado dos metadados do serviço de federação, 30 dias antes da expiração do certificado atual. Se um novo certificado não estiver disponível, o Azure AD monitorará os metadados diariamente e atualizará as configurações de federação para o domínio quando um novo certificado estiver disponível. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|signingCertificateUpdateStatus|[signingCertificateUpdateStatus](../resources/signingcertificateupdatestatus.md)|Fornece o status e o carimbo de data/hora da última atualização do certificado de assinatura.|
|signOutUri|Cadeia de caracteres|URI para o qual os clientes são redirecionados ao sair Azure AD serviços. Corresponde à propriedade **LogOffUri** do [cmdlet Set-MsolDomainFederationSettings MSOnline v1 do PowerShell](/powershell/module/msonline/set-msoldomainfederationsettings).|

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



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [internalDomainFederation atualizado](../resources/internaldomainfederation.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "update_internaldomainfederation"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/domains/contoso.com/federationConfiguration/6601d14b-d113-8f64-fda2-9b5ddda18ecc
Content-Type: application/json

{
  "displayName": "Contoso name change",  
  "federatedIdpMfaBehavior": "acceptIfMfaDoneByFederatedIdp"
}
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.internalDomainFederation"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.internalDomainFederation",
  "id": "6601d14b-d113-8f64-fda2-9b5ddda18ecc",
   "displayName": "Contoso name change",
   "issuerUri": "http://contoso.com/adfs/services/trust",
   "metadataExchangeUri": "https://sts.contoso.com/adfs/services/trust/mex",
   "signingCertificate": "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI",
   "passiveSignInUri": "https://sts.contoso.com/adfs/ls",
   "preferredAuthenticationProtocol": "wsFed",
   "activeSignInUri": "https://sts.contoso.com/adfs/services/trust/2005/usernamemixed",
   "signOutUri": "https://sts.contoso.com/adfs/ls",
   "promptLoginBehavior": "nativeSupport",
   "isSignedAuthenticationRequestRequired": true,
   "nextSigningCertificate": "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI",
   "signingCertificateUpdateStatus": {
        "certificateUpdateResult": "Success",
        "lastRunDateTime": "2021-08-25T07:44:46.2616778Z"
    },
   "federatedIdpMfaBehavior": "acceptIfMfaDoneByFederatedIdp"
}
```

