---
title: 'aplicativo: addKey'
description: Adicione uma credencial de chave a um aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 38b7fa91f1c22d14565eb5cd82170f8a73851045
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383858"
---
# <a name="application-addkey"></a>aplicativo: addKey

Namespace: microsoft.graph

Adicione uma credencial de chave a um [aplicativo](../resources/application.md). Este método, junto com o [RemoveKey](application-removekey.md) , pode ser usado por um aplicativo para automatizar as chaves de expiração.

> [!NOTE]
> [Create Application](../api/application-post-applications.md) and [Update Application](../api/application-update.md) Operations pode continuar a ser usado para adicionar e atualizar as principais credenciais de qualquer aplicativo com ou sem um contexto de usuário.

Como parte da solicitação de validação para esse método, uma prova de posse de uma chave existente é verificada antes que a ação possa ser executada. 

Os aplicativos que não têm certificados válidos existentes (nenhum certificado foi adicionado ainda, ou todos os certificados expiraram) não poderão usar essa ação de serviço. Você pode usar a operação [Atualizar aplicativo](../api/application-update.md) para executar uma atualização.

## <a name="permissions"></a>Permissions

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Nenhum  |
|Delegado (conta pessoal da Microsoft) | Nenhum.    |
|Aplicativo | Nenhum |

> [!NOTE] 
> Um aplicativo não precisa de nenhuma permissão específica para rolar suas próprias chaves.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addKey
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
| keycredential | [keycredential](../resources/keycredential.md) | A nova credencial de chave de aplicativo a ser adicionada. O __tipo__, __uso__ e __chave__ são propriedades obrigatórias para esse uso. Os tipos de chave com suporte são:<br><ul><li>`AsymmetricX509Cert`: O uso deve ser `Verify` .</li><li>`X509CertAndPassword`: O uso deve ser`Sign`</li></ul>|
| passwordCredential | [passwordCredential](../resources/passwordcredential.md) | Só é necessário definir o __secretText__ que deve conter a senha para a chave. Essa propriedade é obrigatória somente para chaves de tipo `X509CertAndPassword` . Defini-lo como `null` caso contrário.|
| evidência | String | Um token JWT auto-assinado usado como prova de posse das chaves existentes. Esse token JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes do aplicativo. O token deve conter as seguintes declarações:<ul><li>`aud`-A audiência precisa ser `00000002-0000-0000-c000-000000000000` .</li><li>`iss`– O emissor precisa ser a __ID__ do aplicativo que está fazendo a chamada.</li><li>`nbf`-Não antes da hora.</li><li>`exp`– O tempo de expiração deve ser "NBF" + 10 minutos.</li></ul><br>Veja a seguir um [exemplo](/graph/application-rollkey-prooftoken) de código que pode ser usado para gerar esse token de prova de posse.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo objeto [keycredential](../resources/keycredential.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-add-a-new-key-credential-to-an-application"></a>Exemplo 1: adicionar uma nova credencial de chave a um aplicativo

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_addkey"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/addKey
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-addkey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-addkey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-addkey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-addkey-java-snippets.md)]
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.keyCredential"
}
```

### <a name="example-2-add-a-key-credential-and-an-associated-password-for-the-key"></a>Exemplo 2: adicionar uma credencial de chave e uma senha associada para a chave

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "application_addkey"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/addKey
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.keyCredential"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: addKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: application_addkey:\r\n      Resource type was null or missing, so we assume there is no response to validate."
    ]
}-->
