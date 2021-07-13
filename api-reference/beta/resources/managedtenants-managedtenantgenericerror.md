---
title: Tipo de recurso managedTenantGenericError
description: Representa um erro genérico para um locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d9cb6ac80bb48e7d8afc91db2cf386a21c7318e9
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401899"
---
# <a name="managedtenantgenericerror-resource-type"></a>Tipo de recurso managedTenantGenericError

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um erro genérico para um locatário gerenciado.

Herda de [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|erro|Cadeia de caracteres|A mensagem de erro da exceção. Herdado [de managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md). Obrigatório. Somente leitura.|
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
