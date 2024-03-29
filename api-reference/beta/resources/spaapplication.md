---
title: Tipo de recurso spaApplication
description: Especifica configurações para um aplicativo de página única.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 82848c5ea8427111b2d8b02c1886f3990faba79e
ms.sourcegitcommit: be09568fa07ab793cd1db500f537ca94ca9e5b4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836939"
---
# <a name="spaapplication-resource-type"></a>Tipo de recurso spaApplication

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica configurações para um aplicativo de página única.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| redirectUris | Coleção de cadeias de caracteres | Especifica as URLs para as quais os tokens de usuário são enviados para entrar ou as URIs de redirecionamento para as quais os códigos de autorização do OAuth 2.0 e tokens de acesso são enviados. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.spaApplication"
}-->

```json
{
  "redirectUris": ["String"]
}
```
