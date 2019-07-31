---
title: tipo de recurso onenoteResource
description: 'Uma imagem ou outro recurso de arquivo em uma página do OneNote. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3884be59ed0eedafa9d4a45c851570d08ea70848
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009339"
---
# <a name="onenoteresource-resource-type"></a>tipo de recurso onenoteResource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma imagem ou outro recurso de arquivo em uma página do OneNote. 

Você pode obter os dados binários de um recurso, mas obter uma representação JSON de um objeto Resource ou uma coleção de recursos não é suportada.

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
Obtenha os dados binários de um recurso específico enviando uma solicitação GET para o ponto de `content` extremidade do recurso:

```
GET ../onenote/resources/{id}/content
```

O URI de recurso do arquivo é retornado quando você obtém o conteúdo HTML de uma página usando a seguinte solicitação:

```
GET ../onenote/pages/{id}/content
```

Na página HTML, uma `img` marca inclui pontos de extremidade do recurso de imagem original no `data-fullres-src` atributo e a imagem otimizada no `src` atributo:
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

Uma `object` marca (que representa arquivos como PDF, docx e png) inclui o ponto de extremidade para o recurso de arquivo no `data` atributo:

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| content | EDM. Stream||
| contentUrl | String ||

## <a name="relationships"></a>Relações
Nenhum


## <a name="methods"></a>Métodos
| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter dados binários do recurso](../api/resource-get.md) | Fluxo |Recupere os dados binários de um recurso de arquivo ou imagem.|

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
