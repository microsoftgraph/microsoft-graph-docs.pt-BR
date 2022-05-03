---
title: Tipo de recurso onenoteResource
description: 'Uma imagem ou outro recurso de arquivo em uma OneNote página. '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: notes
author: jewan-microsoft
ms.openlocfilehash: 21d0be436241b518e87b0eb36956886808211a0d
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176712"
---
# <a name="onenoteresource-resource-type"></a>Tipo de recurso onenoteResource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma imagem ou outro recurso de arquivo em uma OneNote página.

Você pode obter os dados binários de um recurso, mas não há suporte para obter uma representação JSON de um objeto de recurso ou uma coleção de recursos.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": "String (Stream)",
  "contentUrl": "String"
}
```

Obtenha os dados binários de um recurso específico enviando uma solicitação GET para o ponto de extremidade do `content` recurso:

```http
GET ../onenote/resources/{id}/content
```

O URI do recurso do arquivo é retornado quando você obtém o conteúdo HTML de uma página usando a seguinte solicitação:

```http
GET ../onenote/pages/{id}/content
```

No HTML da página, uma `img` marca inclui pontos de extremidade para o recurso de imagem original `data-fullres-src` no atributo e a imagem otimizada no `src` atributo:

```html
<img
    src="image-resource-url"
    data-src-type="media-type"
    data-fullres-src="image-resource-url"
    data-fullres-src-type="media-type" ... />
```

Uma `object` marca (que representa arquivos como PDF, DOCX e PNG) inclui o ponto de extremidade para o recurso de arquivo no `data` atributo:

```html
<object
    data="file-resource-url"
    data-attachment="file-name.file-type"
    type="media-type" ... />
```

## <a name="methods"></a>Métodos
| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter dados binários do recurso](../api/resource-get.md) | Stream |Recupere os dados binários de um recurso de arquivo ou imagem.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| content | Edm.Stream||
| contentUrl | Cadeia de Caracteres ||

## <a name="relationships"></a>Relações
Nenhum

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


