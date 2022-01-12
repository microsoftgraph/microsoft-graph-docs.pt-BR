---
title: Tipo de recurso managedTenantExecutionError
description: Representa uma exceção para uma operação de locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 92917d60cc3bd22da02a8d447c305e275bab51a3
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791893"
---
# <a name="managedtenantexecutionerror-resource-type"></a>Tipo de recurso managedTenantExecutionError

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma exceção para uma operação de locatário gerenciado.

Herda de [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|erro|String|A mensagem de erro da exceção. Herdado [de managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md). Obrigatório. Somente leitura.|
|errorDetails|String|Informações de erro adicionais para a exceção. Opcional. Somente leitura.|
|nodeId|Int32|O identificador do nó onde ocorreu a exceção. Obrigatório. Somente leitura.|
|rawToken|String|O token da exceção. Opcional. Somente leitura.|
|statementIndex|Int32|O índice de instrução da exceção. Obrigatório. Somente leitura.|
|tenantId|String|O Azure Active Directory de locatário do locatário gerenciado. Herdado [de managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md). Obrigatório. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managedTenantExecutionError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenantExecutionError",
  "tenantId": "String",
  "error": "String",
  "rawToken": "String",
  "statementIndex": "Integer",
  "nodeId": "Integer",
  "errorDetails": "String"
}
```
