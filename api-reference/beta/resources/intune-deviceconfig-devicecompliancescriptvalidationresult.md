---
title: Tipo de recurso deviceComplianceScriptValidationResult
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2f6a7d25551f386d17d8882f9c693079e0a5b788de3af2de868ce9ede56d4c4c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54245034"
---
# <a name="devicecompliancescriptvalidationresult-resource-type"></a>Tipo de recurso deviceComplianceScriptValidationResult

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|rules|[Coleção deviceComplianceScriptRule](../resources/intune-deviceconfig-devicecompliancescriptrule.md)|Regras analisados de json.|
|scriptErrors|[Coleção deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)|Erros no json para o script.|
|ruleErrors|[Coleção deviceComplianceScriptRuleError](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md)|Erros no json para o script de regras.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptValidationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptValidationResult",
  "rules": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptRule",
      "settingName": "String",
      "operator": "String",
      "deviceComplianceScriptRulOperator": "String",
      "dataType": "String",
      "deviceComplianceScriptRuleDataType": "String",
      "operand": "String"
    }
  ],
  "scriptErrors": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptError",
      "code": "String",
      "deviceComplianceScriptRulesValidationError": "String",
      "message": "String"
    }
  ],
  "ruleErrors": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptRuleError",
      "code": "String",
      "deviceComplianceScriptRulesValidationError": "String",
      "message": "String",
      "settingName": "String"
    }
  ]
}
```




