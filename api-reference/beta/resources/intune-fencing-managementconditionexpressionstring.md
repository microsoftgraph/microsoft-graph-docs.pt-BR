---
title: tipo de recurso de managementConditionExpressionString
description: Uma cadeia de caracteres de expressão de condição de gerenciamento é uma representação de cadeia de caracteres de uma expressão de condição de gerenciamento.
ms.openlocfilehash: 456df27900aa10ead7e2bc090e5e06e0bcd7754f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040113"
---
# <a name="managementconditionexpressionstring-resource-type"></a>tipo de recurso de managementConditionExpressionString

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma cadeia de caracteres de expressão de condição de gerenciamento é uma representação de cadeia de caracteres de uma expressão de condição de gerenciamento.

Herda de [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|valor|String|O valor de cadeia de caracteres do gerenciamento condição instrução expressão.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementConditionExpressionString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionExpressionString",
  "value": "String"
}
```





