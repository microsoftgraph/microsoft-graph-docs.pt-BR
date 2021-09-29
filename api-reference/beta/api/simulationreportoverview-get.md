---
title: Obter visão geral do relatório de simulação.
description: Obter visão geral do relatório para uma campanha de simulação de ataque.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: d2d74d5a5b3004632df63ef82641bda85f674ec3
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995365"
---
# <a name="get-simulationreportoverview"></a>Obter simulationReportOverview
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma visão geral de uma campanha de simulação e treinamento de ataque.

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
GET /security/attackSimulation/simulations/{id}/report/overview
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto simulationReportOverview](../resources/simulationreportoverview.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_simulationreportoverview"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/attackSimulation/simulations/{id}/report/overview
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-simulationreportoverview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-simulationreportoverview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-simulationreportoverview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-simulationreportoverview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.simulationReportOverview"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "microsoft.graph.simulationReportOverview",
  "resolvedTargetsCount": 1,
  "simulationEventsContent": {
    "compromisedRate": 100.0,
    "events": [
      {
        "@odata.type": "microsoft.graph.simulationEvent",
        "eventName": "SuccessfullyDeliveredMail",
        "count": 1
      },
      {
        "@odata.type": "microsoft.graph.simulationEvent",
        "eventName": "ReportedEmail",
        "count": 0
      },
      {
        "@odata.type": "microsoft.graph.simulationEvent",
        "eventName": "EmailLinkClicked",
        "count": 1
      }
    ]
  },
  "trainingEventsContent": {
    "trainingsAssignedUserCount": 1,
    "assignedTrainingsInfos": [
      {
        "@odata.type": "microsoft.graph.assignedTrainingsInfo",
        "assignedUserCount": 1,
        "completedUserCount": 0,
        "displayName": "Sample Training"
      }
    ]
  },
  "recommendedActions": [
    {
      "@odata.type": "microsoft.graph.recommendedAction",
      "actionWebUrl": "https://recommendedSecurityAction.com",
      "title": "Sample Recommended Security Feature",
      "potentialScoreImpact": 5.0
    }
  ]
}
```

