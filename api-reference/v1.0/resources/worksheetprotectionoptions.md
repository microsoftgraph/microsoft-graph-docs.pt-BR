---
title: Tipo de recurso WorksheetProtectionOptions
description: Representa as opções de proteção da planilha.
ms.openlocfilehash: ef086b911a154df2eddf92ee57b89d570ef12247
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007111"
---
# <a name="worksheetprotectionoptions-resource-type"></a>Tipo de recurso WorksheetProtectionOptions

Representa as opções de proteção da planilha.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowAutoFilter|booliano|Indica a opção de proteção de planilha para permitir a utilização do recurso de filtro automático.|
|allowDeleteColumns|booliano|Indica a opção de proteção de planilha para permitir a exclusão de colunas.|
|allowDeleteRows|booliano|Indica a opção de proteção de planilha para permitir a exclusão de linhas.|
|allowFormatCells|booliano|Indica a opção de proteção de planilha para permitir a formatação de células.|
|allowFormatColumns|booliano|Indica a opção de proteção de planilha para permitir a formatação de colunas.|
|allowFormatRows|booliano|Indica a opção de proteção de planilha para permitir a formatação de linhas.|
|allowInsertColumns|booliano|Indica a opção de proteção de planilha para permitir a inserção de colunas.|
|allowInsertHyperlinks|booliano|Indica a opção de proteção de planilha para permitir a inserção de hiperlinks.|
|allowInsertRows|booliano|Indica a opção de proteção de planilha para permitir a inserção de linhas.|
|allowPivotTables|booliano|Indica a opção de proteção de planilha para permitir a utilização do recurso de tabela dinâmica.|
|allowSort|booliano|Indica a opção de proteção de planilha para permitir a utilização do recurso de classificação.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions"
}-->

```json
{
  "allowAutoFilter": true,
  "allowDeleteColumns": true,
  "allowDeleteRows": true,
  "allowFormatCells": true,
  "allowFormatColumns": true,
  "allowFormatRows": true,
  "allowInsertColumns": true,
  "allowInsertHyperlinks": true,
  "allowInsertRows": true,
  "allowPivotTables": true,
  "allowSort": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtectionOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->