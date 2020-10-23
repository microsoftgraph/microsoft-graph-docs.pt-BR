---
title: Tipo de recurso deviceManagementSettings
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ea20bce4019ff04c81170b895fd5d5445db027cd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707819"
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
|derivedCredentialUrl|String|O URI de autoatendimento do provedor de credenciais derivado.|
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





