---
title: 'servicePrincipalName: addKey'
description: Adicione uma credencial de chave a um servicePrincipalName.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fccde0dac4e447f0e8558e65d375bb475e652f62
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333974"
---
# <a name="serviceprincipal-addkey"></a>servicePrincipalName: addKey

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Adiciona uma credencial de chave a um [servicePrincipalName](../resources/serviceprincipal.md). Este método junto com o [RemoveKey](serviceprincipal-removekey.md) pode ser usado por um servicePrincipalName para automatizar as chaves de expiração.

> [!NOTE]
> [Criar o servicePrincipalName](../api/serviceprincipal-post-serviceprincipals.md) e [Atualizar](../api/serviceprincipal-update.md) as operações do servicePrincipalName podem continuar a ser usado para adicionar e atualizar as principais credenciais de qualquer servicePrincipalName com ou sem o contexto de um usuário.

Como parte da solicitação de validação para esse método, uma prova de posse de uma chave existente é verificada antes que a ação possa ser executada. 

Os servicePrincipalName que não têm certificados válidos existentes (por exemplo: nenhum certificado foi adicionado ainda, ou todos os certificados expiraram) não poderão usar essa ação de serviço. [Atualize o servicePrincipalName](../api/serviceprincipal-update.md) pode ser usado para executar uma atualização.

## <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Nenhum  |
|Delegado (conta pessoal da Microsoft) | Nenhum.    |
|Aplicativo | Nenhum |

> [!NOTE]
> Um servicePrincipalName não precisa de nenhuma permissão específica para a distribuição de suas próprias chaves.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /serviceprincipals/{id}/addKey
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome           | Descrição                |
|:---------------|:---------------------------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type   | application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça as seguintes propriedades obrigatórias.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| keycredential | [keycredential](../resources/keycredential.md) | A nova credencial de chave de servicePrincipalName a ser adicionada. O __tipo__, __uso__ e __chave__ são propriedades obrigatórias para esse uso. Os tipos de chave com suporte são:<br><ul><li>`AsymmetricX509Cert`: O uso deve ser `Verify` .</li><li>`X509CertAndPassword`: O uso deve ser`Sign`</li></ul>|
| passwordCredential | [passwordCredential](../resources/passwordcredential.md) | Só é necessário definir o __secretText__ que deve conter a senha para a chave. Essa propriedade é obrigatória somente para chaves de tipo `X509CertAndPassword` . Defini-lo como `null` caso contrário.|
| evidência | String | Um token JWT auto-assinado usado como prova de posse das chaves existentes. Esse token JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes de servicePrincipalName. O token deve conter as seguintes declarações:<ul><li>`aud`-A audiência precisa ser `00000002-0000-0000-c000-000000000000` .</li><li>`iss`-Issuer precisa ser a __ID__ do servicePrincipalName que está fazendo a chamada.</li><li>`nbf`-Não antes da hora.</li><li>`exp`– O tempo de expiração deve ser "NBF" + 10 minutos.</li></ul><br>Veja a seguir um [exemplo](/graph/application-rollkey-prooftoken) de código que pode ser usado para gerar esse token de prova de posse.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo objeto [keycredential](../resources/keycredential.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-adding-a-new-key-credential-to-a-serviceprincipal"></a>Exemplo 1: adicionando uma nova credencial de chave a um servicePrincipalName

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey"
}-->

```http
POST https://graph.microsoft.com/beta/serviceprincipals/{id}/addKey
Content-type: application/json

{
    "keyCredential": {
        "type": "AsymmetricX509Cert",
        "usage": "Verify",
        "key": "MIIDYDCCAki..."
    },
    "passwordCredential": null,
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addkey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.keyCredential"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.keyCredential"
}
```

### <a name="example-2-adding-a-key-credential-and-an-associated-password-for-the-key"></a>Exemplo 2: adicionando uma credencial de chave e uma senha associada para a chave

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey"
}-->

```http
POST https://graph.microsoft.com/beta/serviceprincipals/{id}/addKey
Content-type: application/json

{
    "keyCredential": {
        "type": "X509CertAndPassword",
        "usage": "Sign",
        "key": "MIIDYDCCAki..."
    },
    "passwordCredential": {
        "secretText": "MKTr0w1..."
    },
    "proof":"eyJ0eXAiOiJ..."
}
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.keyCredential"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: addKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: serviceprincipal_addkey:\r\n      Resource type was null or missing, so we assume there is no response to validate."
    ]
}-->
