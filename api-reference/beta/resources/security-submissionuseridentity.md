---
title: Tipo de recurso submissionUserIdentity
description: Representa a identidade do usuário que envia o envio de ameaças.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: c6f0fbd5c5f413200f358044a0bd202c0e4c031a
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856504"
---
# <a name="submissionuseridentity-resource-type"></a>Tipo de recurso submissionUserIdentity

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a identidade do usuário que envia o envio de ameaças.

Herda da [identidade](../resources/identity.md).

## <a name="properties"></a>Propriedades
| Propriedade    | Tipo   | Descrição                                                                                                    |
|:------------|:-------|:---------------------------------------------------------------------------------------------------------------|
| displayName | String | Herdado da **identidade**.                                                                 |
| email       | Cadeia de caracteres | O email do usuário que está fazendo o envio quando conectado (caso de token delegado). | 
| id          | String | Herdado da **identidade**.  |


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.submissionUserIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.submissionUserIdentity",
  "displayName": "String",
  "id": "String (identifier)",
  "email": "String"
}
```

