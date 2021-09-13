---
author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
ms.localizationpriority: medium
description: O recurso itemPreviewInfo contém informações sobre como inserir uma visualização de um driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e0a56b5129e67af8dc0ac7b360664eb31433d137
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084297"
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
| getUrl         | cadeia de caracteres | URL adequada para a incorporação usando HTTP GET (iframes, etc.)
| postUrl        | cadeia de caracteres | URL adequada para a incorporação usando HTTP POST (postagem de formulário, JS, etc.)
| postParameters | cadeia de caracteres | Parâmetros POST a incluir se estiver usando postUrl

GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual de suporte para as opções especificadas.

postParameters é uma cadeia de caracteres formatada como , e se executar um POST para o postUrl o tipo de conteúdo deve ser `application/x-www-form-urlencoded` definido de acordo. Por exemplo:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Os formatos de URLs e parâmetros devem ser considerados opacos.

