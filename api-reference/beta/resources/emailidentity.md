---
title: Tipo de recurso emailIdentity
description: Representar a identidade de email de um usuário.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 90882a78c149e089fd00baa266240cb574e9864a
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979475"
---
# <a name="emailidentity-resource-type"></a>Tipo de recurso emailIdentity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representar a identidade de email de um usuário.


Herda da [identidade](../resources/identity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome de exibição do usuário. Herdado da [identidade](../resources/identity.md).|
|email|Cadeia de caracteres|Endereço de email do usuário.|
|id|String|ID do usuário. Herdado da [identidade](../resources/identity.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "email": "String"
}
```

