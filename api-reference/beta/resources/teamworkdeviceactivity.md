---
title: Tipo de recurso teamworkDeviceActivity
description: Representa os detalhes da atividade para um Microsoft Teams habilitado para Microsoft Teams.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 43e9e81eb8c2f921ce3657bf42c4a94f17c7c236
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262274"
---
# <a name="teamworkdeviceactivity-resource-type"></a>Tipo de recurso teamworkDeviceActivity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes da atividade para um Microsoft Teams habilitado para [Microsoft Teams](../resources/teamworkdevice.md), incluindo os dispositivos periféricos ativos anexados ao dispositivo.

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter trabalho em equipeDeviceActivity](../api/teamworkdeviceactivity-get.md)|[teamworkDeviceActivity](../resources/teamworkdeviceactivity.md)|Leia as propriedades e as relações de um objeto [teamworkDeviceActivity](../resources/teamworkdeviceactivity.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|activePeripherals|[teamworkActivePeripherals](../resources/teamworkactiveperipherals.md)|Os dispositivos periféricos ativos anexados ao dispositivo.|
|createdBy|[identitySet](../resources/identityset.md)|Identidade do usuário que criou o documento de atividade do dispositivo.|
|createdDateTime|DateTimeOffset|A data e a hora UTC quando o documento de atividade do dispositivo foi criado.|
|id|Cadeia de caracteres|Identificador de documento. Herdado da [entidade](../resources/entity.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Identidade do usuário que modificou pela última vez os detalhes da atividade do dispositivo.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora UTC em que o detalhe da atividade do dispositivo foi modificado pela última vez.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkDeviceActivity",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDeviceActivity",
  "activePeripherals": {
    "@odata.type": "microsoft.graph.teamworkActivePeripherals"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```

