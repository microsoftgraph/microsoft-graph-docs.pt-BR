---
title: tipo de recurso teamsAsyncOperation
description: 'Uma operação assíncrona do Microsoft Teams transcende o tempo de vida de uma única solicitação de API. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 61173f92b6aa74d0a703366140f17f983d94c855
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873276"
---
# <a name="teamsasyncoperation-resource-type"></a>tipo de recurso teamsAsyncOperation

Namespace: microsoft.graph



Uma operação assíncrona do Microsoft Teams é uma operação que transcende o tempo de vida de uma única solicitação de API. Essas operações são de longa duração ou muito caras para concluir dentro do prazo de sua solicitação de origem.

Quando uma operação assíncrona é iniciada, o método retorna um código de resposta aceito 202. A resposta também conterá um cabeçalho de local, que contém o local do teamsAsyncOperation. Verifique periodicamente o status da operação fazendo uma solicitação GET para este local; Aguarde >30 segundos entre as verificações.
Quando a solicitação for concluída com êxito, o status será "bem-sucedido" e o targetResourceLocation apontará para o recurso criado/modificado.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição |
|:---------------|:--------|:----------|
|id|cadeia de caracteres |ID de operação exclusiva.|
|OperationType|[teamsAsyncOperationType](teamsasyncoperationtype.md) |Indica o tipo de operação que está sendo descrito.|
|createdDateTime|DateTimeOffset |Hora em que a operação foi criada.|
|status|[teamsAsyncOperationStatus](teamsasyncoperationstatus.md)| Status da operação.|
|lastActionDateTime|DateTimeOffset |Hora em que a operação assíncrona foi atualizada pela última vez.|
|attemptsCount|Int32|Número de vezes em que a operação foi tentada antes de ser marcada com êxito ou falhou.|
|targetResourceId|#c0 |A ID do objeto que é criado ou modificado como resultado dessa operação assíncrona, normalmente uma [equipe](../resources/team.md).|
|targetResourceLocation|cadeia de caracteres|O local do objeto que é criado ou modificado como resultado dessa operação assíncrona. Essa URL deve ser tratada como um valor opaco e não analisada em seus caminhos de componente.|
|erro|[operationError](operationerror.md)|Qualquer erro que causa falha na operação assíncrona.|

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
