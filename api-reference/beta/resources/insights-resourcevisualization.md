---
title: tipo de recurso de resourceVisualization
description: Tipo complexo que contém propriedades de ideias.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 9dc2d50a5bc694204317f8c3332263ce5259e2fc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575101"
---
# <a name="resourcevisualization-resource-type"></a>tipo de recurso de resourceVisualization

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Tipo complexo que contém propriedades de [officeGraphInsights](insights.md).

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],  
  "@odata.type": "microsoft.graph.resourceVisualization"
}-->
```json
{
}
```

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo          | Descrição  |
| -------------         |---------------| -------------|
| title                 | String        | Texto do título do item.               |
| type              | String        | Tipo de mídia do item. Pode ser usado para filtrar para um arquivo específico com base em um tipo específico. Veja abaixo tipos suportados. |
| mediaType             | String        | Tipo de mídia do item. Pode ser usado para filtragem para um tipo específico de arquivo com base em tipos de Mime de mídia IANA suportados. Observe que nem todos os tipos de Mime de mídia são suportados. |
| previewImageUrl       | String        | Uma URL, levando a imagem de visualização para o item. |
| previewText           | String        | Um texto de visualização para o item. |
| containerWebUrl       | String        | Um caminho que leva à pasta na qual o item está armazenado. |
| containerDisplayName  | String        | Uma cadeia de caracteres que descreve onde o item é armazenado. Por exemplo, o nome de um site do SharePoint ou o nome de usuário que identifica o proprietário do OneDrive armazenar o item.  |
| containerType         | String | Pode ser usado para filtrar por tipo de contêiner no qual o arquivo está armazenado. Como o Site ou OneDriveBusiness.       |

## <a name="type-property-values"></a>Valores de tipo de propriedade
-   PowerPoint
-   Word
-   Excel
-   PDF
-   OneNote
-   OneNotePage
-   InfoPath
-   Visio
-   Publisher
-   Project
-   Access
-   Email
-   CSV
-   Arquivo morto
-   XPS
-   Áudio
-   Vídeo
-   Image
-   Web
-   Texto
-   Xml
-   Story
-   ExternalContent
-   Folder
-   Other

Consulta de exemplo:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

## <a name="containertype-property-values"></a>valores de propriedade containerType
Os tipos suportados podem variar, dependendo em contêineres do qual a [percepção](insights.md) retorna os arquivos. Por exemplo, apenas o insight [compartilhados](insights-shared.md) retorna arquivos do 'Recados', 'Caixa' e 'GDrive'.

-   OneDriveBusiness
-   Site
-   Email
-   Pasta de recados
-   Caixa
-   GDrive

Consulta de exemplo:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
