---
title: tipo de recurso windowsUpdateState
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 25b15487be765de8c45896b10101671359e2659e
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122480"
---
# <a name="windowsupdatestate-resource-type"></a>tipo de recurso windowsUpdateState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsUpdateStates](../api/intune-shared-windowsupdatestate-list.md)|coleção [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Listar Propriedades e relações dos objetos [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .|
|[Obter windowsUpdateState](../api/intune-shared-windowsupdatestate-get.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Leia as propriedades e as relações do objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .|
|[Criar windowsUpdateState](../api/intune-shared-windowsupdatestate-create.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Criar um novo objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .|
|[Excluir windowsUpdateState](../api/intune-shared-windowsupdatestate-delete.md)|Nenhum|Exclui [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).|
|[Atualizar windowsUpdateState](../api/intune-shared-windowsupdatestate-update.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Atualiza as propriedades de um objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Esta é a ID da entidade.|
|deviceId|Cadeia de caracteres|A ID do dispositivo.|
|userId|String|A ID do usuário.|
|deviceDisplayName|Cadeia de caracteres|Nome de exibição do dispositivo.|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário.|
|status|[windowsUpdateStatus](../resources/intune-shared-windowsupdatestatus.md)|Status do Windows UDPATE. Os valores possíveis são: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.|
|qualityUpdateVersion|Cadeia de caracteres|A versão de atualização de qualidade do dispositivo.|
|featureUpdateVersion|Cadeia de caracteres|A versão atual de atualização de recursos do dispositivo.|
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



