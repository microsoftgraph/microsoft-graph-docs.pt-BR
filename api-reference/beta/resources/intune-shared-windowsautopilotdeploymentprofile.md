---
title: Tipo de recurso windowsAutopilotDeploymentProfile
description: Windows Autopilot Deployment Perfil
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a914b132eb01589d90788910349c261faf4b4c8e086908519470427d255317ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54160881"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a>Tipo de recurso windowsAutopilotDeploymentProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows Autopilot Deployment Perfil

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter windowsAutopilotDeploymentProfile](../api/intune-shared-windowsautopilotdeploymentprofile-get.md)|[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Leia propriedades e relações do [objeto windowsAutopilotDeploymentProfile.](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|[atribuir ação](../api/intune-shared-windowsautopilotdeploymentprofile-assign.md)|Nenhuma|Ainda não documentado|
|**Conjunto de Políticas**|
|[Ação hasPayloadLinks](../api/intune-shared-windowsautopilotdeploymentprofile-haspayloadlinks.md)|[coleção hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave de Perfil|
|displayName|Cadeia de caracteres|Nome do perfil|
|description|Cadeia de caracteres|Descrição do perfil|
|idioma|Cadeia de caracteres|Idioma configurado no dispositivo|
|createdDateTime|DateTimeOffset|Tempo de criação de perfil|
|lastModifiedDateTime|DateTimeOffset|Tempo de última modificação do perfil|
|outOfBoxExperienceSettings|[outOfBoxExperienceSettings](../resources/intune-enrollment-outofboxexperiencesettings.md)|Configuração de experiência in-locar|
|enrollmentStatusScreenSettings|[windowsEnrollmentStatusScreenSettings](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|Configuração da tela de status do registro|
|extractHardwareHash|Boolean|Extração de HardwareHash para o perfil|
|deviceNameTemplate|Cadeia de caracteres|O modelo usado para nomear o Dispositivo AutoPilot. Pode ser um texto personalizado e também pode conter o número de série do dispositivo ou um número gerado aleatoriamente. O comprimento total do texto gerado pelo modelo não pode ter mais de 15 caracteres.|
|deviceType|[windowsAutopilotDeviceType](../resources/intune-enrollment-windowsautopilotdevicetype.md)|O tipo de dispositivo AutoPilot ao qual esse perfil é aplicável. Os valores possíveis são: `windowsPc` e `surfaceHub2`.|
|enableWhiteGlove|Boolean|Habilitar o Autopilot White Glove para o perfil.|
|roleScopeTagIds|String collection|Marcas de escopo para o perfil.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Inscrição**|
|assignedDevices|[Coleção windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|A lista de dispositivos atribuídos para o perfil.|
|assignments|[Coleção windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|A lista de atribuições de grupo para o perfil.|

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




