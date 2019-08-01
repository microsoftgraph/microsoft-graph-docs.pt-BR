---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
description: O recurso itemPreviewInfo contém informações sobre como inserir uma visualização de um driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 71d660a71bce09f198a0feb9c3acbb9a69a23a5f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036558"
---
# <a name="itempreviewinfo-resource-type"></a>tipo de recurso itemPreviewInfo

O recurso **itemPreviewInfo** contém informações sobre como inserir uma visualização de um [driveItem](driveitem.md).

## <a name="json-representation"></a>Representação JSON

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a>Propriedades

| Nome           | Tipo   | Descrição
|:---------------|:-------|:---------------------------------------------------
| getUrl         | string | URL adequada para incorporação usando HTTP GET (IFrames, etc.)
| postUrl        | string | URL adequada para incorporação usando HTTP POST (Form Post, JS, etc.)
| postparameters | string | LANÇAR parâmetros para incluir se estiver usando postUrl

Segeturl, postUrl ou ambos podem ser retornados, dependendo do estado atual de suporte para as opções especificadas.

postparameters é uma cadeia de caracteres `application/x-www-form-urlencoded`formatada como e, se estiver executando uma postagem no postUrl, o tipo de conteúdo deve ser definido de acordo. Por exemplo:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Os formatos das URLs e dos parâmetros devem ser considerados opacos.
