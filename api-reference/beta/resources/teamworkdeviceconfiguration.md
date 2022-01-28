---
title: Tipo de recurso teamworkDeviceConfiguration
description: Representa detalhes de configuração para um dispositivo Microsoft Teams habilitado para Microsoft Teams.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8d913040b86bbb1b2e669bbbcb0d622326603ef5
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262269"
---
# <a name="teamworkdeviceconfiguration-resource-type"></a>Tipo de recurso teamworkDeviceConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa detalhes de configuração para um dispositivo habilitado para [Microsoft Teams, incluindo](../resources/teamworkdevice.md) versões de software, configuração de dispositivo periférico (por exemplo, câmera, tela, microfone e alto-falante), configuração de hardware e Teams cliente.


Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter trabalho em equipeDeviceConfiguration](../api/teamworkdeviceconfiguration-get.md)|[teamworkDeviceConfiguration](../resources/teamworkdeviceconfiguration.md)|Leia as propriedades e as relações de um objeto [teamworkDeviceConfiguration](../resources/teamworkdeviceconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|cameraConfiguration|[teamworkCameraConfiguration](../resources/teamworkcameraconfiguration.md)|A configuração da câmera. Aplicável somente para dispositivos Salas do Microsoft Teams habilitados para Salas do Microsoft Teams.|
|createdBy|[identitySet](../resources/identityset.md)|Identidade do usuário que criou o documento de configuração do dispositivo.|
|createdDateTime|DateTimeOffset|A data e a hora UTC em que o documento de configuração do dispositivo foi criado.|
|displayConfiguration|[teamworkDisplayConfiguration](../resources/teamworkdisplayconfiguration.md)|A configuração de exibição.|
|hardwareConfiguration|[teamworkHardwareConfiguration](../resources/teamworkhardwareconfiguration.md)|A configuração de hardware. Aplicável somente para dispositivos Salas do Teams habilitados.|
|id|Cadeia de caracteres|Identificador de documento. Herdado da [entidade](../resources/entity.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Identidade do usuário que modificou pela última vez a configuração do dispositivo.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora UTC em que a configuração do dispositivo foi modificada pela última vez.|
|microphoneConfiguration|[teamworkMicrophoneConfiguration](../resources/teamworkmicrophoneconfiguration.md)|A configuração do microfone. Aplicável somente para dispositivos Salas do Teams habilitados.|
|softwareVersions|[teamworkDeviceSoftwareVersions](../resources/teamworkdevicesoftwareversions.md)|Informações relacionadas a versões de software para o dispositivo, como firmware, sistema operacional, cliente Teams cliente e agente de administração.|
|speakerConfiguration|[teamworkSpeakerConfiguration](../resources/teamworkspeakerconfiguration.md)|A configuração do alto-falante. Aplicável somente para dispositivos Salas do Teams habilitados.|
|systemConfiguration|[teamworkSystemConfiguration](../resources/teamworksystemconfiguration.md)|A configuração do sistema. Não aplicável para dispositivos Salas do Teams habilitados para uso.|
|teamsClientConfiguration|[teamworkTeamsClientConfiguration](../resources/teamworkteamsclientconfiguration.md)|A configuração Teams cliente. Aplicável somente para dispositivos Salas do Teams habilitados.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkDeviceConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDeviceConfiguration",
  "cameraConfiguration": {
    "@odata.type": "microsoft.graph.teamworkCameraConfiguration"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "displayConfiguration": {
    "@odata.type": "microsoft.graph.teamworkDisplayConfiguration"
  },
  "hardwareConfiguration": {
    "@odata.type": "microsoft.graph.teamworkHardwareConfiguration"
  },
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "microphoneConfiguration": {
    "@odata.type": "microsoft.graph.teamworkMicrophoneConfiguration"
  },
  "softwareVersions": {
    "@odata.type": "microsoft.graph.teamworkDeviceSoftwareVersions"
  },
  "speakerConfiguration": {
    "@odata.type": "microsoft.graph.teamworkSpeakerConfiguration"
  },
  "systemConfiguration": {
    "@odata.type": "microsoft.graph.teamworkSystemConfiguration"
  },
  "teamsClientConfiguration": {
    "@odata.type": "microsoft.graph.teamworkTeamsClientConfiguration"
  }
}
```

