---
title: Tipo de recurso assignmentOrder
description: Usado para definir a ordem dos atributos que estão sendo coletados em um fluxo de usuário.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: afc59c24e154e8349eacff0d4059f1b102d8bc19
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033830"
---
# <a name="assignmentorder-resource-type"></a>Tipo de recurso assignmentOrder

Namespace: microsoft.graph

Usado para definir a ordem dos atributos que estão sendo coletados em um fluxo de usuário. THis determina como a página do conjunto de atributos é exibida quando um usuário se ins inscrever por meio de um fluxo de usuário.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|order|String collection|Uma lista de IDs identityUserFlowAttribute fornecidas para determinar a ordem na qual os atributos devem ser coletados em um fluxo de usuário.|

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
