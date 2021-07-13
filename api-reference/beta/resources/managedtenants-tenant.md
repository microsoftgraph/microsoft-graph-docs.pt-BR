---
title: tipo de recurso de locatário
description: Representa um locatário associado à entidade de gerenciamento.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: ee4bd57aa4e7fa2ea15c86376389d3b6e12198ea
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402140"
---
# <a name="tenant-resource-type"></a>tipo de recurso de locatário

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um locatário associado à entidade de gerenciamento.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar locatários](../api/managedtenants-managedtenant-list-tenants.md)|[coleção microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md)|Obter uma lista dos objetos [de locatário](../resources/managedtenants-tenant.md) e suas propriedades.|
|[Obter locatário](../api/managedtenants-tenant-get.md)|[microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md)|Leia as propriedades e as relações de um [objeto tenant.](../resources/managedtenants-tenant.md)|
|[offboardTenant](../api/managedtenants-tenant-offboardtenant.md)|[microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md)|Desempla um locatário da plataforma de gerenciamento de vários locatários.|
|[resetTenantOnboardingStatus](../api/managedtenants-tenant-resettenantonboardingstatus.md)|[microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md)|Redefine o status de integração do locatário com a plataforma de gerenciamento de vários locatários.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contrato|[microsoft.graph.managedTenants.tenantContract](../resources/managedtenants-tenantcontract.md)|Os detalhes do relacionamento do locatário com a entidade de gerenciamento.|
|createdDateTime|DateTimeOffset|A data e a hora em que o locatário foi criado na plataforma de gerenciamento de vários locatários. Opcional. Somente leitura.|
|displayName|String|O nome de exibição do locatário. Obrigatório. Somente leitura.|
|id|Cadeia de caracteres|O Azure Active Directory do locatário para o locatário. Obrigatório. Somente leitura.|
|lastUpdatedDateTime|DateTimeOffset|A data e a hora em que o locatário foi atualizado pela última vez na plataforma de gerenciamento de vários locatários. Opcional. Somente leitura.|
|tenantId|String|O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md) Opcional. Somente leitura.|
|tenantStatusInformation|[microsoft.graph.managedTenants.tenantStatusInformation](../resources/managedtenants-tenantstatusinformation.md)|As informações de status de integração do locatário. Opcional. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenant",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenant",
  "id": "String (identifier)",
  "tenantId": "String",
  "displayName": "String",
  "contract": {
    "@odata.type": "microsoft.graph.managedTenants.tenantContract"
  },
  "tenantStatusInformation": {
    "@odata.type": "microsoft.graph.managedTenants.tenantStatusInformation"
  },
  "lastUpdatedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)"
}
```
