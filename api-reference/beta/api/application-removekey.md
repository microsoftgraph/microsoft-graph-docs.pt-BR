---
title: 'application: removeKey'
description: Remover uma credencial de chave de um aplicativo
ms.localizationpriority: medium
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: e9fbfcc4a506e876655ece20e8c1e69813e7f3fb
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340403"
---
# <a name="application-removekey"></a>application: removeKey

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Remova uma credencial de chave de um [aplicativo](../resources/application.md). Esse método juntamente com [addKey](application-addkey.md) pode ser usado por um aplicativo para automatizar a rolagem de suas chaves expiradas.

> [!NOTE]
> [Crie servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) e [Update servicePrincipal](../api/serviceprincipal-update.md) operações podem continuar a ser usadas para adicionar e atualizar credenciais de chave para qualquer aplicativo com aplicativo ou contexto de usuário.

Como parte da validação de solicitação para esse método, uma prova de posse de uma chave existente é verificada antes que a ação possa ser executada.

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
POST /applications/{id}/removeKey
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome           | Descrição                |
|:---------------|:---------------------------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type   | application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça as seguintes propriedades necessárias.

| Propriedade  | Tipo | Descrição|
|:----------|:-----|:-----------|
| keyId     | GUID | O identificador exclusivo da senha.|
| proof | String | Um token JWT auto-assinado usado como prova de posse das chaves existentes. Esse token de JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes do aplicativo. O token deve conter os seguintes argumentos:<ul><li>`aud` – A audiência deve ser `00000002-0000-0000-c000-000000000000`.</li><li>`iss` - O emissor deve ser o __ID__ do aplicativo que está fazendo a chamada.</li><li>`nbf` – Não antes da hora.</li><li>`exp` - O tempo de expiração deve ser `nbf` + 10 minutos.</li></ul><br>Para etapas para gerar essa prova de token de posse, consulte [Generating proof of possess tokens for rolling keys](/graph/application-rollkey-prooftoken).|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No content`.

## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_removekey"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/removeKey
Content-Type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-removekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-removekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-removekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-removekey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/application-removekey-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/application-removekey-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: removeKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



