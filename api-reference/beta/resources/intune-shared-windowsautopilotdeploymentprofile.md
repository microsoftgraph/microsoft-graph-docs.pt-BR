---
title: tipo de recurso windowsAutopilotDeploymentProfile
description: Perfil de implantação do Windows AutoPilot
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 196355a03a6c86a62765bc2b513670315d3311c2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255578"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a>tipo de recurso windowsAutopilotDeploymentProfile

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Perfil de implantação do Windows AutoPilot

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter windowsAutopilotDeploymentProfile](../api/intune-shared-windowsautopilotdeploymentprofile-get.md)|[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Leia as propriedades e as relações do objeto [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) .|
|[atribuir ação](../api/intune-shared-windowsautopilotdeploymentprofile-assign.md)|Nenhuma|Ainda não documentado|
|**Conjunto de políticas**|
|[ação hasPayloadLinks](../api/intune-shared-windowsautopilotdeploymentprofile-haspayloadlinks.md)|coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave de perfil|
|displayName|String|Nome do perfil|
|description|String|Descrição do perfil|
|idioma|Cadeia de caracteres|Idioma configurado no dispositivo|
|createdDateTime|DateTimeOffset|Hora de criação do perfil|
|lastModifiedDateTime|DateTimeOffset|Hora da última modificação do perfil|
|outOfBoxExperienceSettings|[outOfBoxExperienceSettings](../resources/intune-enrollment-outofboxexperiencesettings.md)|Configuração de experiência inicial da caixa|
|enrollmentStatusScreenSettings|[windowsEnrollmentStatusScreenSettings](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|Configuração da tela status do registro|
|extractHardwareHash|Booliano|Extração HardwareHash para o perfil|
|deviceNameTemplate|String|O modelo usado para nomear o dispositivo de piloto automático. Pode ser um texto personalizado e também pode conter o número de série do dispositivo ou um número gerado aleatoriamente. O comprimento total do texto gerado pelo modelo não pode ter mais de 15 caracteres.|
|deviceType|[windowsAutopilotDeviceType](../resources/intune-enrollment-windowsautopilotdevicetype.md)|O tipo de dispositivo piloto automático ao qual esse perfil se aplica. Os valores possíveis são: `windowsPc` e `surfaceHub2`.|
|enableWhiteGlove|Booliano|Habilite o Glove branco do piloto automático para o perfil.|
|roleScopeTagIds|Coleção de cadeias de caracteres|Marcas de escopo para o perfil.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Enrollmentid**|
|assignedDevices|coleção [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|A lista de dispositivos atribuídos para o perfil.|
|assignments|coleção [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|A lista de atribuições de grupo para o perfil.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeploymentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "language": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "String",
    "deviceUsageType": "String",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "String",
    "installProgressTimeoutInMinutes": 1024,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "String",
  "deviceType": "String",
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```




