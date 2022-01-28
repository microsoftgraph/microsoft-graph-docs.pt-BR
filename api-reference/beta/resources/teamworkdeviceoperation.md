---
title: Tipo de recurso teamworkDeviceOperation
description: Representa detalhes sobre operações assíncronas em execução em um Microsoft Teams habilitado para Microsoft Teams.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 513e18da8ed8432ce988c15f9737944d2493df3d
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262289"
---
# <a name="teamworkdeviceoperation-resource-type"></a>Tipo de recurso teamworkDeviceOperation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa detalhes sobre operações assíncronas em execução em um dispositivo Microsoft Teams habilitado para [Microsoft Teams](../resources/teamworkdevice.md), incluindo o status da operação. Qualquer operação assíncrona em execução em um dispositivo cria um objeto **teamworkDeviceOperation** .

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar trabalho em equipeDeviceOperations](../api/teamworkdeviceoperation-list.md)|[Coleção teamworkDeviceOperation](../resources/teamworkdeviceoperation.md)|Obter uma lista dos objetos [teamworkDeviceOperation](../resources/teamworkdeviceoperation.md) e suas propriedades.|
|[Obter trabalho em equipeDeviceOperation](../api/teamworkdeviceoperation-get.md)|[teamworkDeviceOperation](../resources/teamworkdeviceoperation.md)|Leia as propriedades e as relações de um objeto [teamworkDeviceOperation](../resources/teamworkdeviceoperation.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|completedDateTime|DateTimeOffset|Hora em que a operação atingiu um estado final (por exemplo, `Successful`, `Failed`e `Cancelled`).|
|createdBy|[identitySet](../resources/identityset.md)|Identidade do usuário que criou a operação do dispositivo.|
|createdDateTime|DateTimeOffset|A data e a hora UTC em que a operação do dispositivo foi criada.|
|erro|[operationError](../resources/operationerror.md)|Os detalhes do erro só estão disponíveis em caso de falha no status.|
|id|Cadeia de caracteres|Identificador de documento. Herdado da [entidade](../resources/entity.md).|
|lastActionBy|[identitySet](../resources/identityset.md)|Identidade do usuário que modificou pela última vez a operação do dispositivo.|
|lastActionDateTime|DateTimeOffset|A data e a hora UTC em que a operação do dispositivo foi modificada pela última vez.|
|operationType|teamworkDeviceOperationType|Tipo de operação assíncrona em um dispositivo. Os valores possíveis são: `deviceRestart`, `configUpdate`, , `deviceDiagnostics`, `softwareUpdate`, `deviceManagementAgentConfigUpdate`, `remoteLogin`, `remoteLogout`, `unknownFutureValue`.|
|startedDateTime|DateTimeOffset|Hora em que a operação foi iniciada.|
|status|Cadeia de caracteres|O status atual da operação assíncrona, por exemplo, `Queued`, , `Scheduled``InProgress`, `Successful`, , `Cancelled`e `Failed`.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkDeviceOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDeviceOperation",
  "completedDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "error": {
    "@odata.type": "microsoft.graph.operationError"
  },
  "id": "String (identifier)",
  "lastActionBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastActionDateTime": "String (timestamp)",
  "operationType": "String",
  "startedDateTime": "String (timestamp)",
  "status": "String"
}
```

