---
title: tipo de recurso de synchronizationProgress
description: Representa o progresso de um synchronizationJob rumo à conclusão.
ms.openlocfilehash: 412b7754dac97a36efe082026ab360569c0fe789
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040761"
---
# <a name="synchronizationprogress-resource-type"></a>tipo de recurso de synchronizationProgress

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa o progresso de um [synchronizationJob](synchronization-synchronizationjob.md) rumo à conclusão.

## <a name="properties"></a>Propriedades

| Propriedade                              | Tipo      | Descrição    |
|:--------------------------------------|:----------|:---------------|
|completedUnits|Int32|O numerador de uma proporção de progresso; o número de unidades de alterações já processadas.|
|progressObservationDateTime|DateTimeOffset|A hora de uma observação de progresso como um deslocamento em minutos de UTC.|
|totalUnits|Int32|Denominador de uma proporção de progresso; um número de unidades de alterações a serem processados para realizar a sincronização.|
|unidades|String|Uma descrição opcional das unidades.|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
