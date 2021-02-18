---
title: Listar openShiftChangeRequests
description: Recupere uma lista de objetos openShiftChangeRequest em uma equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 40eef8348138f974a1a9f6c6d7f5dea180477307
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292347"
---
# <a name="list-openshiftchangerequests"></a>Listar openShiftChangeRequests

Namespace: microsoft.graph

Recupere uma lista de [objetos openShiftChangeRequest](../resources/openshiftchangerequest.md) em uma equipe.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Schedule.Read.All, Schedule.ReadWrite.All |

> **Observação**: esta API oferece transporte a permissões de administrador. Os administradores globais podem acessar grupos dos que não são membros.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShiftChangeRequests
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta e a lista de `200 OK` [objetos openShiftChangeRequest](../resources/openshiftchangerequest.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "get_openshiftchangerequest"
}-->

```http
GET https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShiftChangeRequests
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShiftChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [{
        "id": "SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09",
        "openShiftId": "577b75d2-a927-48c0-a5d1-dc984894e7b8",
        "assignedTo": "manager",
        "state": "pending",
        "senderUserId": "3fe0bc21-1398-4fd9-9713-52511b434c1e",
        "senderDateTime": "2019-05-01T10:00:00Z",
        "senderMessage": "Can I take this shift?",
        "managerUserId": null,
        "managerActionDateTime": null,
        "managerActionMessage": null,
        "createdDateTime": "2019-03-14T04:32:51.451Z",
        "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "conversation": null,
            "user": {
                "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
                "displayName": "John Doe"
            }
        }
    }]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List openShiftChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

