---
title: Tipo de recurso printOperation
description: Representa uma operação de impressão universal de longa duração. Classe base para tipos de operação como printerCreateOperation.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 0630d05e30d415ad60f4dd7ea4e7f729506e41b2cc20bded955e1593a6f56161
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54138455"
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
|id|Cadeia de caracteres|O identificador da operação. Apenas leitura.|
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

