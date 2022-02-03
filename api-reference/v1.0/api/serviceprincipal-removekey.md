---
title: 'servicePrincipal: removeKey'
description: Remover uma credencial de chave de um servicePrincipal
ms.localizationpriority: medium
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 70fcb44414bae5f22ab42a01be52f45aa6c1b738
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344121"
---
# <a name="serviceprincipal-removekey"></a>servicePrincipal: removeKey

Namespace: microsoft.graph

Remova uma credencial de chave de [um servicePrincipal](../resources/serviceprincipal.md). Esse método juntamente com [addKey](serviceprincipal-addkey.md) pode ser usado por um servicePrincipal para automatizar a rolagem de suas chaves expiradas.

> [!NOTE]
> [Criar servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) e [Atualizar service As operaçõesPrincipal](../api/serviceprincipal-update.md) podem continuar a ser usadas para adicionar e atualizar credenciais de chave para qualquer servicePrincipal com ou sem o contexto de um usuário.

Como parte da validação de solicitação para esse método, uma prova de posse de uma chave existente é verificada antes que a ação possa ser executada.

## <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.AccessAsUser.All, Application.ReadWrite.All, Directory.ReadWrite.All   |
|Delegado (conta pessoal da Microsoft) | Nenhum.    |
|Aplicativo | Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/removeKey
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
| proof | Cadeia de caracteres | Um token JWT auto-assinado usado como prova de posse das chaves existentes. Esse token JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes do servicePrincipal. O token deve conter os seguintes argumentos:<ul><li>`aud` – A audiência deve ser `00000002-0000-0000-c000-000000000000`.</li><li>`iss` - O emissor precisa ser __a id__  do servicePrincipal que está fazendo a chamada.</li><li>`nbf` – Não antes da hora.</li><li>`exp` – O tempo de expiração deve ser "nbf" + 10 min.</li></ul><br>Aqui está um exemplo [de código](/graph/application-rollkey-prooftoken) que pode ser usado para gerar essa prova de token de posse.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No content`.

## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_removekey"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/removeKey
Content-Type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-removekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-removekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-removekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-removekey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/serviceprincipal-removekey-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/serviceprincipal-removekey-powershell-snippets.md)]
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
  "description": "servicePrincipal: removeKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

