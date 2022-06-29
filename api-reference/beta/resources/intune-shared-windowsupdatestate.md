---
title: Tipo de recurso windowsUpdateState
description: Tipo de recurso windowsUpdateState
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1fcebd4d516d7cc91a3c33163b3325676b824b4a
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444513"
---
# <a name="windowsupdatestate-resource-type"></a>Tipo de recurso windowsUpdateState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsUpdateStates](../api/intune-shared-windowsupdatestate-list.md)|[coleção windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Listar propriedades e relações dos [objetos windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .|
|[Obter windowsUpdateState](../api/intune-shared-windowsupdatestate-get.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Ler propriedades e relações do objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .|
|[Criar windowsUpdateState](../api/intune-shared-windowsupdatestate-create.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Crie um novo [objeto windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .|
|[Excluir windowsUpdateState](../api/intune-shared-windowsupdatestate-delete.md)|Nenhum|Exclui um [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).|
|[Atualizar windowsUpdateState](../api/intune-shared-windowsupdatestate-update.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Atualize as propriedades de um [objeto windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Essa é a ID da entidade.|
|deviceId|Cadeia de caracteres|A ID do dispositivo.|
|userId|Cadeia de caracteres|A ID do usuário.|
|deviceDisplayName|Cadeia de caracteres|Nome de exibição do dispositivo.|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário.|
|status|[windowsUpdateStatus](/resources/intune-shared-windowsupdatestatus.md)|Status de udpate do Windows. Os valores possíveis são: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.|
|qualityUpdateVersion|Cadeia de caracteres|A versão de atualização de qualidade do dispositivo.|
|featureUpdateVersion|Cadeia de caracteres|A versão atual de atualização de recursos do dispositivo.|
|lastScanDateTime|DateTimeOffset|A data em que o agente Windows Update fez uma verificação bem-sucedida.|
|lastSyncDateTime|DateTimeOffset|Última data em que o dispositivo é sincronizado com Microsoft Intune.|

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



