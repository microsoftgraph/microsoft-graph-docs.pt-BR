---
title: tipo de recurso workbookRangeFormat
description: Um objeto de formato que encapsula a fonte, o preenchimento, as bordas, o alinhamento e outras propriedades do intervalo.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 08d1b0fa13e1b615912433b8fda378b89bf9f926
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046192"
---
# <a name="workbookrangeformat-resource-type"></a>tipo de recurso workbookRangeFormat

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um objeto de formato que encapsula a fonte, o preenchimento, as bordas, o alinhamento e outras propriedades do intervalo.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter workbookRangeFormat](../api/rangeformat-get.md) | [workbookRangeFormat](workbookrangeformat.md) |Leia as propriedades e relacionamentos do objeto rangeFormat.|
|[Criar workbookRangeBorder](../api/rangeformat-post-borders.md) |[workbookRangeBorder](workbookrangeborder.md)| Crie uma nova RangeBorder postando na coleção de bordas.|
|[List borders](../api/rangeformat-list-borders.md) |coleção [workbookRangeBorder](workbookrangeborder.md)| Obtenha uma coleção de objetos RangeBorder.|
|[Update](../api/rangeformat-update.md) | [workbookRangeFormat](workbookrangeformat.md) |Atualize o objeto RangeFormat. |
|[Autofitcolumns](../api/rangeformat-autofitcolumns.md)|Nenhum|Altera a largura das colunas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.|
|[Autofitrows](../api/rangeformat-autofitrows.md)|Nenhum|Altera a altura das linhas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|columnWidth|duplo|Obtém ou define a largura de todas as colunas dentro do intervalo. Se as larguras das colunas não forem uniformes, será retornado null.|
|horizontalAlignment|string|Representa o alinhamento horizontal do objeto especificado. Os valores possíveis são: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection` e `Distributed`.|
|rowHeight|duplo|Obtém ou define a altura de todas as linhas do intervalo. Se as alturas das linhas não forem uniformes, será retornado null.|
|verticalAlignment|string|Representa o alinhamento vertical do objeto especificado. Os valores possíveis são: `Top`, `Center`, `Bottom`, `Justify` e `Distributed`.|
|wrapText|booliano|Indica se o Excel quebra automaticamente a linha de texto no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de quebra de linha automática uniforme.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Borders|coleção [workbookRangeBorder](workbookrangeborder.md)|Coleção de objetos de borda que se aplicam a todo o intervalo selecionado. Somente leitura.|
|fill|[workbookRangeFill](workbookrangefill.md)|Retorna o objeto de preenchimento definido em todo o intervalo. Somente leitura.|
|font|[workbookRangeFont](workbookrangefont.md)|Retorna o objeto Font definido em todo o intervalo selecionado. Somente leitura.|
|protection|[formatProtection](formatprotection.md)|Retorna o objeto de proteção de formato para um intervalo. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFormat"
}-->

```json
{
  "columnWidth": 1024,
  "horizontalAlignment": "string",
  "rowHeight": 1024,
  "verticalAlignment": "string",
  "wrapText": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


