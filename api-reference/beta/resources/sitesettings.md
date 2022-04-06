---
title: Tipo de recurso siteSettings
description: Representa as configurações de um site.
author: k-tsoi
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 210b0f36d0dbbfc9402eec6d0a58a62ae646605a
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589644"
---
# <a name="sitesettings-resource-type"></a>Tipo de recurso siteSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de um [site].

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|languageTag|Cadeia de caracteres|A marca de idioma do idioma usado neste site.|
|timeZone|Cadeia de caracteres|Indica o deslocamento de tempo para o fuso horário do site a partir de UTC (Tempo Universal Coordenado).|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteSettings"
}
-->
``` json
{
    "languageTag": "String",
    "timeZone": "String"
}
```

[site]: site.md
