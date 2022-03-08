---
title: Tipo de recurso cloudPcRemoteActionResult
description: Representa o resultado da ação remota especificada pelo computador na nuvem.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 9b708df825104cd85175543b7c16850c16d40d0d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336022"
---
# <a name="cloudpcremoteactionresult-resource-type"></a>Tipo de recurso cloudPcRemoteActionResult

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o resultado da ação remota especificada pelo computador na nuvem.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[getCloudPcRemoteActionResults](../api/manageddevice-getcloudpcremoteactionresults.md)|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|Verifique os resultados de ação remota especificados pelo computador na nuvem. O Cloud PC dá suporte a reprovisionamento e ressarmos ações remotas.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|actionName|Cadeia de caracteres|A ação especificada. Os valores suportados no portal Microsoft Endpoint Manager são: `Reprovision`, , `Resize``Restore`. Os valores suportados em dispositivos cloud pc corporativos são: `Reboot`, `Rename`, , `Reprovision``Troubleshoot`.|
|actionState|[actionState](#actionstate-values)|Estado da ação. Os valores possíveis são: `None`, `pending`, `canceled`, `active`, `done`, `failed` e `notSupported`. Somente leitura.|
|cloudPcId|String|A ID do dispositivo cloud pc no qual a ação remota é executada. Somente leitura.|
|managedDeviceId|String|A ID do dispositivo gerenciado do Intune no qual a ação remota é executada. Somente leitura.|
|startDateTime|DateTimeOffset|Hora em que a ação foi iniciada. O Timestamp é mostrado no formato ISO 8601 e tempo universal coordenado (UTC). Por exemplo, meia-noite UTC em 1º de janeiro de 2014 aparece como '2014-01-01T00:00:00Z'.|
|lastUpdatedDateTime|DateTimeOffset|Hora da última atualização para ação. O Timestamp é mostrado no formato ISO 8601 e tempo universal coordenado (UTC). Por exemplo, meia-noite UTC em 1º de janeiro de 2014 aparece como '2014-01-01T00:00:00Z'.|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcStatusDetails.md)|Os detalhes do status do computador na nuvem. |

### <a name="actionstate-values"></a>valores actionState

|Member|Descrição|
|:---|:---|
|none|Não é um estado de ação válido.|
|pendente|A ação está pendente.|
|cancelado|A ação foi cancelada.|
|active|A ação está ativa.|
|done|Ação concluída sem erros.|
|failed|Falha na ação.|
|notSupported|Não há suporte para ação.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcRemoteActionResult"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcRemoteActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "cloudPcId": "String",
  "managedDeviceId": "String",
  "statusDetails": {
    "@odata.type": "microsoft.graph.cloudPcStatusDetails"
  }
}
```
