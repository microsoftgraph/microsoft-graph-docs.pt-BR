---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
description: O recurso contentTypeOrder especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5c77f2dd3763199fea8f0a1377a1b46f8aa4881d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032834"
---
# <a name="contenttypeorder-resource-type"></a>Tipo de recurso ContentTypeOrder

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
