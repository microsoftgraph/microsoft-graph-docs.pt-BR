---
author: daspek
description: O recurso contentTypeOrder especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.
ms.date: 09/13/2017
title: ContentTypeOrder
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: bf7fca8ae00a0fd131fa2410a980f73fe4588083
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944903"
---
# <a name="contenttypeorder-resource-type"></a>Tipo de recurso ContentTypeOrder

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

| Propriedade     | Tipo    | Descrição                                                                   |
| :----------- | :------ | :---------------------------------------------------------------------------- |
| **default**  | booliano | Se esse é o Content Type padrão                                      |
| **position** | Int32   | Especifica a posição em que o tipo de conteúdo aparece na seleção da interface do usuário. |

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder",
  "suppressions": []
}
-->
