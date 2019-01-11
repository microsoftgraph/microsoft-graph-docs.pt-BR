---
title: Tipo de recurso de OneNoteResource
description: 'Uma imagem ou outro recurso de arquivo em uma página do OneNote. '
localization_priority: Normal
ms.openlocfilehash: ed2fb0dd4b6e68c24da1f2441a157f734a5025f6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855101"
---
# <a name="onenoteresource-resource-type"></a>Tipo de recurso de OneNoteResource

Uma imagem ou outro recurso de arquivo em uma página do OneNote. 

É possível obter os dados binários de um recurso, mas não há suporte para obter uma representação JSON de um objeto de recurso ou uma coleção de recursos.

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

Obtenha os dados binários de um recurso específico enviando uma solicitação GET para o ponto de extremidade `content` do recurso:

```
GET ../onenote/resources/{id}/content
```

O URI de recurso do arquivo é retornado quando você recebe um conteúdo HTML da página usando a seguinte solicitação:

```
GET ../onenote/pages/{id}/content
```

Na página HTML, uma marca `img` inclui os pontos de extremidade do recurso de imagem original no atributo `data-fullres-src` e a imagem otimizada no atributo `src`:
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

Uma marca `object` (que representa arquivos como PDF, DOCX e PNG) inclui o ponto de extremidade para o recurso do arquivo no atributo `data`:

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo            | Descrição
|:---------------------|:----------------|:---------------------------------
| content              | Fluxo          | O fluxo de conteúdo
| contentUrl           | Cadeia de caracteres (url)    | A URL para baixar o conteúdo

## <a name="relationships"></a>Relações
Nenhum


## <a name="methods"></a>Métodos
| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get resource binary data](../api/resource-get.md) | Fluxo |Recupere os dados binários de um recurso de arquivo ou imagem.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
