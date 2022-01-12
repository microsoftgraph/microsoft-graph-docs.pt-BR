---
title: Tipo de recurso tenantGroup
description: Representa um grupo lógico de locatários gerenciados.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: fa731082fbfc32f323b15460780e2ff355a965f8
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791859"
---
# <a name="tenantgroup-resource-type"></a>Tipo de recurso tenantGroup

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um grupo lógico de locatários gerenciados.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar tenantGroups](../api/managedtenants-managedtenant-list-tenantgroups.md)|[coleção microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md)|Obter uma lista dos objetos [tenantGroup](../resources/managedtenants-tenantgroup.md) e suas propriedades.|
|[Obter tenantGroup](../api/managedtenants-tenantgroup-get.md)|[microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md)|Leia as propriedades e as relações de um [objeto tenantGroup.](../resources/managedtenants-tenantgroup.md)|
|[tenantSearch](../api/managedtenants-tenantgroup-tenantsearch.md)|[coleção microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md)|Pesquisa o locatário gerenciado específico entre grupos de locatários.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allTenantsIncluded|Booliano|Um sinalizador indicando se todos os locatários gerenciados estão incluídos no grupo de locatários. Obrigatório. Somente leitura.|
|displayName|String|O nome de exibição do grupo de locatários. Opcional. Somente leitura.|
|id|String|O identificador exclusivo do grupo de locatários. Obrigatório. Somente leitura.|
|managementActions|[coleção microsoft.graph.managedTenants.managementActionInfo](../resources/managedtenants-managementactioninfo.md)|O conjunto de ações de gerenciamento associadas ao grupo de locatários. Opcional. Somente leitura.|
|managementIntents|[coleção microsoft.graph.managedTenants.managementIntentInfo](../resources/managedtenants-managementintentinfo.md)|A coleção de intenções de gerenciamento associadas ao grupo de locatários. Opcional. Somente leitura.|
|tenantIds|Coleção String|A coleção de identificadores de locatários gerenciados inclui no grupo de locatários. Opcional. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantGroup",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantGroup",
  "id": "String (identifier)",
  "displayName": "String",
  "allTenantsIncluded": "Boolean",
  "tenantIds": [
    "String"
  ],
  "managementIntents": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementIntentInfo"
    }
  ],
  "managementActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementActionInfo"
    }
  ]
}
```
