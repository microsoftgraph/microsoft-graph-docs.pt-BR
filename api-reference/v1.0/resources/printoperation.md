---
title: Tipo de recurso printOperation
description: Representa uma operação de impressão universal de longa duração. Classe base para tipos de operação como printerCreateOperation.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 9a397a0166ad62a503027499e9e0f5fd4f127b1e
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517034"
---
# <a name="printoperation-resource-type"></a>Tipo de recurso printOperation

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Representa uma operação de impressão universal de longa duração. Classe base para tipos de operação como [printerCreateOperation](printercreateoperation.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [Obter operação](../api/printoperation-get.md) | [printOperation](printoperation.md) | Recupere uma operação de longa duração dentro do usuário atual ou do locatário do aplicativo. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador da operação. Somente leitura.|
|status|[printOperationStatus](printoperationstatus.md)|O status da operação. Somente leitura.|
|createdDateTime|DateTimeOffset|DateTimeOffset quando a operação foi criada. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printOperation",
  "id": "String (identifier)",
  "status": {
    "@odata.type": "microsoft.graph.printOperationStatus"
  },
  "createdDateTime": "String (timestamp)"
}
```

