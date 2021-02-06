---
title: 'servicePrincipal: removeKey'
description: Remover uma credencial de chave de uma servicePrincipal
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: f82140ff1710d9da7c646d2b84f1d83ac4a66150
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134145"
---
# <a name="serviceprincipal-removekey"></a>servicePrincipal: removeKey

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Remova uma credencial de chave de [um servicePrincipal](../resources/serviceprincipal.md). Esse método, [juntamente com addKey,](serviceprincipal-addkey.md) pode ser usado por uma servicePrincipal para automatizar a rolagem de suas chaves expiradas.

> [!NOTE]
> [Criar operações servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) e [Update servicePrincipal](../api/serviceprincipal-update.md) podem continuar a ser usadas para adicionar e atualizar credenciais de chave para qualquer servicePrincipal com ou sem o contexto de um usuário.

Como parte da validação da solicitação para esse método, uma prova de posse de uma chave existente é verificada antes que a ação possa ser executada.

## <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Nenhum.  |
|Delegado (conta pessoal da Microsoft) | Nenhum.    |
|Aplicativo | Nenhum. |

> [!NOTE]
> Uma servicePrincipal não precisa de nenhuma permissão específica para rolar suas próprias chaves.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /serviceprincipals/{id}/removeKey
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
| proof | String | Um token JWT auto-assinado usado como prova de posse das chaves existentes. Esse token JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes do servicePrincipal. O token deve conter os seguintes argumentos:<ul><li>`aud` – A audiência deve ser `00000002-0000-0000-c000-000000000000`.</li><li>`iss` - O emissor precisa ser a __id__  da servicePrincipal que está fazendo a chamada.</li><li>`nbf` – Não antes da hora.</li><li>`exp` – O tempo de expiração deve ser "nbf" + 10 min.</li></ul><br>Aqui está um exemplo [de código](/graph/application-rollkey-prooftoken) que pode ser usado para gerar esse token de comprovação de posse.|

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
POST https://graph.microsoft.com/beta/serviceprincipals/{id}/removeKey
Content-Type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-removekey-javascript-snippets.md)]
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



