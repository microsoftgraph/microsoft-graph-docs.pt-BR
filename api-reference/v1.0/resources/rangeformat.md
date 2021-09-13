---
title: Tipo de recurso RangeFormat
description: Um objeto de formato que encapsula a fonte, o preenchimento, as bordas, o alinhamento e outras propriedades do intervalo.
ms.localizationpriority: medium
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: cdcea1e15c70bcdef2d56d8f73b56937903160ab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143689"
---
# <a name="rangeformat-resource-type"></a>Tipo de recurso RangeFormat

Namespace: microsoft.graph

Um objeto de formato que encapsula a fonte, o preenchimento, as bordas, o alinhamento e outras propriedades do intervalo.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get RangeFormat](../api/rangeformat-get.md) | [WorkbookRangeFormat](rangeformat.md) |Leia as propriedades e relacionamentos do objeto rangeFormat.|
|[Create RangeBorder](../api/rangeformat-post-borders.md) |[WorkbookRangeBorder](rangeborder.md)| Crie uma nova RangeBorder postando na coleção de bordas.|
|[List borders](../api/rangeformat-list-borders.md) |[Coleção WorkbookRangeBorder](rangeborder.md)| Obtenha uma coleção de objetos RangeBorder.|
|[Update](../api/rangeformat-update.md) | [WorkbookRangeFormat](rangeformat.md) |Atualize o objeto RangeFormat. |
|[Autofitcolumns](../api/rangeformat-autofitcolumns.md)|Nenhum|Altera a largura das colunas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.|
|[Autofitrows](../api/rangeformat-autofitrows.md)|Nenhum|Altera a altura das linhas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|columnWidth|duplo|Obtém ou define a largura de todas as colunas dentro do intervalo. Se as larguras das colunas não forem uniformes, será retornado null.|
|horizontalAlignment|string|Representa o alinhamento horizontal do objeto especificado. Os valores possíveis são: `General` , , , , , , , , `Left` `Center` `Right` `Fill` `Justify` `CenterAcrossSelection` `Distributed` .|
|rowHeight|duplo|Obtém ou define a altura de todas as linhas do intervalo. Se as alturas das linhas não forem uniformes, será retornado null.|
|verticalAlignment|string|Representa o alinhamento vertical do objeto especificado. Os valores possíveis são: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.|
|wrapText|booliano|Indica se o Excel quebra automaticamente a linha de texto no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de quebra de linha automática uniforme.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Borders|[Coleção WorkbookRangeBorder](rangeborder.md)|Coleção de objetos de borda que se aplicam a todo o intervalo selecionado. Somente leitura.|
|fill|[WorkbookRangeFill](rangefill.md)|Retorna o objeto de preenchimento definido em todo o intervalo. Somente leitura.|
|font|[WorkbookRangeFont](rangefont.md)|Retorna o objeto Font definido em todo o intervalo selecionado. Somente leitura.|
|protection|[WorkbookFormatProtection](formatprotection.md)|Retorna o objeto de proteção de formato para um intervalo. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

