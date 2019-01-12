---
title: tipo de recurso de resourceVisualization
description: Tipo complexo que contém propriedades de ideias.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: f8426d13968e5bea929c8e26f71346fa554a5242
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990653"
---
# <a name="resourcevisualization-resource-type"></a>tipo de recurso de resourceVisualization

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Tipo complexo que contém propriedades de [ideias](insights.md).

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

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
-   Outros

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
