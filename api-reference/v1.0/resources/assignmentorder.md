---
title: Tipo de recurso assignmentOrder
description: Define a ordem dos atributos que estão sendo coletados em um fluxo de usuários.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4c5faed250c07d5c4416c91a5452f1276c6b728e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882765"
---
# <a name="assignmentorder-resource-type"></a>Tipo de recurso assignmentOrder

Namespace: microsoft.graph

Usado para definir a ordem dos atributos que estão sendo coletados em um fluxo de usuário. A ordem determina como a página do conjunto de atributos é exibida quando um usuário se insissura usando um fluxo de usuário.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|order|Coleção de cadeias de caracteres|Uma lista de identificadores de objeto identityUserFlowAttribute que determinam a ordem na qual os atributos devem ser coletados em um fluxo de usuário.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentOrder"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.assignmentOrder",
  "order": [
    "String"
  ]
}
```
