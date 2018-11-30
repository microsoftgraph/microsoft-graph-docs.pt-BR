---
title: Tipo de recurso TableSort
description: Gerencia operações de classificação em objetos Table.
ms.openlocfilehash: 02ee1f72bc53a3097c76cf9bab62a165fe3c56f8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041060"
---
# <a name="tablesort-resource-type"></a>Tipo de recurso TableSort

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Gerencia operações de classificação em objetos Table.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get TableSort](../api/tablesort-get.md) | [TableSort](tablesort.md) |Leia as propriedades e os relacionamentos do objeto tableSort.|
|[Aplicar](../api/tablesort-apply.md)|Nenhum|Execute uma operação de classificação.|
|[Clear](../api/tablesort-clear.md)|Nenhum|Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.|
|[Reapply](../api/tablesort-reapply.md)|Nenhum|Reaplica os parâmetros de classificação atuais à tabela.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|matchCase|booliano|Indica se o uso de maiúsculas ou minúsculas afetou a última classificação da tabela. Somente leitura.|
|method|string|Indica o último método de ordenação de caracteres chineses usado para classificar a tabela. Os valores possíveis são: `PinYin` e `StrokeCount`. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|campos|[SortField](sortfield.md)|Representa as condições atuais usadas para a última classificação da tabela. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->