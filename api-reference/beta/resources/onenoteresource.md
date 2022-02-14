---
title: Tipo de recurso do onenoteResource
description: 'Uma imagem ou outro recurso de arquivo em uma OneNote página. '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: f7a479ec529cae209fef085da2978c3e412a844f
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804917"
---
# <a name="onenoteresource-resource-type"></a>Tipo de recurso do onenoteResource

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

Obter os dados binários de um recurso específico enviando uma solicitação GET para o ponto de extremidade do `content` recurso:

```http
GET ../onenote/resources/{id}/content
```

O URI de recurso do arquivo é retornado quando você obter o conteúdo HTML de uma página usando a seguinte solicitação:

```http
GET ../onenote/pages/{id}/content
```

Na página HTML, uma `img` marca inclui pontos de extremidade para o recurso de imagem original `data-fullres-src` no atributo e a imagem otimizada no `src` atributo:

```html
<img
    src="image-resource-url"
    data-src-type="media-type"
    data-fullres-src="image-resource-url"
    data-fullres-src-type="media-type" ... />
```

Uma `object` marca (que representa arquivos como PDF, DOCX e PNG) inclui o ponto de extremidade do recurso de arquivo no `data` atributo:

```html
<object
    data="file-resource-url"
    data-attachment="file-name.file-type"
    type="media-type" ... />
```

## <a name="methods"></a>Métodos
| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter dados binários de recursos](../api/resource-get.md) | Stream |Recupere os dados binários de um recurso de arquivo ou imagem.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| content | Edm.Stream||
| contentUrl | Cadeia de caracteres ||

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


