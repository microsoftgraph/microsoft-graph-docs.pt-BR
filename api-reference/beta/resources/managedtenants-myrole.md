---
title: Tipo de recurso myRole
description: Representa as atribuições de função para um usuário conectado para um locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 3607702c037155efef1e0353b3551ba79f3eda9c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096339"
---
# <a name="myrole-resource-type"></a>Tipo de recurso myRole

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as atribuições de função para um usuário conectado para um [locatário gerenciado](../resources/managedtenants-tenant.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar myRoles](../api/managedtenants-managedtenant-list-myroles.md)|[Coleção microsoft.graph.managedTenants.myRole](../resources/managedtenants-myrole.md)|Obtenha as funções que o usuário conectado tem por meio de uma relação delegada entre [locatários gerenciados](../resources/managedtenants-tenant.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|assignments|[Coleção microsoft.graph.managedTenants.roleAssignment](../resources/managedtenants-roleassignment.md)|Uma coleção de atribuições de função para o [locatário gerenciado](../resources/managedtenants-tenant.md).|
|tenantId|String|O Azure Active Directory de locatário do locatário [gerenciado](../resources/managedtenants-tenant.md). Opcional. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.myRole",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.myRole",
  "assignments": [
    {
      "@odata.type": "microsoft.graph.managedTenants.roleAssignment"
    }
  ],
  "tenantId": "String"
}
```
