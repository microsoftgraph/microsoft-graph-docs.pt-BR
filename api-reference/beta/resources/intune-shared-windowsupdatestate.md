---
title: Tipo de recurso windowsUpdateState
description: Ainda não documentado
author: rolyon
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a904a2c30d134b0b54ac20304ada5a5cbfabee79
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030007"
---
# <a name="windowsupdatestate-resource-type"></a>Tipo de recurso windowsUpdateState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsUpdateStates](../api/intune-shared-windowsupdatestate-list.md)|[Coleção windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Listar propriedades e relações dos [objetos windowsUpdateState.](../resources/intune-shared-windowsupdatestate.md)|
|[Obter windowsUpdateState](../api/intune-shared-windowsupdatestate-get.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Ler propriedades e relações do [objeto windowsUpdateState.](../resources/intune-shared-windowsupdatestate.md)|
|[Criar windowsUpdateState](../api/intune-shared-windowsupdatestate-create.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Crie um novo [objeto windowsUpdateState.](../resources/intune-shared-windowsupdatestate.md)|
|[Excluir windowsUpdateState](../api/intune-shared-windowsupdatestate-delete.md)|Nenhum|Exclui um [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).|
|[Atualizar windowsUpdateState](../api/intune-shared-windowsupdatestate-update.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Atualize as propriedades de um [objeto windowsUpdateState.](../resources/intune-shared-windowsupdatestate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Esta é a ID da entidade.|
|deviceId|Cadeia de caracteres|A id do dispositivo.|
|userId|Cadeia de caracteres|A id do usuário.|
|deviceDisplayName|Cadeia de caracteres|Nome de exibição do dispositivo.|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário.|
|status|[windowsUpdateStatus](../resources/intune-shared-windowsupdatestatus.md)|Windows status udpate. Os valores possíveis são: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.|
|qualityUpdateVersion|Cadeia de caracteres|A Versão de Atualização de Qualidade do dispositivo.|
|featureUpdateVersion|Cadeia de caracteres|A versão atual de atualização de recursos do dispositivo.|
|lastScanDateTime|DateTimeOffset|A data em que o Windows Update Agent fez uma verificação bem-sucedida.|
|lastSyncDateTime|DateTimeOffset|Última data em que o dispositivo sincroniza com Microsoft Intune.|

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



