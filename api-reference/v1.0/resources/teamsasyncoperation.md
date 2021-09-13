---
title: Tipo de recurso teamsAsyncOperation
description: 'Uma Microsoft Teams assíncrona transcende o tempo de vida de uma única solicitação de API. '
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a061ba8951013c12e825141f5a205c3e6d664733
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59071893"
---
# <a name="teamsasyncoperation-resource-type"></a>Tipo de recurso teamsAsyncOperation

Namespace: microsoft.graph



Uma Microsoft Teams assíncrona é uma operação que transcende o tempo de vida de uma única solicitação de API. Essas operações são de longa duração ou muito caras para concluir dentro do período de tempo de sua solicitação de origem.

Quando uma operação assíncrona é iniciada, o método retorna um código de resposta aceito 202. A resposta também conterá um header Location, que contém o local do teamsAsyncOperation. Verifique periodicamente o status da operação fazendo uma solicitação GET para esse local; aguarde >30 segundos entre verificações.
Quando a solicitação for concluída com êxito, o status será "bem-sucedido" e o targetResourceLocation apontará para o recurso criado/modificado.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição |
|:---------------|:--------|:----------|
|id|cadeia de caracteres |ID de operação exclusiva.|
|operationType|[teamsAsyncOperationType](teamsasyncoperationtype.md) |Indica qual tipo de operação está sendo descrito.|
|createdDateTime|DateTimeOffset |Hora em que a operação foi criada.|
|status|[teamsAsyncOperationStatus](teamsasyncoperationstatus.md)| Status da operação.|
|lastActionDateTime|DateTimeOffset |Hora em que a operação assíncrona foi atualizada pela última vez.|
|attemptsCount|Int32|Número de vezes que a operação foi tentada antes de ser marcada com êxito ou falha.|
|targetResourceId|guid |A ID do objeto criado ou modificado como resultado dessa operação assíncrona, normalmente uma [equipe](../resources/team.md).|
|targetResourceLocation|cadeia de caracteres|O local do objeto criado ou modificado como resultado dessa operação assíncrona. Essa URL deve ser tratada como um valor opaco e não analisado em seus caminhos de componente.|
|erro|[operationError](operationerror.md)|Qualquer erro que cause falha na operação assíncrona.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsAsyncOperation"
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

