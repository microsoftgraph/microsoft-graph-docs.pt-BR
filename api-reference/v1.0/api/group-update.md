---
title: Atualizar grupo
description: Atualizar as propriedades de um objeto group.
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1e92b738ffac9d04eaa02b0130e902609d3f944a
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51467985"
---
# <a name="update-group"></a>Atualizar grupo

Namespace: microsoft.graph

Atualizar as propriedades de um objeto group.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All  |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Group.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolean|O padrão é `false`. Indica se as pessoas externas à empresa podem enviar mensagens para o grupo.|
|autoSubscribeNewMembers|Boolean|O padrão é `false`. Indica se novos membros adicionados ao grupo serão automaticamente inscritos para receberem notificações por email. **autoSubscribeNewMembers** não pode ser `true` quando **subscriptionEnabled** é definido como `false` no grupo.|
|descrição|String|Uma descrição opcional para o grupo. |
|displayName|Cadeia de caracteres|O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações. |
|groupTypes|Coleção de cadeias de caracteres|Especifica o tipo de grupo e sua associação.  <br><br>Se a coleção contiver um grupo **unificado** então o grupo será um grupo do Microsoft 365; caso contrário, será um grupo de segurança.  <br><br>Se a coleção incluir **DynamicMembership**, o grupo tem associação dinâmica; caso contrário, a associação é estática. |
|mailEnabled|Boolean|Especifica se o grupo está habilitado para email.|
|mailNickname|String|O alias de email do grupo. Essa propriedade deve ser especificada quando um grupo é criado. |
|securityEnabled|Boolean|Especifica se o grupo é um grupo de segurança. |
|visibility|Cadeia de caracteres|Especifica a visibilidade de um grupo do Microsoft 365. Os valores possíveis são: **Privado**, **Público** ou vazio (que é interpretado como **Público**).|

> **Observação:**
>
> - Você pode atualizar o **autoSubscribeNewMembers** e **autoSubscribeNewMembers** especificando-os em sua própria solicitação de PATCH, sem incluir as outras propriedades na tabela acima.
> - Apenas um subconjunto da API de grupo relacionado à administração do grupo principal e ao aplicativo de suporte para gerenciamento às permissões delegadas. Todos os outros membros da API do grupo, inclusive a atualização **autoSubscribeNewMembers**, dão suporte apenas a permissões delegadas. Confira exemplos nos [problemas conhecidos](/graph/known-issues#groups).
> - As regras para atualizar os grupos de segurança habilitados para email no Microsoft Exchange Server podem ser complexas; Para saber mais, confira [Gerenciar grupos de segurança habilitados para email no Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).

## <a name="response"></a>Resposta

Se for bem-sucedido, este método retorna um código de resposta `204 No Content`, exceto um código de resposta `200 OK` ao atualizar as seguintes propriedades: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra como atualizar um grupo.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}
Content-type: application/json
Content-length: 211

{
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
