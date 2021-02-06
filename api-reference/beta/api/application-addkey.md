---
title: 'application: addKey'
description: Adicione uma credencial de chave a um aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 184608404cfff5eda297a184373fc71f88869c4f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129538"
---
# <a name="application-addkey"></a>application: addKey

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Adicione uma credencial de chave a um [aplicativo.](../resources/application.md) Esse método, juntamente com [removeKey](application-removekey.md), pode ser usado por um aplicativo para automatizar a rolagem de suas chaves expiradas.

> [!NOTE]
> Você pode continuar [](../api/application-post-applications.md) a usar [](../api/application-update.md) as operações Criar aplicativo e Atualizar aplicativo para adicionar e atualizar credenciais de chave para qualquer aplicativo com ou sem o contexto de um usuário. 

Como parte da validação da solicitação para esse método, uma prova de posse de uma chave existente é verificada antes que a ação possa ser executada. 

Os aplicativos que não têm certificados válidos existentes (nenhum certificado foi adicionado ainda ou todos os certificados expiraram), não poderão usar essa ação de serviço. Você pode usar a operação [Atualizar aplicativo](../api/application-update.md) para executar uma atualização.

## <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Nenhum.  |
|Delegado (conta pessoal da Microsoft) | Nenhum.    |
|Aplicativo | Nenhum. |

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

No corpo da solicitação, forneça as seguintes propriedades necessárias.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| keyCredential | [keyCredential](../resources/keycredential.md) | A nova credencial de chave de aplicativo a ser acrescentada. O __tipo__, __uso__ __e chave__ são propriedades necessárias para esse uso. Os tipos de chave com suporte são:<br><ul><li>`AsymmetricX509Cert`: o uso deve `Verify` ser.</li><li>`X509CertAndPassword`: o uso deve ser `Sign`</li></ul>|
| passwordCredential | [passwordCredential](../resources/passwordcredential.md) | Somente __secretText__ é necessário para ser definido que deve conter a senha da chave. Essa propriedade é necessária somente para chaves do tipo `X509CertAndPassword` . De definida como `null` caso contrário.|
| proof | String | Um token JWT auto-assinado usado como prova de posse das chaves existentes. Esse token de JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes do aplicativo. O token deve conter os seguintes argumentos:<ul><li>`aud` – A audiência deve ser `00000002-0000-0000-c000-000000000000`.</li><li>`iss` - O emissor deve ser o __ID__ do aplicativo que está fazendo a chamada.</li><li>`nbf` – Não antes da hora.</li><li>`exp` – O tempo de expiração deve ser "nbf" + 10 min.</li></ul><br>Aqui está um exemplo [de código](/graph/application-rollkey-prooftoken) que pode ser usado para gerar esse token de comprovação de posse.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta e um `200 OK` novo [objeto keyCredential](../resources/keycredential.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-add-a-new-key-credential-to-an-application"></a>Exemplo 1: Adicionar uma nova credencial de chave a um aplicativo

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_addkey"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/addKey
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.keyCredential"
}
```

### <a name="example-2-add-a-key-credential-and-an-associated-password-for-the-key"></a>Exemplo 2: Adicionar uma credencial de chave e uma senha associada à chave

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "application_addkey"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/addKey
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
  "description": "application: addKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: application_addkey:\r\n      Resource type was null or missing, so we assume there is no response to validate."
    ]
}-->



