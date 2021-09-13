---
title: Tipo de recurso servicePrincipalIdentity
description: Modela uma identidade de entidade de serviço.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ae9d82ce65b7a6e8c82e0377df89939b9219f3db
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59108825"
---
# <a name="serviceprincipalidentity-resource-type"></a>Tipo de recurso servicePrincipalIdentity

Namespace: microsoft.graph

Modela uma identidade de entidade de serviço.

Herda da [identidade](../resources/identity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appId|Cadeia de caracteres|O identificador de aplicativo da entidade de serviço.|
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
