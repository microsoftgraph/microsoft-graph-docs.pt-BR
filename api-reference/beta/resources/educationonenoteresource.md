---
title: tipo de recurso de educationOneNoteResource
description: 'Uma subclasse de educationResource. Isso representa o local da página do OneNote.  '
author: mmast-msft
ms.openlocfilehash: dc6fc6a71da12a27cb589e072371814e4bc33cc1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359861"
---
# <a name="educationonenoteresource-resource-type"></a>tipo de recurso de educationOneNoteResource

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Uma subclasse de [educationResource](educationresource.md). Isso representa o local da página do OneNote.  

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|pageUrl|String|A URL de gráfico da Microsoft a página do OneNote.|
|sectionName|String|Nome da seção que devem ser copiadas para distribuições ou que foram copiadas para.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOneNoteResource"
}-->

```json
{
  "pageUrl": "String",
  "sectionName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOneNoteResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
