---
title: tipo de recurso de managementConditionExpressionString
description: Uma cadeia de caracteres de expressão de condição de gerenciamento é uma representação de cadeia de caracteres de uma expressão de condição de gerenciamento.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 872282914dc57be4e8e9bc7d476e7767907ec913
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968845"
---
# <a name="managementconditionexpressionstring-resource-type"></a>tipo de recurso de managementConditionExpressionString

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma cadeia de caracteres de expressão de condição de gerenciamento é uma representação de cadeia de caracteres de uma expressão de condição de gerenciamento.

Herda de [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|valor|Cadeia de caracteres|O valor de cadeia de caracteres do gerenciamento condição instrução expressão.|

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





