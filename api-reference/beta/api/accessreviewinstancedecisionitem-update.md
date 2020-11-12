---
title: Atualizar accessReviewInstanceDecisionItem
description: Atualize um objeto accessReviewInstanceDecisionItem existente que chama o usuário é o revisor de.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2c856cb899cb2379c9d0abf2cd459e289beea82c
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000730"
---
# <a name="update-accessreviewinstancedecisionitem"></a>Atualizar accessReviewInstanceDecisionItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as decisões de acesso, conhecidas como [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md), para as quais o usuário é o revisor.

>[!NOTE]
>Todas as atualizações feitas em um **accessReviewInstanceDecisionItem** só podem ser feitas chamando usuários que estão listados como revisor para o [accessReviewInstance](../resources/accessreviewinstance.md)pai.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é necessária para chamar esta API. Permissões delegadas para contas pessoais da Microsoft não são suportadas. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/pendingAccessReviewInstances/{instance-id}/decisions/{decision-id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Descrição |
|:-------------|:------------|
|Autorização|{token} de portador. Obrigatório.|
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
A tabela a seguir mostra as propriedades aceitas para atualizar um `accessReviewInstanceDecisionItem` .

| Propriedade     | Tipo       | Descrição |
|:-------------|:------------|:------------|
| sobre  | Cadeia de caracteres | Decisão de acesso para a entidade que está sendo revisada. Os valores possíveis são: `Approve` `Deny` `NotReviewed` `DontKnow` . Obrigatório.  |
|  elabora | Cadeia de caracteres | Contexto da revisão fornecida aos administradores. Obrigatório se justificationRequiredOnApproval for true no accessReviewScheduleDefinition.  |

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `204, NoContent` código de resposta e nenhum corpo de resposta.

### <a name="request"></a>Solicitação
## <a name="examples"></a>Exemplos

Este é um exemplo de aprovação de acesso de um usuário representado por um `accessReviewInstanceDecisionItem` .

<!-- {
  "blockType": "request",
  "name": "update_accessReviewInstanceDecisionItem"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions/654b34e7-b48f-4772-a2d4-08f1d0dd014c

{
  "decision": "Approve",
  "justification": "I trust this person"
}
```

---

### <a name="response"></a>Resposta
>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 Accepted
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReviewInstanceDecisionItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
