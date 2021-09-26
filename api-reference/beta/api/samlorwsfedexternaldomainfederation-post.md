---
title: Criar samlOrWsFedExternalDomainFederation
description: Crie um novo objeto samlOrWsFedExternalDomainFederation.
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6d7dc9d422ebe5d3db6fe98b168956d820b92fdd
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766866"
---
# <a name="create-samlorwsfedexternaldomainfederation"></a>Criar samlOrWsFedExternalDomainFederation
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto samlOrWsFedExternalDomainFederation.](../resources/samlorwsfedexternaldomainfederation.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)|Domain.Read.All, Domain.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo|Domain.Read.All, Domain.ReadWrite.All|

A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:

* Administrador Global
* Administrador do Provedor de Identidade Externa

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /directory/federationConfigurations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do [objeto samlOrWsFedExternalDomainFederation.](../resources/samlorwsfedexternaldomainfederation.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição do provedor de identidade baseado em SAML/WS-Fed. Herdado de [identityProviderBase](../resources/identityproviderbase.md).|
|issuerUri|String|URI do emissor do servidor de federação. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|metadataExchangeUri|String|URI do ponto de extremidade do exchange de metadados usado para autenticação de aplicativos cliente ricos. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|passiveSignInUri|String|URI para os quais os clientes baseados na Web são direcionados ao entrar nos serviços do Azure AD. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|preferredAuthenticationProtocol|String|Protocolo de autenticação preferencial. Os valores com suporte incluem `saml` ou `wsfed` . Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|signingCertificate|Cadeia de caracteres|Certificado atual usado para assinar tokens passados para o plataforma de identidade da Microsoft. O certificado é formatado como uma cadeia de caracteres codificada base64 da parte pública do certificado de assinatura de token do IdP federado e deve ser compatível com a classe X509Certificate2.  <br/><br/> Essa propriedade é usada nos seguintes cenários: <ul><li> se uma rolagem for necessária fora da atualização de rolagem automática <li>um novo serviço de federação está sendo criado <li> se o novo certificado de assinatura de token não estiver presente nas propriedades de federação após a atualização do certificado de serviço de federação. </ul> <br/><br/> O Azure AD atualiza certificados por meio de um processo de autorollover no qual tenta recuperar um novo certificado dos metadados do serviço de federação, 30 dias antes da expiração do certificado atual. Se um novo certificado não estiver disponível, o Azure AD monitorará os metadados diariamente e atualizará as configurações de federação para o domínio quando um novo certificado estiver disponível.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_samlorwsfedexternaldomainfederation_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/directory/federationConfigurations
Content-Type: application/json
Content-length: 283

{
    "@odata.type": "microsoft.graph.samlOrWsFedExternalDomainFederation",
    "issuerUri": "https://contoso.com/issuerUri",
    "displayName": "contoso display name",
    "metadataExchangeUri": "https://contoso.com/metadataExchangeUri",
    "passiveSignInUri": "https://contoso.com/signin",
    "preferredAuthenticationProtocol": "wsFed",
    "domains": [
        {
            "@odata.type": "microsoft.graph.externalDomainName",
            "id": "contoso.com"
        }
    ],
    "signingCertificate": "MIIDADCCAeigAwIBAgIQEX41y8r6"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-samlorwsfedexternaldomainfederation-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-samlorwsfedexternaldomainfederation-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-samlorwsfedexternaldomainfederation-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProviderBase"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "id": "3c41f317-9af3-4266-8ccf-26283ceec888",
    "displayName": "contoso display name"
}
```
