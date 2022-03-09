---
title: Tipo de recurso approvalStage
description: O objeto approvalStage associado a um userConsentRequest ou a uma solicitação de atribuição de pacote de acesso.
author: psignoret
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2cd51e18cd3d641018c5f0792754cec129392aa6
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395850"
---
# <a name="approvalstage-resource-type"></a>Tipo de recurso approvalStage

Namespace: microsoft.graph

Especifica um estágio de decisão em uma [aprovação](approval.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Aprovação de listaStages](../api/approval-list-stages.md) | [coleção approvalStage](approvalstage.md) | Listar **os objetos approvalStage** associados a um objeto **de** aprovação no gerenciamento de direitos. |
|[Obter approvalStage](../api/approvalstage-get.md) | [approvalStage](approvalstage.md) | Recupere as propriedades de um **objeto approvalStage** no gerenciamento de direitos. |
|[Atualizar approvalStage](../api/approvalstage-update.md) | Nenhum | Aplicar a decisão aprovar ou negar um **objeto approvalStage** no gerenciamento de direitos. |

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|assignedToMe|Booliano|Indica se o estágio é atribuído ao usuário chamador para revisar. Somente leitura.|
|displayName|Cadeia de caracteres|O rótulo fornecido pelo criador da política para identificar um estágio de aprovação. Somente leitura.|
|id|Cadeia de caracteres|O identificador do estágio associado a um objeto de aprovação. Somente leitura.|
|justification|Cadeia de caracteres|A justificativa associada à decisão do estágio de aprovação.|
|reviewResult|Cadeia de caracteres|O resultado desse registro de aprovação. Os valores possíveis incluem: `NotReviewed`, `Approved`, . `Denied`|
|reviewedBy|[identity](identity.md) | O identificador do revistor. Somente leitura.|
|reviewedDateTime|DateTimeOffset|A data e a hora em que uma decisão foi registrada. As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|status|Cadeia de caracteres|O status do estágio. Valores possíveis: `InProgress`, `Initializing`, `Completed`, `Expired`. Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approvalStage",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.approvalStage",
  "id": "String (identifier)",
  "displayName": "String",
  "status": "String",
  "assignedToMe": "Boolean",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.identity"
  },
  "reviewedDateTime": "String (timestamp)",
  "reviewResult": "String",
  "justification": "String"
}
```
