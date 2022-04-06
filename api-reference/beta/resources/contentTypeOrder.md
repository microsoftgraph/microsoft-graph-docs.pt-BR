---
author: daspek
description: O recurso contentTypeOrder especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.
ms.date: 09/13/2017
title: ContentTypeOrder
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 615655ecf400c814e08ef75dfbabd9a5f97cf167
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63720819"
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
