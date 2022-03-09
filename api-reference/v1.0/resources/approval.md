---
title: tipo de recurso de aprovação
description: O objeto de aprovação associado a um userConsentRequest ou a accessPackageAssignmentRequest.
author: psignoret
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 812c2315593abdc0556fcf2a5f2d545299999fc1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395857"
---
# <a name="approval-resource-type"></a>tipo de recurso de aprovação

Namespace: microsoft.graph

Representa o objeto de aprovação para decisões associadas a uma solicitação.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter aprovação](../api/approval-get.md) | [aprovação](approval.md) | Recupere as propriedades de um **objeto de** aprovação no gerenciamento de direitos. |
|[filterByCurrentUser](../api/approval-filterbycurrentuser.md)| [coleção approval](approval.md)| Recupere os **objetos de** aprovação de um aprovador no gerenciamento de direitos.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador da decisão de aprovação.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|Estágios|[coleção approvalStage](../resources/approvalstage.md)|Uma coleção de estágios na decisão de aprovação. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approval",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.approval",
  "id": "String (identifier)",
  "stages": [{
        "@odata.type": "#microsoft.graph.approvalStage"
    }]
}
```
