---
author: kevinlam
description: O recurso ItemPreviewInfo contém informações sobre como inserir uma visualização de um DriveItem.
ms.date: 3/16/2018
title: ItemPreviewInfo – API de OneDrive
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 49c792845205b8b42b70961185da4ca46bee2fb7
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176972"
---
# <a name="itempreviewinfo-resource-type"></a>Tipo de recurso ItemPreviewInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **recurso ItemPreviewInfo** contém informações sobre como inserir uma visualização de um [DriveItem](driveitem.md).

## <a name="json-representation"></a>Representação JSON

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo   | Descrição                                                      |
| :------------- | :----- | :--------------------------------------------------------------- |
| Geturl         | cadeia de caracteres | URL adequada para inserção usando HTTP GET (iframes etc.)        |
| postUrl        | cadeia de caracteres | URL adequada para inserção usando HTTP POST (postagem de formulário, JS etc.) |
| postParameters | cadeia de caracteres | Parâmetros POST a serem incluídos se estiver usando postUrl                      |

GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual de suporte para as opções especificadas.

postParameters é uma cadeia `application/x-www-form-urlencoded`de caracteres formatada como e, se estiver executando um POST para postUrl, o tipo de conteúdo deverá ser definido adequadamente. Por exemplo:

```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Os formatos de URLs e parâmetros devem ser considerados opacas.
