---
title: Tipo de recurso safeguardProfile
description: Descreve os problemas contra os quais o serviço protege dispositivos.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 8c528111af41ee3340a58402f66d2e4ac5410aca
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890119"
---
# <a name="safeguardprofile-resource-type"></a>Tipo de recurso safeguardProfile

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve os problemas contra os quais o serviço protege dispositivos.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Ferramentas para desenvolvedores|microsoft.graph.windowsUpdates.safeguardCategory|Especifica a categoria de proteções. Os valores possíveis são: `likelyIssues` , `unknownFutureValue` .|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.safeguardProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.safeguardProfile",
  "category": "String"
}
```

