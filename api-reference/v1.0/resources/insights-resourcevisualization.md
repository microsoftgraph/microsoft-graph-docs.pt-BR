---
title: tipo de recurso resourceVisualization
description: Tipo complexo contendo propriedades de insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 2480f55cf0e7ea12d9bfaf31941a943095f62c31
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898034"
---
# <a name="resourcevisualization-resource-type"></a>tipo de recurso resourceVisualization

Namespace: microsoft.graph

Tipo complexo contendo as propriedades de [officeGraphInsights](officegraphinsights.md).

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
| title                 | String        | O texto do título do item.               |
| tipo              | Cadeia de caracteres        | O tipo de mídia do item. Pode ser usado para filtrar um arquivo específico com base em um tipo específico. Veja abaixo os tipos suportados. |
| Mídia             | String        | O tipo de mídia do item. Pode ser usado para filtragem de um tipo específico de arquivo baseado em tipos MIME de mídias da IANA compatíveis. Observe que nem todos os tipos de MIME de mídia têm suporte. |
| previewImageUrl       | String        | Uma URL que leva à imagem de visualização do item. |
| previewText           | String        | Um texto de visualização para o item. |
| containerWebUrl       | String        | Um caminho que conduz à pasta na qual o item está armazenado. |
| containerDisplayName  | String        | Uma cadeia de caracteres que descreve onde o item é armazenado. Por exemplo, o nome de um site do SharePoint ou o nome de usuário que identifica o proprietário do OneDrive que armazena o item.  |
| containerType         | String | Pode ser usado para filtragem pelo tipo de contêiner no qual o arquivo está armazenado. Como site ou OneDriveBusiness.       |

## <a name="type-property-values"></a>Valores de propriedade Type
-   PowerPoint
-   Word
-   Excel
-   Documento
-   OneNote
-   OneNotePage
-   InfoPath
-   Visio
-   Publisher
-   Project
-   Access
-   Correio
-   Limit
-   Arquivar
-   XPS
-   Áudio
-   Vídeo
-   Image
-   Web
-   Texto
-   Xml
-   História
-   ExternalContent
-   Folder
- SPSite
-   Outros

Consulta de exemplo:`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

Observações: `spsite` talvez seja necessário classificar por `lastUsed/lastAccessedDateTime` desc para recuperar resultados válidos

## <a name="containertype-property-values"></a>valores da Propriedade ContainerType
Os tipos com suporte podem diferir com base nos contêineres dos quais o [officeGraphInsights](officegraphinsights.md) retorna arquivos. Por exemplo, somente a percepção [sharedInsight](insights-shared.md) retorna arquivos de "Dropbox", "box" e "GDrive".

-   OneDriveBusiness
-   Site
-   Correio
-   DropBox
-   Caixa
-   GDrive

Consulta de exemplo:`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`
