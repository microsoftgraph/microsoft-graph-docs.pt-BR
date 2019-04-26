---
title: tipo de recurso de ideias
description: Ideias são relações calculadas usando análises e técnicas de aprendizado de máquina. Por exemplo, você pode identificar tendências de documentos do OneDrive com usuários à sua volta.
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: 4e71dbca7bf4ebbe054d0da83436e5dc2129cf19
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551894"
---
# <a name="insights-resource-type"></a>tipo de recurso de ideias

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ideias são relações calculadas usando análises e técnicas de aprendizado de máquina. Por exemplo, você pode identificar tendências de documentos do OneDrive com usuários à sua volta.

Informações são retornadas pelas seguintes APIs:

- [Tendências](insights-trending.md) – retorna a documentos do OneDrive e de sites do SharePoint de tendências de um usuário à sua volta.
- [Usado](insights-used.md) - Retornar documentos visualizados e modificados recentemente por um usuário. Inclui documentos que o usuário usou no OneDrive for Business, SharePoint, aberto como anexos de email e anexos de link de fontes como o Box, DropBox e Google Drive.
- [Compartilhado](insights-shared.md) -retornará documentos compartilhados com um usuário. Documentos podem ser compartilhados como anexos de email ou links do OneDrive para Business enviados por email.

Cada ideia é retornada com um tipo de valor complexo (CVT) `resourceVisualization` e `resourceReference`. O resourceVisualization CVT contém propriedades, como `title` e `previewImageUrl`. A Microsoft usa as propriedades de visualização para renderizar os arquivos em experiências como o Office Delve.

## <a name="relationships"></a>Relações

| Relação      | Tipo          | Descrição  |
| ------------- |---------------| -------------|
| trending      | Coleção [Tendências](insights-trending.md)       | Relação calculada identificando documentos mais populares. Os documentos mais populares podem ser armazenados no OneDrive ou em sites do SharePoint.   |
| used      | Coleção [Usado](insights-used.md)       | Relação calculada para identificar documentos exibidos e modificados por um usuário. Inclui documentos que o usuário usou no OneDrive for Business, SharePoint, aberto como anexos de email e anexos de link de fontes como o Box, DropBox e Google Drive.  |
| shared        | Coleção [compartilhado](insights-shared.md)       | Relação calculada identificando documentos mais populares compartilhados com um usuário. Documentos podem ser compartilhados como anexos de email ou links do OneDrive para Business enviados por email.   |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso
```json
{
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
