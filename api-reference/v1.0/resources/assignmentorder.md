---
title: Tipo de recurso assignmentOrder
description: Define a ordem dos atributos que estão sendo coletados em um fluxo de usuários.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2b4b4519aab605978f7afba1d538d3c7007b3599
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123780"
---
# <a name="assignmentorder-resource-type"></a>Tipo de recurso assignmentOrder

Namespace: microsoft.graph

Usado para definir a ordem dos atributos que estão sendo coletados em um fluxo de usuário. A ordem determina como a página do conjunto de atributos é exibida quando um usuário se insissura usando um fluxo de usuário.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|order|Coleção String|Uma lista de identificadores de objeto identityUserFlowAttribute que determinam a ordem na qual os atributos devem ser coletados em um fluxo de usuário.|

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
