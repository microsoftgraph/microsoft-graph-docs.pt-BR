---
title: Tipo de recurso printerCreateOperation
description: Representa uma operação de registro de impressora de longa duração. Derivado de printOperation.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 91a1d70afccf94abe1c611e696bc4349a59964e1dbb176cce0ddb8aa32dc287a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54169351"
---
# <a name="printercreateoperation-resource-type"></a>Tipo de recurso printerCreateOperation

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Representa uma operação de registro de impressora de longa duração. Derivado de [printOperation](printoperation.md).

Herda de [printOperation](printoperation.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [Obter operação](../api/printoperation-get.md) | [printOperation](printoperation.md) | Recupere uma operação de longa duração dentro do usuário atual ou do locatário do aplicativo. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador da operação. Somente leitura.|
|status|[printOperationStatus](printoperationstatus.md)|O status da operação de registro. Contém o progresso da operação e se ela foi concluída com êxito. Somente leitura.|
|createdDateTime|DateTimeOffset|DateTimeOffset quando a operação foi criada. Somente leitura.|
|certificado|Cadeia de caracteres|O certificado assinado criado durante o processo de registro. Somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|impressora|[impressora](printer.md)|A entidade de impressora criada. Somente leitura.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printerCreateOperation",
  "baseType": "microsoft.graph.printOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerCreateOperation",
  "id": "String (identifier)",
  "status": {
    "@odata.type": "microsoft.graph.printOperationStatus"
  },
  "createdDateTime": "String (timestamp)",
  "certificate": "String"
}
```

