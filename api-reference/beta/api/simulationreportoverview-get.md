---
title: Obter visão geral do relatório de simulação.
description: Obter visão geral do relatório para uma campanha de simulação de ataque.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: c50d2627aea65b93efa57263db669514d6697154
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979464"
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
| Delegada (conta pessoal da Microsoft) | Sem suporte.                              |
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
<!-- {
  "blockType": "request",
  "name": "get_simulationreportoverview"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/attackSimulation/simulations/{id}/report/overview
```


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

