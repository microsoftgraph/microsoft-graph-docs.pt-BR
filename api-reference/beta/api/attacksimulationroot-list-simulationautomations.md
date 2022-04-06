---
title: Listar simulationAutomations
description: Obter uma lista de automações de simulação de ataque para um locatário.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 13bdd574c1b783992b27144ded3ab3a31f2da5a7
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758304"
---
# <a name="list-simulationautomations"></a>Listar simulationAutomations
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista de automações de simulação de ataque para um locatário.

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
GET /security/attackSimulation/simulationAutomations
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos `$count`[parâmetros](/graph/query-parameters) de consulta , `$filter`, `$orderby`, `$skip`, `$top`e `$select` OData para ajudar a personalizar a resposta. Você pode usar os parâmetros `$filter` e `$orderby` de consulta nas **propriedades displayName** e **status** .

Se o conjunto de resultados abrange várias páginas, `@odata.nextLink` o corpo da resposta contém um que você pode usar para página através do conjunto de resultados.

Veja a seguir exemplos de seu uso:

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulationAutomations?$count=true
GET /security/attackSimulation/simulationAutomations?$filter={property} eq '{property-value}'
GET /security/attackSimulation/simulationAutomations?$filter={property} eq '{property-value}'&$top=5
GET /security/attackSimulation/simulationAutomations?$orderby={property}
GET /security/attackSimulation/simulationAutomations?$skip={skipCount}
GET /security/attackSimulation/simulationAutomations?$top=1
GET /security/attackSimulation/simulationAutomations?$select={property}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de [objetos simulationAutomation](../resources/simulationautomation.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

Veja a seguir um exemplo de uma solicitação.

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "list_simulationautomation"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/attackSimulation/simulationAutomations
```


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.simulationAutomation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.simulationAutomation",
      "id": "fbad62b0-b32d-b6ac-9f48-d84bbea08f96",
      "displayName": "Reed Flores",
      "description": "Sample Simulation Automation Description",
      "status": "running",
      "createdDateTime": "2022-01-01T01:01:01.01Z",
      "createdBy": {
        "id": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Reed Flores",
        "email": "reed@contoso.com"
      },
      "lastModifiedDateTime": "2022-01-01T01:01:01.01Z",
      "lastModifiedBy": {
        "id": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Reed Flores",
        "email": "reed@contoso.com"
      },
      "lastRunDateTime": "2022-01-01T01:01:01.01Z",
      "nextRunDateTime": "2022-01-01T01:01:01.01Z"
    }
  ]
}
```

