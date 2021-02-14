---
author: daspek
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
description: O recurso contentTypeOrder especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e25025e86c03d7c94ed88a94ad390a56db4a44b0
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238502"
---
# <a name="contenttypeorder-resource-type"></a>Tipo de recurso ContentTypeOrder

Namespace: microsoft.graph

O recurso **contentTypeOrder** especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **contentTypeOrder**.
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo    | Descrição
|:--------------|:--------|:----------------------------------------------------
| **default**   | booliano | Se esse é o Content Type padrão
| **position**  | Int32   | Especifica a posição em que o tipo de conteúdo aparece na seleção da interface do usuário.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->

