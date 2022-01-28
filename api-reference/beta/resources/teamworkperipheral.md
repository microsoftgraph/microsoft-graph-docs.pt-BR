---
title: Tipo de recurso teamworkPeripheral
description: Representa os detalhes sobre os periféricos anexados a um dispositivo Microsoft Teams habilitado para uso.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 645cf2d64e50d4d46fe2e76ff8c92dcdf948c74f
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262283"
---
# <a name="teamworkperipheral-resource-type"></a>Tipo de recurso teamworkPeripheral

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes sobre os periféricos anexados a um dispositivo Microsoft Teams habilitado para [Microsoft Teams.](../resources/teamworkdevice.md)

Herda da [entidade](../resources/entity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome de exibição para o periférico.|
|id|Cadeia de caracteres|Identificador exclusivo para o periférico específico. Herdado da [entidade](../resources/entity.md).|
|productId|Cadeia de caracteres|A ID do produto do dispositivo. Cada produto de um fornecedor tem sua própria ID.|
|vendorId|Cadeia de caracteres|O identificador exclusivo do fornecedor do dispositivo. Cada fornecedor tem uma ID exclusiva.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkPeripheral",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkPeripheral",
  "displayName": "String",
  "id": "String (identifier)",
  "productId": "String",
  "vendorId": "String"
}
```

