---
title: tipo de recurso synchronizationProgress
description: Representa o andamento de um synchronizationJob para a conclusão.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c9a9ea8b5bd9d2a0fbfbcb1a64381b46e2f96283
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217399"
---
# <a name="synchronizationprogress-resource-type"></a>tipo de recurso synchronizationProgress

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o andamento de um [synchronizationJob](synchronization-synchronizationjob.md) para a conclusão.

## <a name="properties"></a>Propriedades

| Propriedade                              | Tipo      | Descrição    |
|:--------------------------------------|:----------|:---------------|
|completedUnits|Int32|O numerador de uma taxa de progresso; o número de unidades de alterações já processadas.|
|progressObservationDateTime|DateTimeOffset|O tempo de uma observação de progresso como um deslocamento em minutos do UTC.|
|totalUnits|Int32|O denominador de uma taxa de progresso; várias unidades de alterações a serem processadas para realizar a sincronização.|
|unid|Cadeia de Caracteres|Uma descrição opcional das unidades.|

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
