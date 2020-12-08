---
title: tipo de recurso assignmentOrder
description: Usado para definir a ordem dos atributos que estão sendo coletados dentro de um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 41b75e1adf5459279b5675278a8f00a82110b457
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581274"
---
# <a name="assignmentorder-resource-type"></a>tipo de recurso assignmentOrder

Namespace: Microsoft Graph

Usado para definir a ordem dos atributos que estão sendo coletados dentro de um fluxo de usuário. Isso determina como a página de coleção de atributos é exibida quando um usuário se inscreve por meio de um fluxo de usuário.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Ordene|Conjunto de cadeias de caracteres|Uma lista de IDs de identityUserFlowAttribute fornecidos para determinar a ordem na qual os atributos devem ser coletados dentro de um fluxo de usuário.|

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
