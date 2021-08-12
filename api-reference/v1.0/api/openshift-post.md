---
title: Criar openShift
description: Crie uma instância do objeto openShift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f548b2ed0b0f99844f362260bf52d673d0930e77fbc6e06d34d83104cc2194fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54175543"
---
# <a name="create-openshift"></a>Criar openShift

Namespace: microsoft.graph

Crie uma instância de um [objeto openShift.](../resources/openshift.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Schedule.ReadWrite.All, Group.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Schedule.ReadWrite.All |

> **Observação**: esta API oferece transporte a permissões de administrador. Os administradores globais podem acessar grupos dos que não são membros.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShifts
```
  
## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | {token} de portador. Obrigatório. |
| Content-type | application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Forneça o novo [objeto openShift](../resources/openshift.md) no corpo da solicitação para este método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [openShift](../resources/openshift.md) criado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/openshifts
Authorization: Bearer {token}
Content-type: application/json
Content-length: 244

{
   "id":"OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
   "schedulingGroupId":"TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
   "sharedOpenShift":{
      "notes":"InventoryManagement",
      "openSlotCount":2,
      "displayName":"Dayshift",
      "startDateTime":"2018-10-04T00: 58: 45.340Z",
      "endDateTime":"2018-10-04T09: 50: 45.332Z",
      "theme":"white",
      "activities":[
         {
            "isPaid":true,
            "startDateTime":"2018-10-04T00: 58: 45.340Z",
            "endDateTime":"2018-10-04T01: 58: 45.340Z",
            "code":"",
            "displayName":"Lunch"
         }
      ]
   },
   "draftOpenShift":null,
   "createdDateTime":"2019-03-14T04: 32: 51.451Z",
   "lastModifiedDateTime":"2019-03-14T05: 32: 51.451Z",
   "lastModifiedBy":{
      "application":null,
      "device":null,
      "conversation":null,
      "user":{
         "id":"366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
         "displayName":"JohnDoe"
      }
   }
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
    "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
    "sharedOpenShift": {
    "notes": "Inventory Management",
    "openSlotCount":2,
    "displayName": "Day shift",
    "startDateTime": "2018-10-04T00:58:45.340Z",
    "endDateTime": "2018-10-04T09:50:45.332Z",
    "theme": "white",
    "activities": [
    {
    "isPaid": true,
    "startDateTime": "2018-10-04T00:58:45.340Z",
    "endDateTime": "2018-10-04T01:58:45.340Z",
    "code": "",
    "displayName": "Lunch"
    }
    ]
    },
    "draftOpenShift": null,
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
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

