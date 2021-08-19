---
title: Tipo de recurso assignmentOrder
description: Usado para definir a ordem dos atributos que estão sendo coletados em um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 61114b2a4fa39485843a8e1b722c518def0301ae380334f09ca79e088941040d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54245321"
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
