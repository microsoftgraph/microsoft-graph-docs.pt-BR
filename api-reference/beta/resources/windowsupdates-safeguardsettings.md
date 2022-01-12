---
title: Tipo de recurso safeguardSettings
description: Gerencia as proteções que o serviço se aplica a dispositivos em uma implantação.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: d3c276a07483b42e513266077ef1ada3bc516d47
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792117"
---
# <a name="safeguardsettings-resource-type"></a>Tipo de recurso safeguardSettings

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Gerencia as proteções que o serviço se aplica a dispositivos em uma implantação.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|disabledSafeguardProfiles|[coleção microsoft.graph.windowsUpdates.safeguardProfile](../resources/windowsupdates-safeguardprofile.md)|Lista de proteções a ser ignorada por dispositivo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.safeguardSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.safeguardSettings",
  "disabledSafeguardProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.safeguardProfile"
    }
  ]
}
```

