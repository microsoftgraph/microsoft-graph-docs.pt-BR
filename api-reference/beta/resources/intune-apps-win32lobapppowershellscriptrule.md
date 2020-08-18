---
title: tipo de recurso win32LobAppPowerShellScriptRule
description: Um tipo complexo para armazenar os dados da regra de script do PowerShell para um aplicativo LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ce2080b2907f8c691282b44ba6f6ff1ec57a6ed
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792706"
---
# <a name="win32lobapppowershellscriptrule-resource-type"></a>tipo de recurso win32LobAppPowerShellScriptRule

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um tipo complexo para armazenar os dados da regra de script do PowerShell para um aplicativo LOB Win32.


Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|O tipo de regra que indica o objetivo da regra. Herdado de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md). Os valores possíveis são: `detection` e `requirement`.|
|displayName|String|O nome de exibição da regra. Não especifique esse valor se a regra for usada para detecção.|
|enforceSignatureCheck|Booliano|Um valor que indica se uma verificação de assinatura é imposta.|
|runAs32Bit|Booliano|Um valor que indica se o script deve ser executado como 32 bits.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|O contexto de execução do script. Não especifique esse valor se a regra for usada para detecção. As regras de detecção de script serão executadas no mesmo contexto do contexto de instalação de aplicativo associado. Os valores possíveis são: `system` e `user`.|
|scriptContent|String|O conteúdo de script codificado em base64.|
|OperationType|[win32LobAppPowerShellScriptRuleOperationType](../resources/intune-apps-win32lobapppowershellscriptruleoperationtype.md)|O tipo de operação de comparação de saída de script. Use não configurado (o valor padrão) se a regra for usada para detecção. Os valores possíveis são: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.|
|operator|[win32LobAppRuleOperator](../resources/intune-apps-win32lobappruleoperator.md)|O operador de saída de script. Use não configurado (o valor padrão) se a regra for usada para detecção. Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|ComparisonValue|String|O valor de comparação de saída do script. Não especifique um valor se a regra for usada para detecção.|

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



