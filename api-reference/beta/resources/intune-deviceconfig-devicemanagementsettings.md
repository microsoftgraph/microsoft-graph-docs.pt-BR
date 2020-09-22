---
title: Tipo de recurso deviceManagementSettings
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: be4356e2909898c4f93105733d3dc6e7322d7e34
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095286"
---
# <a name="devicemanagementsettings-resource-type"></a>Tipo de recurso deviceManagementSettings

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deviceComplianceCheckinThresholdDays|Int32|O número de dias que tem um dispositivo pode ser executado sem fazer check-in para permanecer em conformidade.|
|isScheduledActionEnabled|Booliano|O recurso está habilitado ou não para ação agendada para a regra.|
|secureByDefault|Booliano|Quando true, o dispositivo deve ser incompatível quando não há nenhuma política de conformidade direcionada|
|enhancedJailBreak|Boolean|O recurso está habilitado ou não para a detecção de jailbreak avançada.|
|deviceInactivityBeforeRetirementInDay|Int32|Quando o dispositivo não faz check-in por um número especificado de dias, os dados da empresa podem ser removidos e o dispositivo não estará sob gerenciamento. Valores válidos de 30 a 270|
|derivedCredentialProvider|[derivedCredentialProviderType](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|O provedor de credenciais derivado a ser usado para esta conta. Os valores possíveis são: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.|
|derivedCredentialUrl|Cadeia de caracteres|O URI de autoatendimento do provedor de credenciais derivado.|
|androidDeviceAdministratorEnrollmentEnabled|Boolean|A propriedade para determinar se o registro do administrador do dispositivo Android está habilitado para esta conta.|
|ignoreDevicesForUnsupportedSettingsEnabled|Boolean|A propriedade para determinar se deve ignorar as configurações de conformidade não suportadas em determinados modelos de dispositivos.|
|enableLogCollection|Boolean|Determina se o recurso de coleção de logs deve estar disponível para uso.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true,
  "enhancedJailBreak": true,
  "deviceInactivityBeforeRetirementInDay": 1024,
  "derivedCredentialProvider": "String",
  "derivedCredentialUrl": "String",
  "androidDeviceAdministratorEnrollmentEnabled": true,
  "ignoreDevicesForUnsupportedSettingsEnabled": true,
  "enableLogCollection": true
}
```






