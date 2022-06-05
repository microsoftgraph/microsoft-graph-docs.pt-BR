---
author: kevinlam
title: Tipo de recurso itemPreviewInfo
ms.localizationpriority: medium
description: Contém informações sobre como inserir uma visualização de um driveItem.
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: d89f7ae60df58cb34891879fbc85c4e33cc9f8d7
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899579"
---
# <a name="itempreviewinfo-resource-type"></a>Tipo de recurso itemPreviewInfo

Namespace: microsoft.graph

Contém informações sobre como inserir uma visualização de [um driveItem](driveitem.md).

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
| Geturl         | string | URL adequada para inserção usando HTTP GET (iframes etc.)
| postUrl        | string | URL adequada para inserção usando HTTP POST (postagem de formulário, JS etc.)
| postParameters | string | Parâmetros POST a serem incluídos se estiver usando postUrl

GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual de suporte para as opções especificadas.

postParameters é uma cadeia `application/x-www-form-urlencoded`de caracteres formatada como e, se estiver executando um POST para postUrl, o tipo de conteúdo deverá ser definido adequadamente. Por exemplo:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Os formatos de URLs e parâmetros devem ser considerados opacas.

