---
title: Tipo de recurso safeguardProfile
description: Descreve os problemas contra os quais o serviço protege dispositivos.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 95ad3d053afa1fb27190407d359055c47afd4135
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861112"
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

