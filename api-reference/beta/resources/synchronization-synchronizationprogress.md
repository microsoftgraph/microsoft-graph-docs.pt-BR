---
title: tipo de recurso synchronizationProgress
description: Representa o andamento de um synchronizationJob para a conclusão.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd1292d34abdc745075e030609d3f28a17b2431a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964638"
---
# <a name="synchronizationprogress-resource-type"></a>tipo de recurso synchronizationProgress

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o andamento de um [synchronizationJob](synchronization-synchronizationjob.md) para a conclusão.

## <a name="properties"></a>Propriedades

| Propriedade                              | Tipo      | Descrição    |
|:--------------------------------------|:----------|:---------------|
|completedUnits|Int32|O numerador de uma taxa de progresso; o número de unidades de alterações já processadas.|
|progressObservationDateTime|DateTimeOffset|O tempo de uma observação de progresso como um deslocamento em minutos do UTC.|
|totalUnits|Int32|O denominador de uma taxa de progresso; várias unidades de alterações a serem processadas para realizar a sincronização.|
|unid|String|Uma descrição opcional das unidades.|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationProgress"
}-->

```json
{
  "completedUnits": 1025,
  "progressObservationDateTime": "2017-10-10T17:00:00Z",
  "totalUnits": 3024,
  "units": "pages"
}

```

<!-- uuid: 15571993-7e2f-4842-84d5-01ceb67cdc05
20185-08-14 22:30:00 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
