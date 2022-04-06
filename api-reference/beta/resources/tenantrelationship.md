---
title: Tipo de recurso tenantRelationship
description: Representa os vários tipos de relações de locatário.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 5873f7b2740b342619755ea3bdda3cdd587837ea
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587305"
---
# <a name="tenantrelationship-resource-type"></a>Tipo de recurso tenantRelationship

Namespace: microsoft.graph

Representa os vários tipos de relações de locatário.

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|delegatedAdminCustomers|[coleção delegatedAdminCustomer](../resources/delegatedadmincustomer.md)|O cliente que tem uma relação de administrador delegada com um parceiro da Microsoft.|
|delegatedAdminRelationships|[coleção delegatedAdminRelationship](../resources/delegatedadminrelationship.md)|Os detalhes dos privilégios administrativos delegados que um parceiro da Microsoft tem em um locatário do cliente.|
|managedTenants|[microsoft.graph.managedTenants.managedTenant](../resources/managedtenants-managedtenant.md)|As operações disponíveis para interagir com a plataforma de gerenciamento de vários locatários.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.tenantRelationship",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.tenantRelationship"
}
```
