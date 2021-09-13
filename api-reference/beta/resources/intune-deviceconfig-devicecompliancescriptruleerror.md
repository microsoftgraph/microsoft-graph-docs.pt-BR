---
title: Tipo de recurso deviceComplianceScriptRuleError
description: Ainda não documentado
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 019d4f1543b3dff8231b32feba1bb57ed8a5b174
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59064340"
---
# <a name="devicecompliancescriptruleerror-resource-type"></a>Tipo de recurso deviceComplianceScriptRuleError

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado


Herda de [deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|código|[code](../resources/intune-deviceconfig-code.md)|Código de erro. Herdado [de deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md). Os valores possíveis são: `none` , `jsonFileInvalid` , , `jsonFileMissing` `jsonFileTooLarge` , `rulesMissing` `duplicateRules` `tooManyRulesSpecified` `operatorMissing` `operatorNotSupported` `datatypeMissing` `datatypeNotSupported` `operatorDataTypeCombinationNotSupported` `moreInfoUriMissing` `moreInfoUriInvalid` `moreInfoUriTooLarge` `descriptionMissing` `descriptionInvalid` `descriptionTooLarge` `titleMissing` `titleInvalid` `titleTooLarge` `operandMissing` `operandInvalid` `operandTooLarge` `settingNameMissing` `settingNameInvalid` `settingNameTooLarge` `englishLocaleMissing` `duplicateLocales` `unrecognizedLocale` `unknown` `remediationStringsMissing`|
|deviceComplianceScriptRulesValidationError|[deviceComplianceScriptRulesValidationError](../resources/intune-deviceconfig-devicecompliancescriptrulesvalidationerror.md)|Código de erro. Herdado [de deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md). Os valores possíveis são: `none` , `jsonFileInvalid` , , `jsonFileMissing` `jsonFileTooLarge` , `rulesMissing` `duplicateRules` `tooManyRulesSpecified` `operatorMissing` `operatorNotSupported` `datatypeMissing` `datatypeNotSupported` `operatorDataTypeCombinationNotSupported` `moreInfoUriMissing` `moreInfoUriInvalid` `moreInfoUriTooLarge` `descriptionMissing` `descriptionInvalid` `descriptionTooLarge` `titleMissing` `titleInvalid` `titleTooLarge` `operandMissing` `operandInvalid` `operandTooLarge` `settingNameMissing` `settingNameInvalid` `settingNameTooLarge` `englishLocaleMissing` `duplicateLocales` `unrecognizedLocale` `unknown` `remediationStringsMissing`|
|mensagem|String|Mensagem de erro. Herdado [de deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)|
|settingName|Cadeia de caracteres|Definindo o nome da regra com erro.|

## <a name="relationships"></a>Relações
Nenhum

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
  "deviceComplianceScriptRulesValidationError": "String",
  "message": "String",
  "settingName": "String"
}
```



