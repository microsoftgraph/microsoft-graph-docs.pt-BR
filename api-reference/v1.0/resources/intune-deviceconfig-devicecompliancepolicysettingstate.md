---
title: Tipo de recurso deviceCompliancePolicySettingState
description: Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 85de06b5baa9ff840ab0e1fd18cb70b0f5676e8b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962209"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a>Tipo de recurso deviceCompliancePolicySettingState

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|configuração|Cadeia de caracteres|A configuração que está sendo relatada|
|settingName|Cadeia de caracteres|Nome traduzido/amigável para o usuário da configuração que está sendo relatada|
|instanceDisplayName|Cadeia de caracteres|Nome da instância de configuração está sendo relatada.|
|estado|[complianceStatus](../resources/intune-shared-compliancestatus.md)|O estado de conformidade da configuração. Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|errorCode|Int64|Código de erro da configuração|
|errorDescription|Cadeia de caracteres|Descrição do erro|
|userId|Cadeia de caracteres|UserId|
|userName|Cadeia de caracteres|UserName|
|userEmail|Cadeia de caracteres|UserEmail|
|userPrincipalName|Cadeia de caracteres|UserPrincipalName.|
|sources|Coleção [settingSource](../resources/intune-deviceconfig-settingsource.md)|Políticas colaboradoras|
|currentValue|Cadeia de caracteres|Valor atual da configuração no dispositivo|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": 1024,
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "currentValue": "String"
}
```



