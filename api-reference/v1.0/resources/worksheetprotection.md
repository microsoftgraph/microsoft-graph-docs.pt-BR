---
title: Tipo de recurso WorksheetProtection
description: Representa a proteção de um objeto de planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c8a719d1be9f21edf1bef82d2aa058b45bbf2df8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984231"
---
# <a name="worksheetprotection-resource-type"></a>Tipo de recurso WorksheetProtection

Representa a proteção de um objeto de planilha.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get WorksheetProtection](../api/worksheetprotection-get.md) | [WorkbookWorksheetProtection](worksheetprotection.md) |Leia as propriedades e os relacionamentos do objeto worksheetProtection.|
|[Protect](../api/worksheetprotection-protect.md)|Nenhum|Protege uma planilha. Gera uma exceção se a planilha estiver protegida.|
|[Unprotect](../api/worksheetprotection-unprotect.md)|Nenhum|Desprotege uma planilha.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|options|[WorkbookWorksheetProtectionOptions](worksheetprotectionoptions.md)|Opções de proteção da planilha. Somente leitura.|
|protected|booliano|Indica se a planilha está protegida.  Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": true,
  "options": { "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
