---
title: tipo de recurso workbookApplication
description: Representa o aplicativo Excel que gerencia a pasta de trabalho.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a8cb375493b018d2d6f277f2cbc7944e9d662f018e301eec551bd3b5ab648368
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251691"
---
# <a name="workbookapplication-resource-type"></a>tipo de recurso workbookApplication

Namespace: microsoft.graph

Representa o aplicativo Excel que gerencia a pasta de trabalho.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter workbookApplication](../api/workbookapplication-get.md) | [workbookApplication](workbookapplication.md) |Ler propriedades e relações do objeto workbookApplication.|
|[Calculate](../api/workbookapplication-calculate.md)|None|Recalcula todas as pastas de trabalho abertas no Excel no momento.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|calculationMode|string|Retorna o modo de cálculo usado na pasta de trabalho. Os valores possíveis são: `Automatic`, `AutomaticExceptTables`, `Manual`.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookApplication"
}-->

```json
{
  "calculationMode": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

