---
title: Atualizar workforceintegration
description: Atualize as propriedades de um objeto workforceintegration.
ms.localizationpriority: medium
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6fcfe75b2ee2d39a3142c952d6218da31c8b36df
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031216"
---
# <a name="update-workforceintegration"></a>Atualizar workforceintegration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um [objeto workforceintegration.](../resources/workforceintegration.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | WorkforceIntegration.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:-----------|
| Autorização | Portador {token} |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|apiVersion|Int32|Versão da API para a URL de retorno de chamada. Comece com 1.|
|displayName|Cadeia de caracteres|Nome da integração da força de trabalho.|
|encryption|workforceIntegrationEncryption|O recurso de criptografia de integração de força de trabalho. |
|isActive|Booliano|Indica se essa integração de força de trabalho está ativa e disponível no momento.|
|suporta|string| Os valores possíveis `none` são , , , , , `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` . Se selecionar mais de um valor, todos os valores devem começar com a primeira letra em maiúscula.|
|supportedEntities|string| Essa propriedade substituirá **os suportes** em v1.0. Recomendamos que você use essa propriedade em vez de **suporte**. A **propriedade supports** ainda terá suporte na versão beta por enquanto. Os valores possíveis `none` são , , , , , `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` . Se selecionar mais de um valor, todos os valores devem começar com a primeira letra em maiúscula.|
|url|Cadeia de caracteres| Url de Integração de Força de Trabalho para retornos de chamada do serviço Shift. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [workforceIntegration](../resources/workforceintegration.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-update-a-workforceintegration-object"></a>Exemplo 1: Atualizar um objeto workforceIntegration

O exemplo a seguir atualiza um **objeto workforceIntegration.**

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}-->

```http
PATCH https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceIntegrationId}
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-workforceintegration-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```

### <a name="example-2-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a>Exemplo 2: Criar uma nova workforceIntegration com SwapRequest habilitada para filtragem de qualificação

O exemplo a seguir cria uma nova **workforceIntegration** com SwapRequest habilitada para filtragem de qualificação.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. 
```
POST https://graph.microsoft.com/beta/teamwork/workforceIntegrations/
Authorization: Bearer {token}
Content-type: application/json

{
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": "My Secret"
  },
  "url": "https://ABCWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}

```
#### <a name="response"></a>Resposta

Este é um exemplo de resposta.
```
HTTP/1.1 200 OK
{
  "id": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": null
  },
  "url": "https://abcWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}

```
Para criar uma nova **workforceIntegration** com SwapRequest habilitado para filtragem de qualificação, consulte o [método Create.](../api/workforceintegration-post.md)

### <a name="example-3-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a>Exemplo 3: buscar turnos qualificados quando SwapRequest está incluído em eligibilityFilteringEnabledEntities

A interação entre o aplicativo Shifts e os pontos de extremidade de integração da força de trabalho seguirá o padrão existente.

#### <a name="request"></a>Solicitação

A seguir, um exemplo da solicitação feita por Shifts para o ponto de extremidade de integração da força de trabalho para buscar turnos qualificados para uma solicitação de troca.

```
POST https://abcWorkforceIntegration.com/Contoso/{apiVersion}/team/{teamId}/read
Accept-Language: en-us

{
  "requests": [
  {
     "id": "{shiftId}",
     "method": "GET”,
     "url": “/shifts/{shiftId}/requestableShifts?requestType={requestType}&startDateTime={startDateTime}&endDateTime={endDateTime}”
   }]
}
```
#### <a name="response"></a>Resposta

A seguir, um exemplo da resposta do serviço de integração da força de trabalho.
```
HTTP/1.1 200 OK
{
  "responses": [
  {
    "body": {
      "SHFT_6548f642-cbc1-4228-8621-054327576457",
      "SHFT_6548f642-cbc1-4228-8621-054327571234"
  }
    "id": "{shiftId}",
    "status: 200,
    "body": {
       "data": [{ShiftId}, {ShiftId}...]
       "error": null
    }
  ]
}
```

### <a name="example-4-shifts-synchronous-call-back-to-the-workforce-integration-endpoint-when-enabled-for-real-time-notifications-on-timecard-changes"></a>Exemplo 4: altera a chamada síncrona de volta para o ponto de extremidade de integração da força de trabalho quando habilitada para notificações em tempo real em alterações do timeCard.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. 
```
POST https://foobarWorkforceIntegration.com/foobar/v1/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/update
Accept-Language: en-us
X-MS-WFMPassthrough: foobarvalue
Content-type: application/json
{
   "requests":[
      {
         "id":"1",
         "method":"POST",
         "url":"/timecards",
         "headers":{
            "X-MS-Transaction-ID":"1"
         },
         "body":{
            "id":"3895809b-a618-4c0d-86a0-d42b25b7d74f",
            "userId":"a3601044-a1b5-438e-b742-f78d01d68a67",
            "createdDateTime":"2019-03-18T00:00:00.000Z",
            "createdBy":{
               "user":{
                  "id":"a3601044-a1b5-438e-b742-f78d01d68a67",
                  "displayName":"Dwight Schrute"
               }
            },
            "lastModifiedDateTime":"2019-03-18T00:00:00.000Z",
            "lastModifiedBy":{
               "user":{
                  "id":"a3601044-a1b5-438e-b742-f78d01d68a67",
                  "displayName":"Dwight Schrute"
               }
            },
            "state":"onBreak",
            "clockIn":{
               "dateTime":"2019-03-18T00:00:00.000Z",
               "atApprovedLocation":true,
               "notes":null
            },
            "clockOut":null,
            "breaks":[
               {
                  "id":"string",
                  "notes":{
                     "content":"Lunch break",
                     "contentType":"text"
                  },
                  "start":{
                     "dateTime":"2019-03-18T00:00:00.000Z",
                     "atApprovedLocation":true,
                     "notes":{
                        "content":"Started my break 5 minutes early",
                        "contentType":"text"
                     }
                  },
                  "end":null
               }
            ],
            "notes":null,
            "originalEntry":{
               "clockIn":{
                  "dateTime":"2019-03-18T00:00:00.000Z",
                  "atApprovedLocation":true,
                  "notes":null
               },
               "clockOut":null,
               "breaks":[
                  {
                     "id":"4591109b-a618-3e0d-e6a0-d42b25b7231f",
                     "notes":{
                        "content":"Lunch break",
                        "contentType":"text"
                     },
                     "start":{
                        "dateTime":"2019-03-18T00:00:00.000Z",
                        "atApprovedLocation":true,
                        "notes":{
                           "content":"Started my break 5 minutes early",
                           "contentType":"text"
                        }
                     },
                     "end":null
                  }
               ]
            }
         }
      }
   ]
}

```
#### <a name="response"></a>Resposta

Este é um exemplo de resposta.
```
HTTP/1.1 200 OK
Content-type: application/json
{
  "responses":[
    {
      "id": "1",
      "status": 200,
      "body":{
        "eTag": "4000ee23-0000-0700-0000-5d1415f60000",
        "error": null
      }
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update workforceintegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


