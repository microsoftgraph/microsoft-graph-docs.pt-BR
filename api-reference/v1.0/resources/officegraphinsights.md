---
title: tipo de recurso officeGraphInsights
description: Ideias são relações calculadas usando análises e técnicas de aprendizado de máquina. Por exemplo, você pode identificar documentos do OneDrive for Business que se aproximam dos usuários.
author: simonhult
ms.localizationpriority: high
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: ba7d88446850ddeddbd1f0b46995f4c363aa1e6d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084206"
---
# <a name="officegraphinsights-resource-type"></a>tipo de recurso officeGraphInsights

Namespace: microsoft.graph

Ideias são relações calculadas usando análises e técnicas de aprendizado de máquina. Por exemplo, você pode identificar documentos do OneDrive for Business que se aproximam dos usuários.

Informações são retornadas pelas seguintes APIs:

- [Tendências](insights-trending.md) - retorna documentos do OneDrive for Business e de sites do SharePoint tendendo para um usuário.
- [Usado](insights-used.md) - retorna documentos visualizados ou modificados por um usuário. Inclui documentos que o usuário usou no OneDrive for Business e no SharePoint.
- [Compartilhado](insights-shared.md) - retornará documentos compartilhados com um usuário. Os documentos podem ser compartilhados como URLs, anexos de arquivo, anexos de referência aos arquivos do OneDrive for Business e SharePoint encontrados nas mensagens e reuniões do Outlook.

Cada opinião é retornada com um **resourceVisualization** e Tipo de valor complexo (CVT) **resourceReference**. O CVT **resourceVisualization** contém propriedades como **título** e **previewImageUrl**. A Microsoft usa as propriedades de visualização para renderizar os arquivos em experiências como o Office Delve.

## <a name="relationships"></a>Relações

| Relação      | Tipo          | Descrição  |
| ------------- |---------------| -------------|
| tendências      | coleção [tendências](insights-trending.md)        | Relacionamento calculado que identifica documentos de tendências em torno de um usuário. Os documentos de tendência são calculados com base na atividade da rede de pessoas mais próximas do usuário e incluem arquivos armazenados no OneDrive for Business e no SharePoint. As informações de tendências ajudam o usuário a descobrir o conteúdo potencialmente útil que ele tem acesso, mas nunca viu antes.|
| usado      | coleção [usedInsight](insights-used.md)        | Relacionamento calculado que identifica os documentos mais recentes exibidos ou modificados por um usuário, incluindo documentos do OneDrive for Business e do SharePoint, classificados por tempo de uso recente.|
| compartilhado        | coleção [sharedInsight](insights-shared.md)        | Relação calculada identificando documentos compartilhados com ou pelo usuário. Isso inclui URLs, anexos de arquivo e anexos de referência para arquivos do OneDrive for Business e do Microsoft Office SharePoint Online encontrados em mensagens e reuniões do Outlook. Isso também inclui URLs e anexos de referência para conversas do Teams. Ordenado por tempo para retorno do compartilhamento.|

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

