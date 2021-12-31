---
title: Tipo de recurso authenticationStrength
description: A força de autenticação personalizada imposta em uma política de Acesso Condicional
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a316d3d6f575183fcb59647355545746838b0cdf
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647199"
---
# <a name="authenticationstrength-resource-type"></a>Tipo de recurso authenticationStrength

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A força de autenticação personalizada imposta em uma política de Acesso Condicional. 

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|authenticationStrengthId|String|Identificador da força de autenticação.|
|displayName|String|O nome da força de autenticação.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationStrength"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationStrength",
  "authenticationStrengthId": "String",
  "displayName": "String"
}
```

