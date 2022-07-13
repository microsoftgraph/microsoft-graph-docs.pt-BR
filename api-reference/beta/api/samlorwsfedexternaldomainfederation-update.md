---
title: Atualizar samlOrWsFedExternalDomainFederation
description: Atualize as propriedades de um objeto samlOrWsFedExternalDomainFederation.
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4e6f568cd2be81883086ea45aa1434f2669e0f17
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768144"
---
# <a name="update-samlorwsfedexternaldomainfederation"></a>Atualizar samlOrWsFedExternalDomainFederation
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um [objeto samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante)|IdentityProvider.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo|IdentityProvider.ReadWrite.All|

A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções do [Azure Active Directory (Azure AD](/azure/active-directory/roles/permissions-reference)):

* Administrador Global
* Administrador do Provedor de Identidade Externo

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH directory/federationConfigurations/graph.samlOrWsFedExternalDomainFederation/{samlOrWsFedExternalDomainFederation ID}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça um objeto JSON com uma ou mais propriedades que precisam ser atualizadas para um objeto [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) no Azure AD locatário.

A tabela a seguir mostra as propriedades que você pode atualizar para um [objeto samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) .

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome de exibição do provedor de identidade baseado em SAML/WS-Fed. Herdado de [identityProviderBase](../resources/identityproviderbase.md).|
|issuerUri|String|URI do emissor do servidor de federação. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|metadataExchangeUri|String|URI do ponto de extremidade de troca de metadados usado para autenticação de aplicativos cliente avançados. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|passiveSignInUri|String|URI para o qual os clientes baseados na Web são direcionados ao entrar Azure AD serviços. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|preferredAuthenticationProtocol|String|Protocolo de autenticação preferencial. Os valores com suporte incluem `saml` ou `wsfed`. Herdado [de samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|signingCertificate|String|Certificado atual usado para assinar tokens passados para o plataforma de identidade da Microsoft. O certificado é formatado como uma cadeia de caracteres codificada em Base64 da parte pública do certificado de assinatura de token do IdP federado e deve ser compatível com a classe X509Certificate2.  <br/><br/> Essa propriedade é usada nos seguintes cenários: <ul><li> se uma substituição for necessária fora da atualização de registro automático <li>um novo serviço de federação está sendo configurado <li> se o novo certificado de assinatura de token não estiver presente nas propriedades de federação depois que o certificado do serviço de federação tiver sido atualizado. </ul> <br/><br/> Azure AD atualiza certificados por meio de um processo de registro automático no qual ele tenta recuperar um novo certificado dos metadados do serviço de federação, 30 dias antes da expiração do certificado atual. Se um novo certificado não estiver disponível, o Azure AD monitorará os metadados diariamente e atualizará as configurações de federação para o domínio quando um novo certificado estiver disponível.|

## <a name="response"></a>Resposta

Se tiver êxito, este método `200 OK` retornará um código de resposta e um objeto [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_samlorwsfedexternaldomainfederation"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/directory/federationConfigurations/graph.samlOrWsFedExternalDomainFederation/d5a56845-6845-d5a5-4568-a5d54568a5d5
Content-Type: application/json

{
  "displayName": "Contoso name change",
  "issuerUri": "http://contoso-test.com/adfs/services/trust",
  "metadataExchangeUri": null,
  "signingCertificate": "M66C6DCCAdCgAwIBAgIQQ6vYJIVKQ",
  "passiveSignInUri": "https://contoso-test.com/adfs/ls/",
  "preferredAuthenticationProtocol": "wsFed"
}


```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-samlorwsfedexternaldomainfederation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-samlorwsfedexternaldomainfederation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-samlorwsfedexternaldomainfederation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-samlorwsfedexternaldomainfederation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.samlOrWsFedExternalDomainFederation"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
 "id": "d5a56845-6845-d5a5-4568-a5d54568a5d5",
  "displayName": "Contoso name change",
  "issuerUri": "http://contoso-test.com/adfs/services/trust",
  "metadataExchangeUri": null,
  "signingCertificate": "M66C6DCCAdCgAwIBAgIQQ6vYJIVKQ",
  "passiveSignInUri": "https://contoso-test.com/adfs/ls/",
  "preferredAuthenticationProtocol": "wsFed",
  "domains": [
      {
          "id": "contoso.com"
      }
  ]
}
```
