---
title: tipo de recurso activeDirectoryWindowsAutopilotDeploymentProfile
description: Perfil de implantação do Windows AutoPilot
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5d1ce8270848c70bebffe88f739b86102809e428
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196641"
---
# <a name="activedirectorywindowsautopilotdeploymentprofile-resource-type"></a>tipo de recurso activeDirectoryWindowsAutopilotDeploymentProfile

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Perfil de implantação do Windows AutoPilot


Herda de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar activeDirectoryWindowsAutopilotDeploymentProfiles](../api/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile-list.md)|coleção [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)|Listar Propriedades e relações dos objetos [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .|
|[Obter activeDirectoryWindowsAutopilotDeploymentProfile](../api/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile-get.md)|[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)|Leia as propriedades e as relações do objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .|
|[Criar activeDirectoryWindowsAutopilotDeploymentProfile](../api/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile-create.md)|[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)|Criar um novo objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .|
|[Excluir activeDirectoryWindowsAutopilotDeploymentProfile](../api/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile-delete.md)|Nenhum|Exclui [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).|
|[Atualizar activeDirectoryWindowsAutopilotDeploymentProfile](../api/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile-update.md)|[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)|Atualiza as propriedades de um objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave de perfil herdada de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|displayName|String|Nome do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|descrição|String|Descrição do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|idioma|Cadeia de caracteres|Idioma configurado no dispositivo herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|createdDateTime|DateTimeOffset|Tempo de criação de perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|lastModifiedDateTime|DateTimeOffset|Hora da última modificação do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|outOfBoxExperienceSettings|[outOfBoxExperienceSettings](../resources/intune-enrollment-outofboxexperiencesettings.md)|Configuração de experiência inicial da caixa herdada de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|enrollmentStatusScreenSettings|[windowsEnrollmentStatusScreenSettings](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|Configuração da tela de status do registro herdada de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|extractHardwareHash|Booliano|Extração HardwareHash para o perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|deviceNameTemplate|String|O modelo usado para nomear o dispositivo de piloto automático. Pode ser um texto personalizado e também pode conter o número de série do dispositivo ou um número gerado aleatoriamente. O comprimento total do texto gerado pelo modelo não pode ter mais de 15 caracteres. Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|deviceType|[windowsAutopilotDeviceType](../resources/intune-enrollment-windowsautopilotdevicetype.md)|O tipo de dispositivo piloto automático ao qual esse perfil se aplica. Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md). Os valores possíveis são: `windowsPc` e `surfaceHub2`.|
|enableWhiteGlove|Booliano|Habilite o Glove branco do piloto automático para o perfil. Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Marcas de escopo para o perfil. Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignedDevices|coleção [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|A lista de dispositivos atribuídos para o perfil. Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|assignments|coleção [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|A lista de atribuições de grupo para o perfil. Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|domainJoinConfiguration|windowsDomainJoinConfiguration|Configuração para ingressar no domínio do Active Directory|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
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



