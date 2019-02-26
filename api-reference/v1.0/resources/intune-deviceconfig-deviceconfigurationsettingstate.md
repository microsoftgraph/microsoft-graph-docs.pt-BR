---
title: tipo de recurso deviceConfigurationSettingState
description: Estado da definição de configuração de um determinado dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d79d4c35572c98c82f80f8903d42cfa3b983c2e9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252900"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a>tipo de recurso deviceConfigurationSettingState

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado da definição de configuração de um determinado dispositivo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|configuração|String|A configuração que está sendo relatada|
|settingName|String|Nome traduzido/amigável para o usuário da configuração que está sendo relatada|
|instanceDisplayName|String|Nome da instância de configuração está sendo relatada.|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|O estado de conformidade da configuração. Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|errorCode|Int64|Código de erro da configuração|
|errorDescription|String|Descrição do erro|
|userId|String|UserId|
|userName|String|UserName|
|userEmail|String|UserEmail|
|userPrincipalName|String|UserPrincipalName.|
|sources|Coleção [settingSource](../resources/intune-deviceconfig-settingsource.md)|Políticas colaboradoras|
|currentValue|Cadeia de caracteres|Valor atual da configuração no dispositivo|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
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



