---
title: Tipo de recurso assignmentOrder
description: Usado para definir a ordem dos atributos que estão sendo coletados em um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7d7716cb4b13917aad33cd88afeb364a2891e3df
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761237"
---
# <a name="assignmentorder-resource-type"></a>Tipo de recurso assignmentOrder

Namespace: microsoft.graph

Usado para definir a ordem dos atributos que estão sendo coletados em um fluxo de usuário. THis determina como a página do conjunto de atributos é exibida quando um usuário se ins inscrever por meio de um fluxo de usuário.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|order|Coleção de cadeias de caracteres|Uma lista de IDs identityUserFlowAttribute fornecidas para determinar a ordem na qual os atributos devem ser coletados em um fluxo de usuário.|

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
