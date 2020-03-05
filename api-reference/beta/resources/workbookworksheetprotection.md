---
title: tipo de recurso workbookWorksheetProtection
description: Representa a proteção de um objeto sheet.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ab5d3101b1b9cabf8843d3726f036de74bf3a258
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519096"
---
# <a name="workbookworksheetprotection-resource-type"></a>tipo de recurso workbookWorksheetProtection

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a proteção de um objeto sheet.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter workbookWorksheetProtection](../api/worksheetprotection-get.md) | [workbookWorksheetProtection](workbookworksheetprotection.md) |Leia as propriedades e os relacionamentos do objeto workbookWorksheetProtection.|
|[Protect](../api/worksheetprotection-protect.md)|Nenhum|Protege uma planilha. Gera uma exceção se a planilha estiver protegida.|
|[Unprotect](../api/worksheetprotection-unprotect.md)|Nenhum|Desprotege uma planilha.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|options|[workbookWorksheetProtectionOptions](workbookworksheetprotectionoptions.md)|Opções de proteção da planilha. Somente leitura.|
|protected|booliano|Indica se a planilha está protegida.  Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "options"
  ],
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": "boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookWorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
