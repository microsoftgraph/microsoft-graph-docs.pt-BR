---
title: Tipo de recurso teamsAsyncOperation
description: 'Uma Microsoft Teams assíncrona é uma operação que transcende o tempo de vida de uma única solicitação de API. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2db0708ada9bb57ad4f0f88da89c797ff4a4e1e2
ms.sourcegitcommit: 596b3d5636f3f3e042d180ea8f039f00ebd6b38a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2021
ms.locfileid: "53665897"
---
# <a name="teamsasyncoperation-resource-type"></a>Tipo de recurso teamsAsyncOperation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma Microsoft Teams assíncrona é uma operação que transcende o tempo de vida de uma única solicitação de API. Essas operações são de longa duração ou muito caras para concluir dentro do período de tempo de sua solicitação de origem.

Quando uma operação assíncrona é iniciada, o método retorna um código de resposta aceito 202. A resposta também conterá um header Location, que contém o local do teamsAsyncOperation. Verifique periodicamente o status da operação fazendo uma solicitação GET para esse local; aguarde >30 segundos entre verificações.
Quando a solicitação for concluída com êxito, o status será "bem-sucedido" e o targetResourceLocation apontará para o recurso criado/modificado.

## <a name="methods"></a>Métodos

|  Método                                                                   |  Tipo de retorno                                                                     | Descrição                                                       | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :---------------------------------------------------------------- |
| [Listar operações em um chat](../api/chat-list-operations.md)               | Coleção [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Listar operações assíncronas que executam ou estão em execução em um chat específico. |
| [Obter operação](../api/teamsasyncoperation-get.md)                   | Coleção [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Obter uma operação assíncrona que foi executado ou está sendo executado em um recurso específico. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição |
|:---------------|:--------|:----------|
|id|string |ID de operação exclusiva.|
|operationType|[teamsAsyncOperationType](teamsasyncoperationtype.md) |Indica o tipo de operação que está sendo descrito. |
|createdDateTime|DateTimeOffset |Hora em que a operação foi criada.|
|status|[teamsAsyncOperationStatus](teamsasyncoperationstatus.md)| Status da operação.|
|lastActionDateTime|DateTimeOffset |Hora em que a operação assíncrona foi atualizada pela última vez.|
|attemptsCount|Int32|Número de vezes que a operação foi tentada antes de ser marcada com êxito ou falha.|
|targetResourceId|guid |A ID do objeto criado ou modificado como resultado dessa operação assíncrona, normalmente uma [equipe](../resources/team.md).|
|targetResourceLocation|string|O local do objeto criado ou modificado como resultado dessa operação assíncrona. Essa URL deve ser tratada como um valor opaco e não analisado em seus caminhos de componente.|
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
    "operationType": "string",
    "createdDateTime": "string (timestamp)",
    "status": "string",
    "lastActionDateTime": "string (timestamp)",
    "attemptsCount": "Integer",
    "targetResourceId": "string",
    "targetResourceLocation": "string",
    "error": null
}
```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


