---
title: Tipo de recurso printOperation
description: Representa uma operação de impressão universal de longa duração. Classe base para tipos de operação como printerCreateOperation.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 55bf24e75f79a66d9691b14ebac1073c43f15a4e
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60942503"
---
# <a name="printoperation-resource-type"></a>Tipo de recurso printOperation

Namespace: microsoft.graph

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

