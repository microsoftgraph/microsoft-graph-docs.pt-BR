---
title: Listar executa
description: Obter uma lista da automação de simulação de ataque executado para um locatário.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 36f0a7375b1aafbaa5eed5ec44b8c47790c2bf0b
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758302"
---
# <a name="list-runs"></a>Listar executa
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista da automação de simulação de ataque executado para um locatário.

## <a name="permissions"></a>Permissions
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
GET /security/attackSimulation/simulationAutomations/{simulationAutomationId}/runs
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos `$count`[parâmetros](/graph/query-parameters) de consulta , `$skiptoken`, `$top`e `$select` OData para ajudar a personalizar a resposta.

Se o conjunto de resultados abrange várias páginas, `@odata.nextLink` o corpo da resposta contém um que você pode usar para página através do conjunto de resultados.

Veja a seguir exemplos de seu uso:

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulationautomations/{simulationAutomationId}/runs?$count=true
GET /security/attackSimulation/simulationautomations/{simulationAutomationId}/runs?$skipToken={skipToken}
GET /security/attackSimulation/simulationautomations/{simulationAutomationId}/runs?$top=1
GET /security/attackSimulation/simulationautomations/{simulationAutomationId}/runs?$select={property}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção [de objetos simulationAutomationRun](../resources/simulationautomationrun.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

<!-- {
  "blockType": "request",
  "name": "list_simulationautomationrun"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/attackSimulation/simulationAutomations/fbad62b0-b32d-b6ac-9f48-d84bbea08f96/runs
```


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.simulationAutomationRun",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.simulationAutomationRun",
      "id": "ac4936a5-3865-a0ec-7254-67a22f6121e2",
      "status": "succeeded",
      "startDateTime": "2021-01-01T02:01:01.01Z",
      "endDateTime": "2021-01-01T02:01:01.01Z",
      "simulationId": "bc4936a5-3865-a0ec-7254-67a22f6121e2"
    }
  ]
}
```

