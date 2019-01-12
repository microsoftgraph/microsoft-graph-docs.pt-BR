---
title: Tipo de recurso RangeFormat
description: Um objeto de formatação que engloba a fonte, o preenchimento, as bordas, o alinhamento e outras propriedades do intervalo.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: b4018995e37ff40ae014b54d08b77bbed73d6fe2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937345"
---
# <a name="rangeformat-resource-type"></a>Tipo de recurso RangeFormat

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Um objeto de formatação que engloba a fonte, o preenchimento, as bordas, o alinhamento e outras propriedades do intervalo.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get RangeFormat](../api/rangeformat-get.md) | [RangeFormat](rangeformat.md) |Leia as propriedades e relacionamentos do objeto rangeFormat.|
|[Create RangeBorder](../api/rangeformat-post-borders.md) |[RangeBorder](rangeborder.md)| Crie uma nova RangeBorder postando na coleção de bordas.|
|[List borders](../api/rangeformat-list-borders.md) |Coleção [RangeBorder](rangeborder.md)| Obtenha uma coleção de objetos RangeBorder.|
|[Update](../api/rangeformat-update.md) | [RangeFormat](rangeformat.md) |Atualize o objeto RangeFormat. |
|[Autofitcolumns](../api/rangeformat-autofitcolumns.md)|Nenhum|Altera a largura das colunas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.|
|[Autofitrows](../api/rangeformat-autofitrows.md)|Nenhum|Altera a altura das linhas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|columnWidth|double|Obtém ou define a largura de todas as colunas dentro do intervalo. Se as larguras das colunas não forem uniformes, será retornado null.|
|horizontalAlignment|string|Representa o alinhamento horizontal do objeto especificado. Os valores possíveis são: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection` e `Distributed`.|
|rowHeight|double|Obtém ou define a altura de todas as linhas do intervalo. Se as alturas das linhas não forem uniformes, será retornado null.|
|verticalAlignment|string|Representa o alinhamento vertical do objeto especificado. Os valores possíveis são: `Top`, `Center`, `Bottom`, `Justify` e `Distributed`.|
|wrapText|booliano|Indica se o Excel quebra automaticamente a linha de texto no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de quebra de linha automática uniforme.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|borders|Coleção [RangeBorder](rangeborder.md)|Coleção de objetos de borda que se aplicam a todo o intervalo selecionado. Somente leitura.|
|fill|[RangeFill](rangefill.md)|Retorna o objeto de preenchimento definido em todo o intervalo. Somente leitura.|
|font|[RangeFont](rangefont.md)|Retorna o objeto Font definido em todo o intervalo selecionado. Somente leitura.|
|protection|[FormatProtection](formatprotection.md)|Retorna o objeto de proteção de formato para um intervalo. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFormat"
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
