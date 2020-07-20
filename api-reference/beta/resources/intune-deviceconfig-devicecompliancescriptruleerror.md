---
title: tipo de recurso deviceComplianceScriptRuleError
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a842d33c52774d2f2d5e251d32980e7cd28d4ec5
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44789296"
---
# <a name="devicecompliancescriptruleerror-resource-type"></a>tipo de recurso deviceComplianceScriptRuleError

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado


Herda de [deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|código|[code](../resources/intune-deviceconfig-code.md)|Código de erro. Herdado de [deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md). Os valores possíveis são:,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,, `none` `jsonFileInvalid` `jsonFileMissing` `jsonFileTooLarge` `rulesMissing` `duplicateRules` `tooManyRulesSpecified` `operatorMissing` `operatorNotSupported` `datatypeMissing` `datatypeNotSupported` `operatorDataTypeCombinationNotSupported` `moreInfoUriMissing` `moreInfoUriInvalid` `moreInfoUriTooLarge` `descriptionMissing` `descriptionInvalid` `descriptionTooLarge` `titleMissing` `titleInvalid` `titleTooLarge` `operandMissing` `operandInvalid` `operandTooLarge` `settingNameMissing` `settingNameInvalid` `settingNameTooLarge` `englishLocaleMissing` `duplicateLocales` `unrecognizedLocale` `unknown` `remediationStringsMissing` .|
|mensagem|String|Mensagem de erro. Herdado de [deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)|
|settingName|Cadeia de caracteres|Nome da configuração da regra com erro.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRuleError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRuleError",
  "code": "String",
  "message": "String",
  "settingName": "String"
}
```



