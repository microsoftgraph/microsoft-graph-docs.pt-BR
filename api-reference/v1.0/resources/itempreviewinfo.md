---
author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
description: O recurso itemPreviewInfo contém informações sobre como inserir uma visualização de um driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc7ece7ed529a714b2e1262c4e39444639caced1
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240567"
---
# <a name="itempreviewinfo-resource-type"></a>Tipo de recurso itemPreviewInfo

Namespace: microsoft.graph

O **recurso itemPreviewInfo** contém informações sobre como inserir uma visualização de [um driveItem](driveitem.md).

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
| getUrl         | string | URL adequada para incorporação usando HTTP GET (iframes, etc.)
| postUrl        | string | URL adequada para incorporação usando HTTP POST (postagem de formulário, JS etc.)
| postParameters | string | Parâmetros POST a incluir se estiver usando postUrl

GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual do suporte para as opções especificadas.

postParameters é uma cadeia de caracteres formatada como , e se executar um POST para postUrl, o tipo de conteúdo deve `application/x-www-form-urlencoded` ser definido de acordo. Por exemplo:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Os formatos de URLs e parâmetros devem ser considerados opacos.

