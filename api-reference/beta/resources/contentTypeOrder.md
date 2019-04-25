---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
ms.openlocfilehash: 9b92a8234c493ae9b0f396db7010e7bf717d5959
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535421"
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
