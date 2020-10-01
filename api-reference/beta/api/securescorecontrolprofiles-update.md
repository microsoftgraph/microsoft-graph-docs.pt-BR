---
title: Atualizar secureScoreControlProfiles
description: Atualize uma propriedade secureScoreControlProfiles editável em qualquer solução integrada para alterar várias propriedades, como assignedTo ou tenantNote.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 6d3df08c36a7a59e4502164ac1f89c85268d0a01
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330190"
---
# <a name="update-securescorecontrolprofiles"></a>Atualizar secureScoreControlProfiles

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize uma propriedade **secureScoreControlProfiles** editável em qualquer solução integrada para alterar várias propriedades, como **assignedTo** ou **tenantNote**.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |   SecurityEvents.ReadWrite.All  |
|Delegado (conta pessoal da Microsoft) |  Sem suporte.  |
|Aplicativo | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:-----------|
| Autorização  | Portador {código}. Obrigatório.|
|Preferir | Return = representação. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON dos valores de campos relevantes que devem ser atualizados. A tabela a seguir lista os campos que podem ser atualizados para um secureScoreControlProfile. Os valores das propriedades existentes que não estão incluídas no corpo da solicitação não serão alterados. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|assignedTo|Cadeia de caracteres|Nome do analista ao qual o controle é atribuído para a triagem, implementação ou correção.|
|tenantNote|Cadeia de caracteres|Comentários de analista sobre o controle (para o gerenciamento de controle de clientes).|
|controlStateUpdates| Cadeia de caracteres|Configuração orientada pelo analista no controle. Os valores possíveis são: `ignore`, `thirdParty`, `reviewed`.|


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

Se o cabeçalho de solicitação opcional for usado, o método retornará um `200 OK` código de resposta e o objeto [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/secureScoreControlProfiles/AdminMFA
Content-type: application/json

{
  "controlStateUpdates": "controlStateUpdates-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Veja a seguir o exemplo de uma resposta bem-sucedida.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 204 No Content
```




<!--
{
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


