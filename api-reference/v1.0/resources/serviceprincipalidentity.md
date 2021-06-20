---
title: Tipo de recurso servicePrincipalIdentity
description: Modela uma identidade de entidade de serviço.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 231a0d9dc811569de23412d6ad76a2ba35f6c58b
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031023"
---
# <a name="serviceprincipalidentity-resource-type"></a>Tipo de recurso servicePrincipalIdentity

Namespace: microsoft.graph

Modela uma identidade de entidade de serviço.

Herda da [identidade](../resources/identity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appId|String|O identificador de aplicativo da entidade de serviço.|
|displayName|String|O nome de exibição da identidade da entidade de serviço. Herdado da [identidade](../resources/identity.md)|
|id|String|O identificador da identidade da entidade de serviço. Herdado da [identidade](../resources/identity.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.servicePrincipalIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.servicePrincipalIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "appId": "String"
}
```
