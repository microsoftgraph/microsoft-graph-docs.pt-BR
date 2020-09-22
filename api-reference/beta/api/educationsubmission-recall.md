---
title: 'educationSubmission: rechamar'
description: 'Indica que um aluno deseja fazer um envio. Esta ação só pode ser feita por um aluno. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 606a2a5325da9aed6203303e40ad5b3b95f0d7d6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007228"
---
# <a name="educationsubmission-recall"></a>educationSubmission: rechamar

Namespace: Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica que um aluno deseja fazer um envio. Esta ação só pode ser feita por um aluno. Ele alterará o status do envio de "enviado" de volta para "trabalho".

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)             |
| :------------------------------------- | :------------------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte                                           |
| Aplicativo                            | Sem suporte.                                          |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/recall
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor                     |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra como chamar essa API.

##### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: recall",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


