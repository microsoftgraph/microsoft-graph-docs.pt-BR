---
title: tipo de recurso configurationManagerClientHealthState
description: Estado de integridade do cliente de gerenciador de configurações
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e0ed47d34f8f3d749ccab7d2788528c9b12679f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943008"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a>tipo de recurso configurationManagerClientHealthState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de integridade do cliente de gerenciador de configurações

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|state|[configurationManagerClientState](../resources/intune-devices-configurationmanagerclientstate.md)|Estado atual do cliente do Configuration Manager. Os valores possíveis são: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.|
|errorCode|Int32|Código de erro para estado de falha.|
|lastSyncDateTime|DateTimeOffset|DateTime fo última sincronização com o ponto de gerenciamento do Configuration Manager.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientHealthState",
  "state": "String",
  "errorCode": 1024,
  "lastSyncDateTime": "String (timestamp)"
}
```




