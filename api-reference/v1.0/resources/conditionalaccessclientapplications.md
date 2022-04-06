---
title: Tipo de recurso conditionalAccessClientApplications
description: Representa aplicativos cliente (entidades de serviço e identidades de carga de trabalho) incluídos e excluídos do escopo da política.
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f53d79f311d5f6be8b3d9ee0781636eb4c62c686
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672746"
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

