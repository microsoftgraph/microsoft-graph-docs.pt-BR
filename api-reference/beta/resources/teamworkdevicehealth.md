---
title: Tipo de recurso teamworkDeviceHealth
description: Representa os detalhes de saúde de um Microsoft Teams habilitado para uso.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0c26b784f42dedc87b02e3a616ff93b7f0c1b46b
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262262"
---
# <a name="teamworkdevicehealth-resource-type"></a>Tipo de recurso teamworkDeviceHealth

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de saúde de um Microsoft Teams habilitado para [uso.](../resources/teamworkdevice.md) A saúde do dispositivo é calculada com base na configuração do dispositivo e em outros parâmetros de dispositivo.

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter trabalho em equipeDeviceHealth](../api/teamworkdevicehealth-get.md)|[teamworkDeviceHealth](../resources/teamworkdevicehealth.md)|Leia as propriedades e as relações de um objeto [teamworkDeviceHealth](../resources/teamworkdevicehealth.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|connection|[teamworkConnection](../resources/teamworkconnection.md)|Informações sobre o status da conexão.|
|createdBy|[identitySet](../resources/identityset.md)|Identidade do usuário que criou o documento de saúde do dispositivo.|
|createdDateTime|DateTimeOffset|A data e a hora UTC em que o documento de saúde do dispositivo foi criado.|
|hardwareHealth|[teamworkHardwareHealth](../resources/teamworkhardwarehealth.md)|Detalhes de saúde sobre o hardware do dispositivo.|
|id|Cadeia de caracteres|Identificador de documentos. Herdado da [entidade](../resources/entity.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Identidade do usuário que modificou pela última vez os detalhes de saúde do dispositivo.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora UTC em que o detalhe de saúde do dispositivo foi modificado pela última vez.|
|loginStatus|[teamworkLoginStatus](../resources/teamworkloginstatus.md)|O status de logon Microsoft Teams, Skype for Business e Exchange.|
|peripheralsHealth|[teamworkPeripheralsHealth](../resources/teamworkperipheralshealth.md)|Detalhes de saúde sobre todos os periféricos (por exemplo, alto-falante e microfone) anexados a um dispositivo.|
|softwareUpdateHealth|[teamworkSoftwareUpdateHealth](../resources/teamworksoftwareupdatehealth.md)|Atualizações de software disponíveis para o dispositivo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkDeviceHealth",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDeviceHealth",
  "connection": {
    "@odata.type": "microsoft.graph.teamworkConnection"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "hardwareHealth": {
    "@odata.type": "microsoft.graph.teamworkHardwareHealth"
  },
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "loginStatus": {
    "@odata.type": "microsoft.graph.teamworkLoginStatus"
  },
  "peripheralsHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralsHealth"
  },
  "softwareUpdateHealth": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateHealth"
  }
}
```

