---
title: Tipo de recurso WorksheetProtection
description: Representa a proteção de um objeto de planilha.
author: lumine2008
ms.openlocfilehash: 91415b067fbe54333e32d1a2ed84bce5025b7d3a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339204"
---
# <a name="worksheetprotection-resource-type"></a>Tipo de recurso WorksheetProtection

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa a proteção de um objeto de planilha.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get WorksheetProtection](../api/worksheetprotection-get.md) | [WorksheetProtection](worksheetprotection.md) |Leia as propriedades e os relacionamentos do objeto worksheetProtection.|
|[Protect](../api/worksheetprotection-protect.md)|Nenhum|Protege uma planilha. Gera uma exceção se a planilha estiver protegida.|
|[Unprotect](../api/worksheetprotection-unprotect.md)|Nenhum|Desprotege uma planilha.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|protected|booliano|Indica se a planilha está protegida.  Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|options|[WorksheetProtectionOptions](worksheetprotectionoptions.md)|Opções de proteção da planilha. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheetProtection"
}-->

```json
{
  "protected": true
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