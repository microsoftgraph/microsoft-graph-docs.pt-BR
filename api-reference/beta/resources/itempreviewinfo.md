---
author: kevinlam
description: O recurso ItemPreviewInfo contém informações sobre como inserir uma visualização de um DriveItem.
ms.date: 3/16/2018
title: ItemPreviewInfo - OneDrive API
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9e4f3b390fe21284791b6c40d19d4de71ec3548b
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723343"
---
# <a name="itempreviewinfo-resource-type"></a>Tipo de recurso ItemPreviewInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **recurso ItemPreviewInfo** contém informações sobre como inserir uma visualização de [um DriveItem](driveitem.md).

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
| getUrl         | string | URL adequada para a incorporação usando HTTP GET (iframes, etc.)        |
| postUrl        | string | URL adequada para a incorporação usando HTTP POST (postagem de formulário, JS, etc.) |
| postParameters | string | Parâmetros POST a incluir se estiver usando postUrl                      |

GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual de suporte para as opções especificadas.

postParameters é uma cadeia de caracteres formatada `application/x-www-form-urlencoded`como , e se executar um POST para o postUrl o tipo de conteúdo deve ser definido de acordo. Por exemplo:

```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Os formatos de URLs e parâmetros devem ser considerados opacos.
