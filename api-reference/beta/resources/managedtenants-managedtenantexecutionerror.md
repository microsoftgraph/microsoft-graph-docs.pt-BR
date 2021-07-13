---
title: Tipo de recurso managedTenantExecutionError
description: Representa uma exceção para uma operação de locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 5a1fd2d1524cad663ee6acef93ab20cc8e40fd24
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401905"
---
# <a name="managedtenantexecutionerror-resource-type"></a>Tipo de recurso managedTenantExecutionError

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma exceção para uma operação de locatário gerenciado.

Herda de [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|erro|Cadeia de caracteres|A mensagem de erro da exceção. Herdado [de managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md). Obrigatório. Somente leitura.|
|errorDetails|Cadeia de caracteres|Informações de erro adicionais para a exceção. Opcional. Somente leitura.|
|nodeId|Int32|O identificador do nó onde ocorreu a exceção. Obrigatório. Somente leitura.|
|rawToken|Cadeia de caracteres|O token da exceção. Opcional. Somente leitura.|
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
