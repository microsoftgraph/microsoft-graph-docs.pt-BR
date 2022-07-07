---
title: Tipo de recurso win32LobAppPowerShellScriptRule
description: Um tipo complexo para armazenar os dados de regra de script do PowerShell para um aplicativo LOB win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fdfff5d8a80d7c9ad6184dd4aa179975d5891fbd
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66666771"
---
# <a name="win32lobapppowershellscriptrule-resource-type"></a>Tipo de recurso win32LobAppPowerShellScriptRule

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um tipo complexo para armazenar os dados de regra de script do PowerShell para um aplicativo LOB win32.


Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|O tipo de regra que indica a finalidade da regra. Herdado [de win32LobAppRule](../resources/intune-apps-win32lobapprule.md). Os valores possíveis são: `detection` e `requirement`.|
|displayName|Cadeia de caracteres|O nome de exibição da regra. Não especifique esse valor se a regra for usada para detecção.|
|enforceSignatureCheck|Boolean|Um valor que indica se uma verificação de assinatura é imposta.|
|runAs32Bit|Boolean|Um valor que indica se o script deve ser executado como 32 bits.|
|runAsAccount|[runAsAccountType](../resources/intune-apps-runasaccounttype.md)|O contexto de execução do script. Não especifique esse valor se a regra for usada para detecção. As regras de detecção de script serão executadas no mesmo contexto que o contexto de instalação do aplicativo associado. Os valores possíveis são: `system` e `user`.|
|scriptContent|Cadeia de caracteres|O conteúdo do script codificado em base64.|
|operationType|[win32LobAppPowerShellScriptRuleOperationType](../resources/intune-apps-win32lobapppowershellscriptruleoperationtype.md)|O tipo de operação de comparação de saída de script. Use NotConfigured (o valor padrão) se a regra for usada para detecção. Os valores possíveis são: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.|
|operator|[win32LobAppRuleOperator](../resources/intune-apps-win32lobappruleoperator.md)|O operador de saída de script. Use NotConfigured (o valor padrão) se a regra for usada para detecção. Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|comparisonValue|Cadeia de caracteres|O valor de comparação de saída do script. Não especifique um valor se a regra for usada para detecção.|

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




