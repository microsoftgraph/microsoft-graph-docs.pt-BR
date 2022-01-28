---
title: Tipo de recurso teamworkConnection
description: Representa os detalhes sobre o status de conexão de um dispositivo Microsoft Teams habilitado para Microsoft Teams e seus periféricos.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a02096ce1a807d4d75db5ba12b40488ef268bb36
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262245"
---
# <a name="teamworkconnection-resource-type"></a>Tipo de recurso teamworkConnection

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes sobre o status de conexão de um dispositivo Microsoft Teams habilitado para [Microsoft Teams](../resources/teamworkdevice.md) e seus periféricos.
O status da conexão é útil quando você calcula a saúde do dispositivo como quando o periférico necessário não está conectado corretamente, a saúde do dispositivo muda para o estado crítico.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|connectionStatus|teamworkConnectionStatus|Indica se um componente/periférico está conectado/desconectado ou seu estado é desconhecido. Os valores possíveis são: `unknown`, `connected`, `disconnected`, `unknownFutureValue`.|
|lastModifiedDateTime|DateTimeOffset|Hora em que o estado foi alterado pela última vez. Por exemplo, indica conectado _desde_ quando o estado está `connected` e _desconectado_ desde quando o estado é `disconnected`.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkConnection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkConnection",
  "connectionStatus": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

