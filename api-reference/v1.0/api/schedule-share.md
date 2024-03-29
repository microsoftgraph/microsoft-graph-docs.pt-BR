---
title: 'schedule: share'
description: Compartilhe um intervalo de tempo de agendamento com membros de agendamento.
author: akumar39
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b0fe3490060835d2144745f1be562530cac1734a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347168"
---
# <a name="schedule-share"></a>schedule: share

Namespace: microsoft.graph

Compartilhe um [intervalo de](../resources/schedule.md) tempo de agendamento com membros de agendamento.
Faça com que as coleções de itens [shift](../resources/shift.md), [openshift](../resources/openshift.md) e [timeOff](../resources/timeoff.md) no intervalo de tempo especificado do [](../resources/schedule.md) cronograma sejam visualizadas pelos membros da equipe especificados, incluindo funcionários e gerentes.
Cada [turno](../resources/shift.md), [instância openshift](../resources/openshift.md) [e timeOff](../resources/timeoff.md) em um [cronograma](../resources/schedule.md) oferece suporte a uma versão de rascunho e uma versão compartilhada do item. A versão de rascunho pode ser visualizada somente por gerentes, e a versão compartilhada pode ser visualizada por funcionários e gerentes. Para cada [turno](../resources/shift.md), [instância openshift](../resources/openshift.md) e [timeOff](../resources/timeoff.md) no intervalo de tempo especificado, a ação de compartilhamento atualiza a versão compartilhada da versão de rascunho, para que, além dos gerentes, os funcionários também possam exibir as informações mais atuais sobre o item. O **parâmetro notifyTeam** especifica ainda quais funcionários podem exibir o item.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Schedule.ReadWrite.All, Group.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Schedule.ReadWrite.All |

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
| notifyTeam            |`Boolean`             |Indica se toda a equipe deve receber uma notificação visível dessa ação ou apenas os funcionários que têm um turno atribuído a eles que foi compartilhado. Obrigatório.       |
| startDateTime         |`DateTimeOffset`   |A hora de início para compartilhar turnos no agendamento de. Obrigatório.   |
| endDateTime           |`DateTimeOffset`   | A hora de término para compartilhar turnos na agenda até.   |

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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/schedule-share-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/schedule-share-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a>Resposta

Este é um exemplo de resposta. 

<!-- {
  "blockType": "response",
  "truncated": true
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

