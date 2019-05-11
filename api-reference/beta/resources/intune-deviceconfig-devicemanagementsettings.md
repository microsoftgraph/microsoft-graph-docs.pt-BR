---
title: Tipo de recurso deviceManagementSettings
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 079d957d14e5f891af691ba7b41916adb8ac9669
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946963"
---
# <a name="devicemanagementsettings-resource-type"></a>Tipo de recurso deviceManagementSettings

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deviceComplianceCheckinThresholdDays|Int32|O número de dias que tem um dispositivo pode ser executado sem fazer check-in para permanecer em conformidade. Valores válidos de 0 a 120|
|isScheduledActionEnabled|Booliano|O recurso está habilitado ou não para ação agendada para a regra.|
|secureByDefault|Booliano|Quando true, o dispositivo deve ser incompatível quando não há nenhuma política de conformidade direcionada|
|enhancedJailBreak|Booliano|O recurso está habilitado ou não para a detecção de jailbreak avançada.|
|deviceInactivityBeforeRetirementInDay|Int32|Quando o dispositivo não faz check-in por um número especificado de dias, os dados da empresa podem ser removidos e o dispositivo não estará sob gerenciamento. Valores válidos de 30 a 270|
|derivedCredentialProvider|[derivedCredentialProviderType](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|O provedor de credenciais derivado a ser usado para esta conta. Os valores possíveis são: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.|
|derivedCredentialUrl|Cadeia de caracteres|O URI de autoatendimento do provedor de credenciais derivado.|

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
  "derivedCredentialUrl": "String"
}
```




