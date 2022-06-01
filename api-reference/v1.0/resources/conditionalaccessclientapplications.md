---
title: Tipo de recurso conditionalAccessClientApplications
description: Representa aplicativos cliente (entidades de serviço e identidades de carga de trabalho) incluídos e excluídos do escopo da política.
author: calebb
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0afcbcc68291d73aa83f9d730d81c257932c1dd7
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819059"
---
# <a name="conditionalaccessclientapplications-resource-type"></a>Tipo de recurso conditionalAccessClientApplications

Namespace: microsoft.graph

Representa aplicativos cliente (entidades de serviço e identidades de carga de trabalho) incluídos e excluídos do escopo da política.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|excludeServicePrincipals|Coleção de cadeias de caracteres|IDs da entidade de serviço excluídas do escopo da política.|
|includeServicePrincipals|Coleção de cadeias de caracteres|IDs da entidade de serviço incluídas no escopo da política ou `ServicePrincipalsInMyTenant`. |

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

