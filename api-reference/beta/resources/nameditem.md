---
title: Tipo de recurso NamedItem
description: Representa um nome definido para um intervalo de células ou um valor. Os nomes podem ser objetos nomeados primitivos (conforme exibido no tipo abaixo), objetos de intervalo ou uma referência a um intervalo. Use esse objeto para obter um objeto de intervalo associado aos nomes.
localization_priority: Normal
ms.openlocfilehash: 5dd093976b2c09ae93c608144c8d6c2b7d7161c2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581496"
---
# <a name="nameditem-resource-type"></a>Tipo de recurso NamedItem

Representa um nome definido para um intervalo de células ou um valor. Os nomes podem ser objetos nomeados primitivos (conforme exibido no tipo abaixo), objetos de intervalo ou uma referência a um intervalo. Use esse objeto para obter um objeto de intervalo associado aos nomes.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Add](../api/nameditem-add.md)|[NamedItem](nameditem.md)|Adiciona um novo nome à coleção do escopo fornecido.|
|[AddFormulaLocal](../api/nameditem-addformulalocal.md)|[NamedItem](nameditem.md)|Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.|
|[Get NamedItem](../api/nameditem-get.md) | [NamedItem](nameditem.md) |Leia as propriedades e os relacionamentos do objeto namedItem.|
|[Update](../api/nameditem-update.md) | [NamedItem](nameditem.md)   |Atualize o objeto NamedItem. |
|[Range](../api/nameditem-range.md)|[Range](range.md)|Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.|
|[List](../api/nameditem-list.md) | Coleção [NamedItem](nameditem.md) |Obtenha uma coleção de objetos namedItem. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|name|string|O nome do objeto. Somente leitura.|
|comment|cadeia de caracteres|Representa o comentário associado a esse nome.|
|scope|string|Indica se o nome tem escopo para a pasta de trabalho ou uma planilha específica. Somente leitura.|
|type|string|Indica o tipo de referência associado ao nome. Os valores possíveis são: `String`, `Integer`, `Double`, `Boolean` e `Range`. Somente leitura.|
|value|string|Representa a fórmula à qual o nome está definido para fazer referência. Por exemplo, =Plan14!$B$2:$H$12, =4,75, etc. Somente leitura.|
|visible|booliano|Determina se o objeto fica visível ou não.|

## <a name="relationships"></a>Relações
| Relação     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|planilha|[worksheet](worksheet.md)|Retorna a planilha em que o item nomeado está no escopo. Disponível somente se o item estiver com escopo de planilha. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": "string",
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
