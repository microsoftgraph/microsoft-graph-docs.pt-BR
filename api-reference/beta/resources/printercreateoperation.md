---
title: tipo de recurso printerCreateOperation
description: Representa uma operação de registro de impressora de longa execução. Derivado de reoperation.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 54f458e14cbda209d9c2d85f08df4c106db6ab00
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007159"
---
# <a name="printercreateoperation-resource-type"></a>tipo de recurso printerCreateOperation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma operação de registro de impressora de longa execução. Derivado de [Reoperation](printoperation.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Operação get](../api/printoperation-get.md) | [Operação de reoperação](printoperation.md) | Recupere uma operação de execução longa dentro do usuário atual ou do locatário do aplicativo. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O identificador da operação. Somente leitura.|
|status|[printOperationStatus](printoperationstatus.md)|O status da operação de registro. Contém o andamento da operação e se ela foi concluída com êxito. Somente leitura.|
|createdDateTime|DateTimeOffset|O DateTimeOffset quando a operação foi criada. Somente leitura.|
|certificado|Cadeia de caracteres|O certificado assinado criado durante o processo de registro. Somente leitura.|
|impressora|[impressora](printer.md)|A entidade de impressora criada. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerCreateOperation",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
    "id": "String (identifier)",
    "status": {"@odata.type": "microsoft.graph.printOperationStatus"},
    "createdDateTime": "2020-06-15T19:54:14.853Z",
    "certificate": "",
    "printer": {"@odata.type": "microsoft.graph.printer"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerCreateOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->