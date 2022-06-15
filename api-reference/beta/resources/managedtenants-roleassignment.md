---
title: Tipo de recurso roleAssignment
description: Representa a atribuição de função a um usuário conectado para um locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 8455036941676bd304f12d957220dd982530b6db
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096338"
---
# <a name="roleassignment-resource-type"></a>Tipo de recurso roleAssignment

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a atribuição de função a um usuário conectado para um [locatário gerenciado](../resources/managedtenants-tenant.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|assignmentType|delegatedPrivilegeStatus|O tipo das relações de administrador associadas à atribuição de função. Os valores possíveis são: `none`, `delegatedAdminPrivileges`, `unknownFutureValue`, `granularDelegatedAdminPrivileges`, `delegatedAndGranularDelegetedAdminPrivileges`. Observe que você deve usar o `Prefer: include-unknown-enum-members` cabeçalho da solicitação para obter os seguintes valores dessa [enumeração evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `granularDelegatedAdminPrivileges` , `delegatedAndGranularDelegetedAdminPrivileges`.|
|funções|[Coleção microsoft.graph.managedTenants.roleDefinition](../resources/managedtenants-roledefinition.md)|A coleção de funções atribuídas.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.roleAssignment",
  "assignmentType": "String",
  "roles": [
    {
      "@odata.type": "microsoft.graph.managedTenants.roleDefinition"
    }
  ]
}
```
