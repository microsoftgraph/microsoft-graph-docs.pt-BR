---
title: Tipo de recurso oneNoteResource
description: 'Uma imagem ou outro recurso de arquivo em uma OneNote página. '
ms.localizationpriority: medium
author: jewan-microsoft
ms.prod: notes
doc_type: resourcePageType
ms.openlocfilehash: e304bdcee171350ade75b6253d12e3abfac77856
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034884"
---
# <a name="onenoteresource-resource-type"></a>Tipo de recurso oneNoteResource

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

Obtenha os dados binários de um recurso específico enviando uma solicitação GET para o ponto de extremidade do `content` recurso:

```
GET ../onenote/resources/{id}/content
```

O URI do recurso do arquivo é retornado quando você obtém o conteúdo HTML de uma página usando a seguinte solicitação:

```
GET ../onenote/pages/{id}/content
```

No HTML da página, uma `img` marca inclui pontos de extremidade para o recurso de imagem original `data-fullres-src` no atributo e a imagem otimizada no `src` atributo:
```
<img
    src="image-resource-url"
    data-src-type="media-type"
    data-fullres-src="image-resource-url"
    data-fullres-src-type="media-type" ... />
```

Uma `object` marca (que representa arquivos como PDF, DOCX e PNG) inclui o ponto de extremidade para o recurso de arquivo no `data` atributo:

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
|[Obter dados binários do recurso](../api/resource-get.md) | Fluxo |Recupere os dados binários de um recurso de arquivo ou imagem.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

