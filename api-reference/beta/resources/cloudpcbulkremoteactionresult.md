---
title: Tipo de recurso cloudPcBulkRemoteActionResult
description: Representa o resultado da ação remota em massa especificada pelo computador na nuvem.
author: rongting
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 46f1336ec8f8cfa53813a73ac1230767f3a2e937
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338160"
---
# <a name="cloudpcbulkremoteactionresult-resource-type"></a>Tipo de recurso cloudPcBulkRemoteActionResult

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o resultado da ação remota em massa especificada pelo computador na nuvem.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|failedDeviceIds|Coleção de cadeias de caracteres|Uma lista de todas as IDs de dispositivo gerenciado do Intune que concluíram a ação em massa com uma falha.|
|notFoundDeviceIds|String collection|Uma lista de todas as IDs de dispositivo gerenciado do Intune que não foram encontradas quando a ação em massa foi tentada.|
|notSupportedDeviceIds|Coleção de cadeias de caracteres|Uma lista de todas as IDs de dispositivo gerenciado do Intune que foram identificadas como sem suporte para a ação em massa.|
|successfulDeviceIds|Coleção de cadeias de caracteres|Uma lista de todas as IDs de dispositivo gerenciado do Intune que concluíram a ação em massa com êxito.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcBulkRemoteActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcBulkRemoteActionResult",
  "failedDeviceIds": [
    "String"
  ],
  "notFoundDeviceIds": [
    "String"
  ],
  "notSupportedDeviceIds": [
    "String"
  ],
  "successfulDeviceIds": [
    "String"
  ]
}
```

