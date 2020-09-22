---
title: 'agendamento: share'
description: Compartilhar um intervalo de tempo de agendamento com membros de agendamento.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 054a6dd0589929c22c7dc6b8c5e954dee360bef2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015656"
---
# <a name="schedule-share"></a>agendamento: share

Namespace: microsoft.graph

Compartilhar um intervalo de tempo de [agendamento](../resources/schedule.md) com membros de agendamento.
Faça as coleções de itens [Shift](../resources/shift.md), [openshift](../resources/openshift.md) e [timeOff](../resources/timeoff.md) no intervalo de tempo especificado da [agenda](../resources/schedule.md) exibida pelos membros da equipe especificados, incluindo funcionários e gerentes.
Cada [mudança](../resources/shift.md), [openshift](../resources/openshift.md) e [timeOff](../resources/timeoff.md) instância em um [cronograma](../resources/schedule.md) suporta uma versão de rascunho e uma versão compartilhada do item. A versão de rascunho é visível apenas por gerentes e a versão compartilhada é visível por funcionários e gerentes. Para cada [mudança](../resources/shift.md), [openshift](../resources/openshift.md) e [timeOff](../resources/timeoff.md) instância no intervalo de tempo especificado, a ação de compartilhamento atualiza a versão compartilhada da versão de rascunho, para que, além dos gerentes, os funcionários também possam exibir as informações mais recentes sobre o item. O parâmetro **notifyTeam** especifica ainda mais quais funcionários podem exibir o item.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Schedule. ReadWrite. All, Group. ReadWrite. All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Schedule.ReadWrite.All |

> **Observação**: esta API oferece transporte a permissões de administrador. Os administradores globais podem acessar grupos dos quais eles não são membros.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

|Parâmetro                   |Tipo           |Descrição  |
|-----------------------|-------------------|--------------|
| notifyTeam            |`Boolean`             |Indica se a equipe inteira deve receber uma notificação visível desta ação ou apenas os funcionários que têm uma alteração atribuída a elas que foram compartilhadas. Obrigatório.       |
| startDateTime         |`DateTimeOffset`   |O horário de início para compartilhar as mudanças no cronograma. Obrigatório.   |
| endDateTime           |`DateTimeOffset`   | O horário de término para compartilhar turnos no cronograma até.   |

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-share"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/share
Content-type: application/json

{
  "notifyTeam": true,
  "startDateTime": "2018-10-08T00:00:00.000Z",
  "endDateTime": "2018-10-15T00:00:00.000Z"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-share-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-share-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-share-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-share-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a>Resposta

Este é um exemplo de resposta. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Shares a time-range of the schedule with the schedule members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

