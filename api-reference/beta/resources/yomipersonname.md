---
title: tipo de recurso yomiPersonName
description: tipo de recurso yomiPersonName
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 926479832db04e427e7ca1d73744008db7dc6aaa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079624"
---
# <a name="yomipersonname-resource-type"></a>tipo de recurso yomiPersonName

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece um mecanismo para que um usuário armazene informações sobre como pronunciar um nome para alto-falantes não nativos do idioma no qual o recurso [PersonName](personname.md) é representado.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição                                             |
|:-------------|:------------|:--------------------------------------------------------|
|displayName   |Cadeia de caracteres       | Composto de guias de pronúncia de nome e de sobrenome.  |
|primeiro         |Cadeia de caracteres       | Guia de pronúncia para o primeiro nome do usuário.     |
|durar          |Cadeia de caracteres       | Guia de pronúncia para o sobrenome do usuário.      |
|Virgem        |Cadeia de caracteres       | Guia de pronúncia para o nome de solteira do usuário.    |
|middleware        |Cadeia de caracteres       | Guia de pronúncia para o nome do meio do usuário.    |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yomiPersonName"
}
-->

``` json

{
  "displayName": "String",
  "first": "String",
  "maiden": "String",
  "middle": "String",
  "last": "String"
}
```


