---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
ms.openlocfilehash: e7df636f9c406a499baa5ef3be1748273920cac4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585234"
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

SegetUrl, postUrl ou ambos podem ser retornados, dependendo do estado atual de suporte para as opções especificadas.

postparameters é uma cadeia de caracteres `application/x-www-form-urlencoded`formatada como e, se estiver executando uma postaGem no postUrl, o tipo de conteúdo deve ser definido de acordo. Por exemplo:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Os formatos das URLs e dos parâmetros devem ser considerados opacos.
