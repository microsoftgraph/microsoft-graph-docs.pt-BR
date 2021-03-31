---
title: authenticationMethodConfigurations
description: objeto authenticationMethodConfigurations.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 26d0cd948a69968a7d45b3406b3da7109ffc3f18
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469126"
---
# <a name="authenticationmethodconfiguration-resource-type"></a>tipo de recurso authenticationMethodConfiguration
Namespace: microsoft.graph

Representa uma política de método de autenticação.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O nome da política.|
|state|authenticationMethodState|O estado da política. Os valores possíveis são: `enabled`, `disabled`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```
