---
title: 'reportRoot: getAttackSimulationTrainingUserCoverage'
description: Listar cobertura de treinamento para usuários de um locatário em campanhas de treinamento e simulação de ataques.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: ddda75fe00fa548ffc2ac7e01492e6a0864a73ec
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979501"
---
# <a name="reportroot-getattacksimulationtrainingusercoverage"></a>reportRoot: getAttackSimulationTrainingUserCoverage
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Listar [cobertura de treinamento](../resources/attacksimulationtrainingusercoverage.md) para cada usuário de um locatário em campanhas de simulação e treinamento de ataques.

Esta função é `@odata.nextLink` compatível com paginação.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | Reports.Read.All                            |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | Reports.Read.All                            |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/getAttackSimulationTrainingUserCoverage
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará um código de resposta e uma `200 OK` [coleção attackSimulationTrainingUserCoverage](../resources/attacksimulationtrainingusercoverage.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "reportroot_getattacksimulationtrainingusercoverage"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getAttackSimulationTrainingUserCoverage
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.attackSimulationTrainingUserCoverage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "userTrainings": [
        {
          "assignedDateTime": "2021-01-01T01:01:01.01Z",
          "completionDateTime": "2021-01-02T01:01:01.01Z",
          "trainingStatus": "Completed",
          "displayName": "Sample Training"
        }
      ],
      "attackSimulationUser": {
        "userId": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Sample User",
        "email": "sampleuser@contoso.com"
      }
    }
  ]
}
```

