---
title: Tipo de recurso excludeTarget
description: Representa os usuários ou grupos de usuários excluídos de uma política.
author: mjsantani
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 368d6446d9dbead0ccacfb5538c3433050b6c79c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61034401"
---
# <a name="excludetarget-resource-type"></a>Tipo de recurso excludeTarget

Namespace: microsoft.graph

Representa os usuários ou grupos de usuários excluídos de uma política.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador de objeto de um Azure Active Directory usuário ou grupo.|
|targetType|authenticationMethodTargetType|O tipo de destino do método de autenticação. Os valores possíveis são: `user`, `group`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludeTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludeTarget",
  "id": "String (identifier)",
  "targetType": "String"
}
```
