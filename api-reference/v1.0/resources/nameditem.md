---
title: Tipo de recurso NamedItem
description: Representa um nome definido para um intervalo de células ou um valor. Os nomes podem ser objetos nomeados primitivos (conforme exibido no tipo abaixo), objetos de intervalo ou uma referência a um intervalo. Use esse objeto para obter um objeto de intervalo associado aos nomes.
ms.openlocfilehash: 683bc93fdd9c14005b70cb125cf09eba5c8075a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007418"
---
# <a name="nameditem-resource-type"></a>Tipo de recurso NamedItem

Representa um nome definido para um intervalo de células ou um valor. Os nomes podem ser objetos nomeados primitivos (conforme exibido no tipo abaixo), objetos de intervalo ou uma referência a um intervalo. Use esse objeto para obter um objeto de intervalo associado aos nomes.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Add](../api/nameditem-add.md)|[WorkbookNamedItem](nameditem.md)|Adiciona um novo nome à coleção do escopo fornecido.|
|[AddFormulaLocal](../api/nameditem-addformulalocal.md)|[WorkbookNamedItem](nameditem.md)|Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.|
|[Get NamedItem](../api/nameditem-get.md) | [WorkbookNamedItem](nameditem.md) |Leia as propriedades e os relacionamentos do objeto namedItem.|
|[Update](../api/nameditem-update.md) | [WorkbookNamedItem](nameditem.md)   |Atualize o objeto NamedItem. |
|[Range](../api/nameditem-range.md)|[Range](range.md)|Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.|
|[List](../api/nameditem-list.md) | Coleção [WorkbookNamedItem](nameditem.md) |Obtenha uma coleção de objetos namedItem. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|name|string|O nome do objeto. Somente leitura.|
|comment|string|Representa o comentário associado a esse nome.|
|scope|string|Indica se o nome tem escopo para a pasta de trabalho ou uma planilha específica. Somente leitura.|
|type|string|Indica o tipo de referência é associado ao nome. Os valores possíveis são: `String`, `Integer`, `Double`, `Boolean`, `Range`. Somente leitura.|
|valor|Json|Representa a fórmula à qual o nome está definido para fazer referência. Por exemplo, =Plan14!$B$2:$H$12, =4,75, etc. Somente leitura.|
|visible|booliano|Determina se o objeto fica visível ou não.|

## <a name="relationships"></a>Relações
| Relação     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|planilha|[WorkbookWorksheet](worksheet.md)|Retorna a planilha em que o item nomeado está no escopo. Disponível somente se o item estiver com escopo de planilha. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookNamedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": {"@odata.type": "microsoft.graph.Json"},
  "visible": true
  
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
