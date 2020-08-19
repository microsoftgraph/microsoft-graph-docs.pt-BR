---
title: tipo de recurso yomiPersonName
description: tipo de recurso yomiPersonName
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6e112d97f67b260c19de9fe0ab104e9dc1ed1d74
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810332"
---
# <a name="yomipersonname-resource-type"></a>tipo de recurso yomiPersonName

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece um mecanismo para que um usuário armazene informações sobre como pronunciar um nome para alto-falantes não nativos do idioma no qual o recurso [PersonName](personname.md) é representado.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição                                             |
|:-------------|:------------|:--------------------------------------------------------|
|displayName   |String       | Composto de guias de pronúncia de nome e de sobrenome.  |
|primeiro         |String       | Guia de pronúncia para o primeiro nome do usuário.     |
|durar          |String       | Guia de pronúncia para o sobrenome do usuário.      |
|Virgem        |String       | Guia de pronúncia para o nome de solteira do usuário.    |
|middleware        |String       | Guia de pronúncia para o nome do meio do usuário.    |

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
