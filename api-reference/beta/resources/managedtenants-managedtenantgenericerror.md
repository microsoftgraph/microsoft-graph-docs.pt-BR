---
title: Tipo de recurso managedTenantGenericError
description: Representa um erro genérico para um locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 167d8a581f2e8020ea4efabf951d07c409947ef3
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61789975"
---
# <a name="managedtenantgenericerror-resource-type"></a>Tipo de recurso managedTenantGenericError

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um erro genérico para um locatário gerenciado.

Herda de [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|erro|String|A mensagem de erro da exceção. Herdado [de managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md). Obrigatório. Somente leitura.|
|tenantId|String|O Azure Active Directory de locatário do locatário gerenciado. Herdado [de managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md). Opcional. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managedTenantGenericError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenantGenericError",
  "tenantId": "String",
  "error": "String"
}
```
