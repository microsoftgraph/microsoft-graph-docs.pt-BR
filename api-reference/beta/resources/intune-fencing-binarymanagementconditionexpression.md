---
title: tipo de recurso de binaryManagementConditionExpression
description: Uma expressão de condição de gerenciamento que é avaliada usando uma operação de binário.
author: tfitzmac
ms.openlocfilehash: 6f271be2527427daaa04436899552abb4d21475e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357516"
---
# <a name="binarymanagementconditionexpression-resource-type"></a>tipo de recurso de binaryManagementConditionExpression

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma expressão de condição de gerenciamento que é avaliada usando uma operação de binário.

Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|operador|[binaryManagementConditionExpressionOperatorType](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|O operador usado na avaliação da operação binário. Os valores possíveis são: `or` e `and`.|
|firstOperand|[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)|O primeiro operando da operação binário.|
|secondOperand|[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)|O segundo operando da operação binário.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.binaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.binaryManagementConditionExpression",
  "operator": "String",
  "firstOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  },
  "secondOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```





