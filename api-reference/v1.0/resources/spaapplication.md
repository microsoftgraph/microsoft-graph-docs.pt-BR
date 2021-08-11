---
title: Tipo de recurso spaApplication
description: Especifica configurações para um aplicativo de página única.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: bc1974925713354484ea3998d394b9a212432caec2b2f56d12ee7072bb825f97
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152002"
---
# <a name="spaapplication-resource-type"></a>Tipo de recurso spaApplication

Namespace: microsoft.graph

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
