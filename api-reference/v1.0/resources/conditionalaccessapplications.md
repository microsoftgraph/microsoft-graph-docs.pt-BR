---
title: Tipo de recurso conditionalAccessApplications
description: Representa aplicativos e ações de usuário incluídas e excluídas do escopo da política.
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c051ee2c00a2a62319c17a6859c57a64f8438d4f
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66667793"
---
# <a name="conditionalaccessapplications-resource-type"></a>Tipo de recurso conditionalAccessApplications

Namespace: microsoft.graph

Representa os aplicativos e as ações do usuário incluídas e excluídas da política de acesso condicional.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| includeApplications | String collection | Pode ser um dos seguintes: <li> A lista de IDs de cliente (**appId**) à qual a política se aplica, a menos que seja explicitamente excluída (em **excludeApplications**) <li> `All` <li> `Office365`- Para obter a lista de aplicativos incluídos`Office365`, consulte [Aplicativos de destino de Acesso Condicional: Office 365](/azure/active-directory/conditional-access/concept-conditional-access-cloud-apps) |
| excludeApplications | Conjunto de cadeias de caracteres | Pode ser um dos seguintes: <li> A lista de IDs de cliente (**appId**) explicitamente excluídas da política.<li> `Office365`- Para obter a lista de aplicativos incluídos`Office365`, consulte [Aplicativos de destino de Acesso Condicional: Office 365](/azure/active-directory/conditional-access/concept-conditional-access-cloud-apps) |
| includeUserActions | Conjunto de cadeias de caracteres | Ações do usuário a serem incluídos. Os valores com suporte são `urn:user:registersecurityinfo` e `urn:user:registerdevice` |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeApplications",
    "excludeApplications",
    "includeUserActions"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessApplications"
}-->

```json
{
  "includeApplications": ["String"],
  "excludeApplications": ["String"],
  "includeUserActions": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessApplications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

