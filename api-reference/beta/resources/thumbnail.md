---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Miniatura
localization_priority: Normal
ms.openlocfilehash: 22602d534c3fd1f308a5e2bb67992bd76086c4fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863221"
---
# <a name="thumbnail-resource-type"></a>Tipo de recurso thumbnail

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O tipo de recurso **thumbnail** representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON de um recurso **thumbnail**.

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width", "sourceItemId"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,

  /* relationships */
  "content": "stream"
}
```

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   | Descrição                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| height       | Int32  | A altura da miniatura em pixels.                                                                                     |
| sourceItemId | String | O identificador exclusivo do item que disponibilizou a miniatura. Só estará disponível quando for solicitada uma miniatura da pasta. |
| url          | Cadeia de caracteres | A URL usada para buscar o conteúdo da miniatura.                                                                                |
| width        | Int32  | A largura da miniatura em pixels.                                                                                      |

## <a name="relationships"></a>Relações

| Nome    | Tipo   | Descrição                           |
| :------ | :----- | :------------------------------------ |
| content | Fluxo | O fluxo de conteúdo da miniatura. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
