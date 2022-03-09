---
title: Tipo de recurso deviceManagementSettings
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8a8b0632eab2d33e9bc5676a807a0f949b90c528
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367682"
---
# <a name="devicemanagementsettings-resource-type"></a>Tipo de recurso deviceManagementSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deviceComplianceCheckinThresholdDays|Int32|O número de dias que tem um dispositivo pode ser executado sem fazer check-in para permanecer em conformidade.|
|isScheduledActionEnabled|Booliano|O recurso está habilitado ou não para ação agendada para a regra.|
|secureByDefault|Booliano|Quando true, o dispositivo deve ser incompatível quando não há nenhuma política de conformidade direcionada|
|enhancedJailBreak|Booliano|O recurso está habilitado ou não para detecção de jailbreak aprimorada.|
|deviceInactivityBeforeRetirementInDay|Int32|Quando o dispositivo não faz check-in para o número especificado de dias, os dados da empresa podem ser removidos e o dispositivo não estará sob gerenciamento. Valores válidos de 30 a 270|
|derivedCredentialProvider|[derivedCredentialProviderType](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|O Provedor de Credenciais Derivado a ser usado para essa conta. Os valores possíveis são: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.|
|derivedCredentialUrl|Cadeia de caracteres|O URI de autoatendado do Provedor de Credenciais Derivado.|
|androidDeviceAdministratorEnrollmentEnabled|Booliano|A propriedade para determinar se o registro do administrador de dispositivo Android está habilitado para essa conta.|
|ignoreDevicesForUnsupportedSettingsEnabled|Booliano|A propriedade para determinar se deve ignorar as configurações de conformidade sem suporte em determinados modelos de dispositivos.|
|enableLogCollection|Booliano|Determina se o recurso de conjunto de log deve estar disponível para uso.|
|enableAutopilotDiagnostics|Booliano|Determina se o recurso de diagnóstico do piloto automático está habilitado ou não.|
|enableEnhancedTroubleshootingExperience|Booliano|Determina se o UX de solução de problemas aprimorado está habilitado ou não.|
|enableDeviceGroupMembershipReport|Booliano|Determina se o recurso de relatório de associação ao grupo de dispositivos está habilitado ou não.|

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
  "enableLogCollection": true,
  "enableAutopilotDiagnostics": true,
  "enableEnhancedTroubleshootingExperience": true,
  "enableDeviceGroupMembershipReport": true
}
```




