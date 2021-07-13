---
title: Tipo de recurso conditionalAccessPolicyCoverage
description: Representa informações sobre qualquer política Azure Active Directory que define regras de acesso de um recurso para um determinado locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: a4bc4f336692166ff032727a6fb13222edd9d7d9
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401943"
---
# <a name="conditionalaccesspolicycoverage-resource-type"></a>Tipo de recurso conditionalAccessPolicyCoverage

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações sobre qualquer política Azure Active Directory que define regras de acesso de um recurso para um determinado locatário gerenciado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar conditionalAccessPolicyCoverages](../api/managedtenants-managedtenant-list-conditionalaccesspolicycoverages.md)|[coleção microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md)|Obter uma lista dos [objetos conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) e suas propriedades.|
|[Obter conditionalAccessPolicyCoverage](../api/managedtenants-conditionalaccesspolicycoverage-get.md)|[microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md)|Leia as propriedades e as relações de [um objeto conditionalAccessPolicyCoverage.](../resources/managedtenants-conditionalaccesspolicycoverage.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|conditionalAccessPolicyState|Cadeia de caracteres|O estado da política de acesso condicional. Os valores possíveis são: `enabled`, `disabled`, `enabledForReportingButNotEnforced`. Obrigatório. Somente leitura.|
|id|Cadeia de caracteres|O identificador exclusivo dessa entidade. Obrigatório. Somente leitura.|
|latestPolicyModifiedDateTime|DateTimeOffset|A data e a hora em que a política de acesso condicional foi modificada pela última vez. Obrigatório. Somente leitura.|
|requiresDeviceCompliance|Boolean|Um sinalizador indicando se a política de acesso condicional requer conformidade do dispositivo. Obrigatório. Somente leitura.|
|tenantDisplayName|Cadeia de caracteres|O nome de exibição do locatário gerenciado. Obrigatório. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
  "id": "String (identifier)",
  "tenantDisplayName": "String",
  "conditionalAccessPolicyState": "String",
  "requiresDeviceCompliance": "Boolean",
  "latestPolicyModifiedDateTime": "String (timestamp)"
}
```
