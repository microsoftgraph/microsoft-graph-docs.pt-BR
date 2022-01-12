---
title: Tipo de recurso conditionalAccessPolicyCoverage
description: Representa informações sobre qualquer política Azure Active Directory que define regras de acesso de um recurso para um determinado locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 686e587378b0dd921dedac4aac80cacfeafb885f
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61798750"
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
|conditionalAccessPolicyState|String|O estado da política de acesso condicional. Os valores possíveis são: `enabled`, `disabled`, `enabledForReportingButNotEnforced`. Obrigatório. Somente leitura.|
|id|String|O identificador exclusivo dessa entidade. Obrigatório. Somente leitura.|
|latestPolicyModifiedDateTime|DateTimeOffset|A data e a hora em que a política de acesso condicional foi modificada pela última vez. Obrigatório. Somente leitura.|
|requiresDeviceCompliance|Boolean|Um sinalizador indicando se a política de acesso condicional requer conformidade do dispositivo. Obrigatório. Somente leitura.|
|tenantDisplayName|String|O nome de exibição do locatário gerenciado. Obrigatório. Somente leitura.|

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
