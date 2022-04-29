---
title: Tipo de recurso cloudPcLaunchInfo
description: Contém as informações para conectar um COMPUTADOR na nuvem.
author: andrewku0409
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 546bd11263c3bdb9ac4421eb8f9eb3580e6af255
ms.sourcegitcommit: 4ef29d4a2cfa1ccc4a3da649e683377b17b90108
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65126330"
---
# <a name="cloudpclaunchinfo-resource-type"></a>Tipo de recurso cloudPcLaunchInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém as informações para conectar um [cloudPC](../resources/cloudpc.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|cloudPcId|Cadeia de caracteres|O identificador exclusivo do PC na nuvem.|
|cloudPcLaunchUrl|Cadeia de caracteres|A URL de conexão do PC na nuvem.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcLaunchInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcLaunchInfo",
  "cloudPcId": "String",
  "cloudPcLaunchUrl": "String"
}
```

