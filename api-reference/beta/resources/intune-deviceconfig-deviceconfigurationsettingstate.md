---
title: tipo de recurso deviceConfigurationSettingState
description: Estado da definição de configuração de um determinado dispositivo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9355cdf0aab60208246fdae699cda78be65d62ff
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415184"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a>tipo de recurso deviceConfigurationSettingState

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Estado da definição de configuração de um determinado dispositivo.

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




