---
author: daspek
ms.date: 09/13/2017
title: ContentTypeOrder
ms.localizationpriority: medium
description: O recurso contentTypeOrder especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: d7a1ef454fc43dbde05d974ae8b7d355a1e33d00
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971543"
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

