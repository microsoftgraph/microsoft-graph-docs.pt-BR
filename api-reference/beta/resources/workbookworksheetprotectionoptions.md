---
title: tipo de recurso workbookWorksheetProtectionOptions
description: Representa as opções de proteção da planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c5f5a953490eebf456ce4cc37b515c758630b3ce
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348476"
---
# <a name="workbookworksheetprotectionoptions-resource-type"></a>tipo de recurso workbookWorksheetProtectionOptions

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
<!--
{
  "type": "#page.annotation",
  "description": "workbookWorksheetProtectionOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
