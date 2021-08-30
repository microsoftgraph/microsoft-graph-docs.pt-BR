---
title: tipo de recurso officeGraphInsights
description: Representa o tipo base para itemInsights. officeGraphInsights é para fins de compatibilidade com versões anteriores da API do insights. Use apenas itemInsights ao acessar a API do insights.
author: simonhult
ms.localizationpriority: high
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 308d35e19eaf1ac5454b33b030d2e9c0a7f7a416
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695914"
---
# <a name="officegraphinsights-resource-type"></a>tipo de recurso officeGraphInsights

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use [itemInsights](iteminsights.md) no lugar de **officeGraphInsights** para acessar a API do insights.

**officeGraphInsights** é para fins de compatibilidade com versões anteriores da API do insights. É o tipo de base para [itemInsights](iteminsights.md).

Ideias são relações calculadas usando análises e técnicas de aprendizado de máquina. Por exemplo, você pode identificar documentos do OneDrive for Business que se aproximam dos usuários.

Informações são retornadas pelas seguintes APIs:

- [Tendências](insights-trending.md) - retorna documentos do OneDrive for Business e de sites do SharePoint tendendo para um usuário.
- [Usado](insights-used.md) - retorna documentos visualizados ou modificados por um usuário. Inclui documentos que o usuário usou no OneDrive for Business e no SharePoint.
- [Compartilhado](insights-shared.md) - retornará documentos compartilhados com um usuário. Os documentos podem ser compartilhados como URLs, anexos de arquivo, anexos de referência aos arquivos do OneDrive for Business e SharePoint encontrados nas mensagens e reuniões do Outlook.

Cada opinião é retornada com um **resourceVisualization** e Tipo de valor complexo (CVT) **resourceReference**. O CVT **resourceVisualization** contém propriedades como **título** e **previewImageUrl**. A Microsoft usa as propriedades de visualização para renderizar os arquivos em experiências como o Office Delve.

## <a name="relationships"></a>Relações

| Relação      | Tipo          | Descrição  |
| ------------- |---------------| -------------|
| tendências      | coleção [tendências](insights-trending.md)        | Acessar essa propriedade a partir do tipo derivado [itemInsights](iteminsights.md).|
| usado      | coleção [usedInsight](insights-used.md)        | Acessar essa propriedade a partir do tipo derivado [itemInsights](iteminsights.md).|
| compartilhado        | coleção [sharedInsight](insights-shared.md)        | Acessar essa propriedade a partir do tipo derivado [itemInsights](iteminsights.md).|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso
<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "baseType":"microsoft.graph.entity",
  "optionalProperties": [
    "trending",
    "used",
    "shared"
  ],
  "@odata.type": "microsoft.graph.officeGraphInsights"
}-->

```json
{
  "id": "string",
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```



