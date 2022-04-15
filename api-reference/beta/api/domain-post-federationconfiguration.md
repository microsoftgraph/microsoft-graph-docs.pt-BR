---
title: Criar federationConfiguration
description: Crie um novo objeto internalDomainFederation.
author: akgoel23
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c7f3857ecaf2f16435d8a1ae2bc0e554fd96d2bd
ms.sourcegitcommit: b21ad24622e199331b6ab838a949ddce9726b41b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2022
ms.locfileid: "64852644"
---
# <a name="create-federationconfiguration"></a>Criar federationConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto internalDomainFederation](../resources/internaldomainfederation.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Domain.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|Domain.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /domains/{domainsId}/federationConfiguration
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto internalDomainFederation](../resources/internaldomainfederation.md) .

Você pode especificar as propriedades a seguir ao criar **um internalDomainFederation**.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição do provedor de identidade federada.|
|issuerUri|Cadeia de Caracteres|URI do emissor do servidor de federação.|
|metadataExchangeUri|Cadeia de Caracteres|URI do ponto de extremidade de troca de metadados usado para autenticação de aplicativos cliente avançados.|
|signingCertificate|Cadeia de Caracteres|Certificado atual usado para assinar tokens passados para o plataforma de identidade da Microsoft. O certificado é formatado como uma cadeia de caracteres codificada em Base64 da parte pública do certificado de assinatura de token do IdP federado e deve ser compatível com a classe X509Certificate2. <br>Essa propriedade é usada nos seguintes cenários: <li> Se uma substituição for necessária fora da atualização de registro automático <li> Um novo serviço de federação está sendo configurado <li> Se o novo certificado de assinatura de token não estiver presente nas propriedades de federação depois que o certificado do serviço de federação tiver sido atualizado.<br>O Azure AD atualiza certificados por meio de um processo de registro automático no qual ele tenta recuperar um novo certificado dos metadados do serviço de federação, 30 dias antes da expiração do certificado atual. Se um novo certificado não estiver disponível, o Azure AD monitorará os metadados diariamente e atualizará as configurações de federação para o domínio quando um novo certificado estiver disponível.|
|passiveSignInUri|Cadeia de Caracteres|URI para o qual os clientes baseados na Web são direcionados ao entrar nos serviços do Azure AD.|
|preferredAuthenticationProtocol|authenticationProtocol|Protocolo de autenticação preferencial. Os valores possíveis são: `wsFed`, `saml`, `unknownFutureValue`.|
|activeSignInUri|Cadeia de Caracteres|URL do ponto de extremidade usado por clientes ativos ao autenticar com domínios federados configurados para logon único no Azure Active Directory (Azure AD). Corresponde à propriedade **ActiveLogOnUri** do [cmdlet Set-MsolDomainFederationSettings MSOnline v1 do PowerShell](/powershell/module/msonline/set-msoldomainfederationsettings).|
|signOutUri|Cadeia de caracteres|URI para o qual os clientes são redirecionados ao sair dos serviços do Azure AD. Corresponde à propriedade **LogOffUri** do [cmdlet Set-MsolDomainFederationSettings MSOnline v1 do PowerShell](/powershell/module/msonline/set-msoldomainfederationsettings).|
|promptLoginBehavior|promptLoginBehavior|Define o comportamento preferencial para o prompt de entrada. Os valores possíveis são: `translateToFreshPasswordAuthentication`, `nativeSupport`, `disabled`, `unknownFutureValue`.|
|isSignedAuthenticationRequestRequired|Booleano|Se for true, quando as solicitações de autenticação SAML forem enviadas para o IDP do SAML federado, o Azure AD assinará essas solicitações usando a chave de assinatura orgID. Se for false (padrão), as solicitações de autenticação SAML enviadas para o IDP federado não serão assinadas.|
|nextSigningCertificate|Cadeia de Caracteres|Certificado de autenticação de token de fallback usado para assinar tokens quando o certificado de assinatura primário expira. Formatado como cadeias de caracteres codificadas em Base64 da parte pública do certificado de autenticação de token do IdP federado. Precisa ser compatível com a classe X509Certificate2. Assim como o **signingCertificate**, a propriedade **nextSigningCertificate** será usada se uma substituição for necessária fora da atualização de substituição automática, um novo serviço de federação será configurado ou se o novo certificado de assinatura de token não estiver presente nas propriedades de federação depois que o certificado do serviço de federação for atualizado.|
|signingCertificateUpdateStatus|[signingCertificateUpdateStatus](../resources/signingcertificateupdatestatus.md)|Fornece o status e o carimbo de data/hora da última atualização do certificado de assinatura.|
|federatedIdpMfaBehavior|federatedIdpMfaBehavior|Determina se o Azure AD aceita a MFA executada pelo IdP federado quando um usuário federado acessa um aplicativo que é regido por uma política de acesso condicional que requer MFA. Os valores possíveis são: `acceptIfMfaDoneByFederatedIdp`, `enforceMfaByFederatedIdp`, `rejectMfaByFederatedIdp`, `unknownFutureValue`. Para obter mais informações, consulte [valores federatedIdpMfaBehavior](#federatedidpmfabehavior-values).|

### <a name="federatedidpmfabehavior-values"></a>Valores federatedIdpMfaBehavior

| Member | Descrição |
| :--- | :--- |
| acceptIfMfaDoneByFederatedIdp | O Azure AD aceita a MFA executada pelo provedor de identidade federada. Se o provedor de identidade federada não tiver executado a MFA, o Azure AD executará a MFA. |
| enforceMfaByFederatedIdp | O Azure AD aceita a MFA executada pelo provedor de identidade federado. Se o provedor de identidade federada não tiver executado a MFA, ele redirecionará a solicitação para o provedor de identidade federada para executar a MFA. |
| rejectMfaByFederatedIdp | O Azure AD sempre executa a MFA e rejeita a MFA executada pelo provedor de identidade federada. |

**Observação:** **federatedIdpMfaBehavior** é uma versão evoluida da propriedade **SupportsMfa** do [cmdlet Do PowerShell Set-MsolDomainFederationSettings MSOnline v1](/powershell/module/msonline/set-msoldomainfederationsettings). 
+ Não há suporte **para a alternância entre federatedIdpMfaBehavior** e **SupportsMfa** .
+ Depois **que a propriedade federatedIdpMfaBehavior** é definida, o Azure AD ignora a **configuração SupportsMfa** .
+ Se a **propriedade federatedIdpMfaBehavior** nunca for definida, o Azure AD continuará respeitando a **configuração SupportsMfa** .
+ Se nem **federatedIdpMfaBehavior** nem **SupportsMfa** estiver definido, o Azure AD usará o comportamento como `acceptIfMfaDoneByFederatedIdp` padrão.


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `201 Created` de resposta e um [objeto internalDomainFederation](../resources/internaldomainfederation.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "create_internaldomainfederation_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/domains/contoso.com/federationConfiguration
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.internalDomainFederation",
  "displayName": "Contoso",
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
  "federatedIdpMfaBehavior": "rejectMfaByFederatedIdp"
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
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.internalDomainFederation",
  "id": "6601d14b-d113-8f64-fda2-9b5ddda18ecc",
   "displayName": "Contoso",
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
   "federatedIdpMfaBehavior": "rejectMfaByFederatedIdp"
}
```

