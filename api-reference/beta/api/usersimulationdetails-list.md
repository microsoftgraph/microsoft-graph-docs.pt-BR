---
title: Listar usuários de simulação
description: Listar usuários de um locatário em uma campanha de simulação de ataque com suas ações online.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: ecb3bcc46b57cbd6b5afd3f0f698fba3da5ef436
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996659"
---
# <a name="list-simulationusers"></a>Listar simulationUsers
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Listar usuários de um locatário e suas ações online em uma campanha de simulação de ataque.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | SecurityEvents.Read.All                     |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | SecurityEvents.Read.All                     |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulations/{id}/report/simulationUsers
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta: `$count` , `$skiptoken` , `$top` .

Use `@odata.nextLink` para paginação.

Veja a seguir exemplos de seu uso:

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulations/{id}/report/simulationUsers?$top=1
GET /security/attackSimulation/simulations/{id}/report/simulationUsers?$count=true
```

Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos userSimulationDetails](../resources/usersimulationdetails.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usersimulationdetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/attackSimulation/simulations/{id}/report/simulationUsers
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usersimulationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usersimulationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usersimulationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usersimulationdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userSimulationDetails)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "isCompromised": true,
      "compromisedDateTime": "2021-01-01T01:02:01.01Z",
      "simulationEvents": [
        {
          "eventName": "SuccessfullyDeliveredEmail",
          "eventDateTime": "2021-01-01T01:01:01.01Z",
          "ipAddress": "100.200.100.200",
          "osPlatformDeviceDetails": "Sample OS",
          "browser": "Sample Browser"
        },
        {
          "eventName": "EmailLinkClicked",
          "eventDateTime": "2021-01-01T01:02:01.01Z",
          "ipAddress": "100.200.100.200",
          "osPlatformDeviceDetails": "Sample OS",
          "browser": "Sample Browser"
        }
      ],
      "trainingEvents": [
        {
          "displayName": "Sample Training",
          "latestTrainingStatus": "assigned",
          "trainingAssignedProperties": {
            "contentDateTime": "2021-01-01T01:03:01.01Z",
            "ipAddress": "100.200.100.200",
            "osPlatformDeviceDetails": "Sample OS",
            "browser": "Sample Browser",
            "potentialScoreImpact": 5.0
          },
          "trainingUpdatedProperties": {
            "contentDateTime": "2021-01-01T01:04:01.01Z",
            "ipAddress": "100.200.100.201",
            "osPlatformDeviceDetails": "Sample OS-2",
            "browser": "Sample Browser",
            "potentialScoreImpact": 5.0
          },
          "trainingCompletedProperties": {
            "contentDateTime": "2021-01-01T01:05:01.01Z",
            "ipAddress": "100.200.100.202",
            "osPlatformDeviceDetails": "Sample OS",
            "browser": "Sample Browser-2",
            "potentialScoreImpact": 5.0
          }
        }
      ],
      "assignedTrainingsCount": 1,
      "completedTrainingsCount": 0,
      "inProgressTrainingsCount": 0,
      "reportedPhishDateTime": "2021-01-01T01:01:01.01Z",
      "simulationUser": {
        "userId": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Sample User",
        "email": "sampleuser@contoso.com"
      }
    }
  ]
}
```

