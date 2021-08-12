---
title: Tipo de recurso servicePrincipalIdentity
description: Modela uma identidade de entidade de serviço.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9f486efbbfefb9639551c4d7fa587d056aaf3211e5b53dd8d212b7171b59baac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202116"
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
