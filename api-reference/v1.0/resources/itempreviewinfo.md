---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
ms.openlocfilehash: 8b8f7a962e237cc20a42503efd31f083996ad715
ms.sourcegitcommit: ebac77d2ca32438e552831de0258fe5e86fa225a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2018
ms.locfileid: "26605864"
---
# <a name="itempreviewinfo-resource-type"></a>tipo de recurso de itemPreviewInfo

O recurso de **itemPreviewInfo** contém informações sobre como inserir uma visualização de um [driveItem](driveitem.md).

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
| postUrl        | string | URL adequada para incorporação usando POST HTTP (formulário post, JS, etc.)
| postParameters | string | Parâmetros de POSTAGEM para incluir se usando postUrl

GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual do suporte para as opções especificadas.

postParameters é uma cadeia de caracteres formatada como `application/x-www-form-urlencoded`, e se realizar uma POSTAGEM para o postUrl o tipo de conteúdo deve ser definida adequadamente. Por exemplo:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Os formatos das URLs e dos parâmetros devem ser considerados opacos.
