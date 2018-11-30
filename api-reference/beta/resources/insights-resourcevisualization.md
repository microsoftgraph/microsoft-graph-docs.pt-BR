---
title: tipo de recurso de resourceVisualization
description: Tipo complexo que contém propriedades de ideias.
ms.openlocfilehash: 3ed61a8547e072938fc073d90f2592baf4c08fba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038203"
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
-   Projeto
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
-   Pasta
-   Outro

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