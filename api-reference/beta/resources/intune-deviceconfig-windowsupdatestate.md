---
title: tipo de recurso windowsUpdateState
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a023e4f74fe7a0abc96a47b79c7da7104617c9d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725825"
---
# <a name="windowsupdatestate-resource-type"></a>tipo de recurso windowsUpdateState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsUpdateStates](../api/intune-deviceconfig-windowsupdatestate-list.md)|coleção [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)|Listar Propriedades e relações dos objetos [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) .|
|[Obter windowsUpdateState](../api/intune-deviceconfig-windowsupdatestate-get.md)|[windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)|Leia as propriedades e as relações do objeto [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) .|
|[Criar windowsUpdateState](../api/intune-deviceconfig-windowsupdatestate-create.md)|[windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)|Criar um novo objeto [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) .|
|[Excluir windowsUpdateState](../api/intune-deviceconfig-windowsupdatestate-delete.md)|Nenhum|Exclui [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md).|
|[Atualizar windowsUpdateState](../api/intune-deviceconfig-windowsupdatestate-update.md)|[windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)|Atualiza as propriedades de um objeto [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Esta é a ID da entidade.|
|deviceId|String|A ID do dispositivo.|
|userId|String|A ID do usuário.|
|deviceDisplayName|Cadeia de caracteres|Nome de exibição do dispositivo.|
|userPrincipalName|String|Nome principal do usuário.|
|status|[windowsUpdateStatus](../resources/intune-deviceconfig-windowsupdatestatus.md)|Status do Windows UDPATE. Os valores possíveis são: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.|
|qualityUpdateVersion|String|A versão de atualização de qualidade do dispositivo.|
|featureUpdateVersion|String|A versão atual de atualização de recursos do dispositivo.|
|lastScanDateTime|DateTimeOffset|A data e hora em que o agente do Windows Update realizou uma verificação bem-sucedida.|
|lastSyncDateTime|DateTimeOffset|Data e hora da última sincronização do dispositivo com o Microsoft Intune.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "id": "String (identifier)",
  "deviceId": "String",
  "userId": "String",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "status": "String",
  "qualityUpdateVersion": "String",
  "featureUpdateVersion": "String",
  "lastScanDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)"
}
```





