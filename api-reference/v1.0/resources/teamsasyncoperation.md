---
title: tipo de recurso de teamsAsyncOperation
description: 'Uma operação assíncrona de Teams da Microsoft é uma operação que transcende o tempo de vida de uma única solicitação de API. '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 607730ff48213b45177560046dc6f38afe1bcc75
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873616"
---
# <a name="teamsasyncoperation-resource-type"></a>tipo de recurso de teamsAsyncOperation



Uma operação assíncrona de Teams da Microsoft é uma operação que transcende o tempo de vida de uma única solicitação de API. Essas operações são muito caro concluir dentro do período de tempo de sua solicitação de origem ou de longa execução.

Quando é iniciada uma operação assíncrona, o método retornará um código de resposta 202 aceitos. A resposta conterá também um cabeçalho de local, que contém a localização do teamsAsyncOperation. Verificar periodicamente o status da operação, tornando uma solicitação GET para este local; Aguarde > 30 segundos entre as verificações.
Quando a solicitação for concluída com êxito, o status será "sucedido" e o targetResourceLocation apontará para o recurso criado/modificado.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição |
|:---------------|:--------|:----------|
|id|string |Id exclusiva de operação.|
|operationType|[teamsAsyncOperationType](teamsasyncoperationtype.md) |Indica qual tipo de operação está sendo descrito.|
|createdDateTime|DateTimeOffset |Hora em que a operação foi criada.|
|status|[teamsAsyncOperationStatus](teamsasyncoperationstatus.md)| Status de operação.|
|lastActionDateTime|DateTimeOffset |Hora de quando a operação assíncrona foi atualizada pela última vez.|
|attemptsCount|Int32|Número de vezes que a operação foi tentada antes de serem marcadas com êxito ou falha.|
|targetResourceId|GUID |A identificação do objeto que tenha criado ou modificado como resultado dessa operação assíncrona, geralmente uma [equipe](../resources/team.md).|
|targetResourceLocation|string|O local do objeto que tenha criado ou modificado como resultado dessa operação assíncrona. Essa URL deve ser tratado como um valor opaco e não analisado em caminhos de seus componentes.|
|erro|[operationError](operationerror.md)|Qualquer erro que faz com que a operação assíncrona falhe.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsasyncoperation"
}-->

```json
{
    "id": "string",
    "operationType": "archiveTeam",
    "createdDateTime": "2018-01-01T00:00:00.0000000Z",
    "status": "succeeded",
    "lastActionDateTime": "2018-01-01T00:00:00.0000000Z",
    "attemptsCount": 1,
    "targetResourceId": "fa4aa5a2-a75b-4769-86f4-9e2742a18fda",
    "targetResourceLocation": "/groups('fa4aa5a2-a75b-4769-86f4-9e2742a18fda')/team",
    "error": null
}
```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
