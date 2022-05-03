---
title: Tipo de recurso printerCreateOperation
description: Representa uma operação de registro de impressora de execução longa. Derivado de printOperation.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 716c23603dd811ddad61dd604c9961d1df3f5297
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176530"
---
# <a name="printercreateoperation-resource-type"></a>Tipo de recurso printerCreateOperation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma operação de registro de impressora de execução longa. Derivado de [printOperation](printoperation.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter operação](../api/printoperation-get.md) | [printOperation](printoperation.md) | Recupere uma operação de execução longa dentro do locatário do usuário ou do aplicativo atual. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|O identificador da operação. Somente leitura.|
|status|[printOperationStatus](printoperationstatus.md)|O status da operação de registro. Contém o progresso da operação e se ela foi concluída com êxito. Somente leitura.|
|createdDateTime|DateTimeOffset|O DateTimeOffset quando a operação foi criada. Somente leitura.|
|certificado|Cadeia de caracteres|O certificado assinado criado durante o processo de registro. Somente leitura.|
|Impressora|[impressora](printer.md)|A entidade de impressora criada. Somente leitura.|

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

