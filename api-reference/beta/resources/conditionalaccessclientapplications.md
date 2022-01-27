---
title: Tipo de recurso conditionalAccessClientApplications
description: Representa aplicativos cliente (entidades de serviço e identidades de carga de trabalho) incluídos e excluídos do escopo da política.
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ad30e86d9c434641e197338613f5f58cf5d2a788
ms.sourcegitcommit: de9df4bf6313b49afba74b6e9ef819907669c662
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2022
ms.locfileid: "62239369"
---
# <a name="conditionalaccessclientapplications-resource-type"></a>Tipo de recurso conditionalAccessClientApplications

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa aplicativos cliente (entidades de serviço e identidades de carga de trabalho) incluídos e excluídos do escopo da política.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|excludeServicePrincipals|String collection|IDs da entidade de serviço excluídas do escopo da política.|
|includeServicePrincipals|Conjunto de cadeias de caracteres|IDs da entidade de serviço incluídas no escopo da política ou `ServicePrincipalsInMyTenant` . |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessClientApplications"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessClientApplications",
  "includeServicePrincipals": [
    "String"
  ],
  "excludeServicePrincipals": [
    "String"
  ]
}
```

