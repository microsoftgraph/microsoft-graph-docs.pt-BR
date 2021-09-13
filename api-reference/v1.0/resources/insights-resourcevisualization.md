---
title: tipo de recurso resourceVisualization
description: Tipo complexo que contém propriedades de Insights.
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: e35848be021df48cb2ff10533bf597e91e58db24
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109154"
---
# <a name="resourcevisualization-resource-type"></a>tipo de recurso resourceVisualization

Namespace: microsoft.graph

Tipo complexo que contém propriedades do [officeGraphInsights](officegraphinsights.md).

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
  "title": "string",
  "type"  : "string",
  "mediaType": "string",
  "previewImageUrl": "string",
  "previewText": "string",
  "containerWebUrl": "string",
  "containerDisplayName": "string",
  "containerType": "string"
}
```

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo          | Descrição  |
| -------------         |---------------| -------------|
| title                 | Cadeia de caracteres        | O texto do título do item.               |
| tipo              | String        | O tipo de mídia do item. Pode ser usado para filtrar um arquivo específico com base em um tipo específico. Consulte abaixo os tipos com suporte. |
| mediaType             | Cadeia de caracteres        | O tipo de mídia do item. Pode ser usado para filtragem de um tipo específico de arquivo com base nos Tipos de Mime de Mídia IANA suportados. Observe que nem todos os Tipos de Mime de Mídia são suportados. |
| previewImageUrl       | Cadeia de caracteres        | Uma URL que conduz à imagem de visualização do item. |
| previewText           | Cadeia de caracteres        | Um texto de visualização para o item. |
| containerWebUrl       | Cadeia de caracteres        | Um caminho que leva à pasta na qual o item é armazenado. |
| containerDisplayName  | String        | Uma cadeia de caracteres que descreve onde o item está armazenado. Por exemplo, o nome de um site SharePoint ou o nome do usuário que identifica o proprietário do OneDrive o item.  |
| containerType         | Cadeia de caracteres | Pode ser usado para filtragem pelo tipo de contêiner no qual o arquivo está armazenado. Como Site ou OneDriveBusiness.       |

## <a name="type-property-values"></a>Digite valores de propriedade
-   PowerPoint
-   Word
-   Excel
-   Pdf
-   OneNote
-   OneNotePage
-   InfoPath
-   Visio
-   Publisher
-   Project
-   Access
-   Email
-   Csv
-   Arquivar
-   Xps
-   Áudio
-   Vídeo
-   Imagem
-   Web
-   Texto
-   Xml
-   História
-   ExternalContent
-   Folder
- Spsite
-   Outros

Consulta de exemplo: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

Observações: `spsite` talvez seja necessário classificar por `lastUsed/lastAccessedDateTime` desc para recuperar resultados válidos

## <a name="containertype-property-values"></a>valores da propriedade containerType
Os tipos com suporte podem diferir com base em contêineres dos quais [o officeGraphInsights](officegraphinsights.md) retorna arquivos. Por exemplo, somente o [insight sharedInsight](insights-shared.md) retorna arquivos de 'DropBox', 'Box' e 'GDrive'.

-   OneDriveBusiness
-   Site
-   Email
-   DropBox
-   Caixa
-   GDrive

Consulta de exemplo: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

