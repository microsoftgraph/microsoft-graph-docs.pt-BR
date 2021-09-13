---
title: Tipo de recurso do OneNoteResource
description: 'Uma imagem ou outro recurso de arquivo em uma OneNote página. '
ms.localizationpriority: medium
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f0f290329135f828ac36d5e5d805c515f2d9a207
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59055847"
---
# <a name="onenoteresource-resource-type"></a>Tipo de recurso do OneNoteResource

Namespace: microsoft.graph

Uma imagem ou outro recurso de arquivo em uma OneNote página.

Você pode obter os dados binários de um recurso, mas não há suporte para obter uma representação JSON de um objeto de recurso ou uma coleção de recursos.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "contentUrl": "string (url)"
}
```

Obter os dados binários de um recurso específico enviando uma solicitação GET para o ponto de extremidade do `content` recurso:

```
GET ../onenote/resources/{id}/content
```

O URI de recurso do arquivo é retornado quando você obter o conteúdo HTML de uma página usando a seguinte solicitação:

```
GET ../onenote/pages/{id}/content
```

Na página HTML, uma marca inclui pontos de extremidade para o recurso de imagem original no atributo e a imagem `img` `data-fullres-src` otimizada no `src` atributo:
```
<img
    src="image-resource-url"
    data-src-type="media-type"
    data-fullres-src="image-resource-url"
    data-fullres-src-type="media-type" ... />
```

Uma marca (que representa arquivos como PDF, DOCX e PNG) inclui o ponto de extremidade do recurso `object` de arquivo no `data` atributo:

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type"
    type="media-type" ... />
```

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo            | Descrição
|:---------------------|:----------------|:---------------------------------
| conteúdo              | Fluxo          | O fluxo de conteúdo
| contentUrl           | Cadeia de caracteres (url)    | A URL para baixar o conteúdo

## <a name="relationships"></a>Relações
Nenhum


## <a name="methods"></a>Métodos
| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter dados binários de recursos](../api/resource-get.md) | Stream |Recupere os dados binários de um recurso de arquivo ou imagem.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

