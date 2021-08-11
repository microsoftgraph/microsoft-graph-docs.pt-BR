---
author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
description: O recurso itemPreviewInfo contém informações sobre como inserir uma visualização de um driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d6a3eaac24991c4c95da0dd4b4ae2640d6462f95c25b47d0fcbea6ff459962ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130048"
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
| getUrl         | string | URL adequada para a incorporação usando HTTP GET (iframes, etc.)
| postUrl        | string | URL adequada para a incorporação usando HTTP POST (postagem de formulário, JS, etc.)
| postParameters | string | Parâmetros POST a incluir se estiver usando postUrl

GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual de suporte para as opções especificadas.

postParameters é uma cadeia de caracteres formatada como , e se executar um POST para o postUrl o tipo de conteúdo deve ser `application/x-www-form-urlencoded` definido de acordo. Por exemplo:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Os formatos de URLs e parâmetros devem ser considerados opacos.

