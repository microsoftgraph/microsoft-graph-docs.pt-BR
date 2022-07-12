---
title: Tipo de recurso win32LobAppPowerShellScriptRule
description: Um tipo complexo para armazenar os dados de regra de script do PowerShell para um aplicativo LOB win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 307e93f1f41b31f8139d25d1d2b1fbf97fe7a10d
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730774"
---
# <a name="win32lobapppowershellscriptrule-resource-type"></a>Tipo de recurso win32LobAppPowerShellScriptRule

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um tipo complexo para armazenar os dados de regra de script do PowerShell para um aplicativo LOB win32.


Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|O tipo de regra que indica a finalidade da regra. Herdado [de win32LobAppRule](../resources/intune-apps-win32lobapprule.md). Os valores possíveis são: `detection` e `requirement`.|
|displayName|String|O nome de exibição da regra. Não especifique esse valor se a regra for usada para detecção.|
|enforceSignatureCheck|Booliano|Um valor que indica se uma verificação de assinatura é imposta.|
|runAs32Bit|Booliano|Um valor que indica se o script deve ser executado como 32 bits.|
|runAsAccount|[runAsAccountType](../resources/intune-apps-runasaccounttype.md)|O contexto de execução do script. Não especifique esse valor se a regra for usada para detecção. As regras de detecção de script serão executadas no mesmo contexto que o contexto de instalação do aplicativo associado. Os valores possíveis são: `system` e `user`.|
|scriptContent|String|O conteúdo do script codificado em base64.|
|operationType|[win32LobAppPowerShellScriptRuleOperationType](../resources/intune-apps-win32lobapppowershellscriptruleoperationtype.md)|O tipo de operação de comparação de saída de script. Use NotConfigured (o valor padrão) se a regra for usada para detecção. Os valores possíveis são: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.|
|operator|[win32LobAppRuleOperator](../resources/intune-apps-win32lobappruleoperator.md)|O operador de saída de script. Use NotConfigured (o valor padrão) se a regra for usada para detecção. Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|comparisonValue|String|O valor de comparação de saída do script. Não especifique um valor se a regra for usada para detecção.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptRule",
  "ruleType": "String",
  "displayName": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "runAsAccount": "String",
  "scriptContent": "String",
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```





