---
title: Tipo de recurso servicePrincipalIdentity
description: Modela uma identidade de entidade de serviço.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f2daece3e3f9fb01c58a2470aa667da7e62ce4ef
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697925"
---
# <a name="serviceprincipalidentity-resource-type"></a>Tipo de recurso servicePrincipalIdentity

Namespace: microsoft.graph

Modela uma identidade de entidade de serviço.

Herda da [identidade](../resources/identity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appId|Cadeia de caracteres|O identificador de aplicativo da entidade de serviço.|
|displayName|Cadeia de caracteres|O nome de exibição da identidade da entidade de serviço. Herdado da [identidade](../resources/identity.md)|
|id|Cadeia de caracteres|O identificador da identidade da entidade de serviço. Herdado da [identidade](../resources/identity.md)|

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
