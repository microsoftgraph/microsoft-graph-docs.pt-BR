---
title: Tipo de recurso win32LobAppPowerShellScriptRule
description: Um tipo complexo para armazenar os dados da regra de script do PowerShell para um aplicativo LOB win32.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4022174368b23895a31e89cacd45e393ba894d3e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057506"
---
# <a name="win32lobapppowershellscriptrule-resource-type"></a>Tipo de recurso win32LobAppPowerShellScriptRule

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um tipo complexo para armazenar os dados da regra de script do PowerShell para um aplicativo LOB win32.


Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|O tipo de regra que indica a finalidade da regra. Herdado [de win32LobAppRule](../resources/intune-apps-win32lobapprule.md). Os valores possíveis são: `detection` e `requirement`.|
|displayName|Cadeia de caracteres|O nome de exibição da regra. Não especifique esse valor se a regra for usada para detecção.|
|enforceSignatureCheck|Boleano|Um valor que indica se uma verificação de assinatura é imposta.|
|runAs32Bit|Boleano|Um valor que indica se o script deve ser executado como 32 bits.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|O contexto de execução do script. Não especifique esse valor se a regra for usada para detecção. As regras de detecção de script serão executados no mesmo contexto que o contexto de instalação do aplicativo associado. Os valores possíveis são: `system` e `user`.|
|scriptContent|Cadeia de Caracteres|O conteúdo de script codificado com base64.|
|operationType|[win32LobAppPowerShellScriptRuleOperationType](../resources/intune-apps-win32lobapppowershellscriptruleoperationtype.md)|O tipo de operação de comparação de saída de script. Use NotConfigured (o valor padrão) se a regra for usada para detecção. Os valores possíveis são: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.|
|operator|[win32LobAppRuleOperator](../resources/intune-apps-win32lobappruleoperator.md)|O operador de saída de script. Use NotConfigured (o valor padrão) se a regra for usada para detecção. Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|comparisonValue|Cadeia de Caracteres|O valor de comparação de saída de script. Não especifique um valor se a regra for usada para detecção.|

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



