---
title: tipo de recurso workbookOperationError
description: Representa um erro de uma operação de workbook com falha.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: df629e7fce25638dce64dbec6914026a36c42e8b88f98d7348832eb040afb87f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235244"
---
# <a name="workbookoperationerror-resource-type"></a>tipo de recurso workbookOperationError

Representa um erro de uma operação de workbook com falha.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|código|Cadeia de caracteres| O código de erro.|
|mensagem|String| A mensagem de erro.|
|innererror|error object| Opcional. Objetos error adicionais que podem ser mais específicos do que o erro de nível superior.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookOperationError",
  "baseType": null
}-->

```json
{
  "code": "String",
  "message": "String",
  "innererror": { "@odata.type": "odata.error" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

