---
title: Tipo de recurso messageRule
description: Uma regra que se aplica a mensagens na Caixa de Entrada de um usuário.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6147640a221b72716f20bf4a90e74e25a7f9a448
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133760"
---
# <a name="messagerule-resource-type"></a>Tipo de recurso messageRule

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma regra que se aplica a mensagens na Caixa de Entrada de um usuário.

No Outlook, é possível configurar regras para mensagens recebidas na Caixa de Entrada, para realizar ações específicas em determinadas condições. 

Programaticamente, você pode acessar regras por meio da propriedade de navegação **messageRules** da [pasta](mailfolder.md) Caixa de Entrada. Cada regra é representada por esse recurso **messageRule**, as ações de regra disponíveis são representadas pelo tipo complexo [messageRuleActions](messageruleactions.md) e as condições e exceções de regra disponíveis são representadas pelo tipo complexo [messageRulePredicates](messagerulepredicates.md).


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| actions | [messageRuleActions](messageruleactions.md) | Ações a serem realizadas em uma mensagem quando as condições correspondentes forem atendidas. |
| conditions | [messageRulePredicates](messagerulepredicates.md) | Condições que, quando atendidas, acionarão as ações correspondentes dessa regra. |
| displayName | String | O nome de exibição da regra. |
| exceptions | [messageRulePredicates](messagerulepredicates.md) | Condições de exceção para a regra. |
| hasError | Boolean | Indica se a regra está em uma condição de erro. Somente leitura. |
| id |String|O identificador exclusivo da regra. Somente leitura.|
| isEnabled | Booliano | Indica se a regra está habilitada para ser aplicada a mensagens. |
| isReadOnly | Boolean | Indica se a regra é somente leitura e não pode ser modificada ou excluída pelas regras da API REST. |
| sequence | Int32 | Indica a ordem em que a regra é executada, entre outras regras. |


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRule"
}-->

```json
{
  "actions": {"@odata.type": "microsoft.graph.messageRuleActions"},
  "conditions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "displayName": "String",
  "exceptions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "hasError": "Boolean",
  "id": "String",
  "isEnabled": "Boolean",
  "isReadOnly": "Boolean",
  "sequence": "Int32"
}

```

## <a name="methods"></a>Métodos
| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar regras](../api/mailfolder-list-messagerules.md) | Coleção [messageRule](messagerule.md) |Obtenha todos os objetos **messageRule** definidos para a Caixa de Entrada do usuário.|
|[Obter regra](../api/messagerule-get.md) | [messageRule](messagerule.md) |Leia as propriedades e as relações de um objeto **messageRule**.|
|[Criar](../api/mailfolder-post-messagerules.md) | [messageRule](messagerule.md) |Crie um objeto **messageRule** especificando um conjunto de condições e ações.|
|[Atualizar](../api/messagerule-update.md) | [messageRule](messagerule.md) |Altere as propriedades graváveis em um objeto **messageRule** e salve as alterações. |
|[Delete](../api/messagerule-delete.md) | Nenhuma |Exclua o objeto **messageRule** especificado. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


