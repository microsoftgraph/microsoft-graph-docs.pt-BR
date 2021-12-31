---
title: tipo de recurso conditionalAccessRulesSatisfied
description: Indica as regras de acesso condicional atendidas durante um evento de autenticação.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c86ffeaa52941d863529ed4ed3a72d7216359480
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647048"
---
# <a name="conditionalaccessrulessatisfied-resource-type"></a>tipo de recurso conditionalAccessRulesSatisfied

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica os atributos relacionados à política de acesso condicional ou políticas aplicadas que são disparadas pela atividade de entrada correspondente.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|conditionalAccessCondition|conditionalAccessConditions|Refere-se às condições de política de acesso condicional que são atendidas. Os valores possíveis são: `none` , , , , , , , , `application` , , , , `users` , `devicePlatform` , , , `location` , `clientType` `signInRisk` `userRisk` `time` `deviceState` `client` `ipAddressSeenByAzureAD` `ipAddressSeenByResourceProvider` `unknownFutureValue` `servicePrincipals` `servicePrincipalRisk` . Observe que você deve usar o header de solicitação para obter os seguintes valores neste `Prefer: include-unknown-enum-members` [número evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `servicePrincipals` , `servicePrincipalRisk` .|
|ruleSatisfied|conditionalAccessRule|Refere-se às condições de política de acesso condicional que foram atendidas. Os valores possíveis são: `allApps` , , , , , , , `firstPartyApps` , `office365` , , , `appId` `acr` , `appFilter` `allUsers` `guest` `groupId` `roleId` `userId` `allDevicePlatforms` `devicePlatform` `allLocations` `insideCorpnet` , `allTrustedLocations` `locationId` `allDevices` `deviceFilter` `deviceState` `unknownFutureValue` `deviceFilterIncludeRuleNotMatched` `allDeviceStates` Observe que você deve usar o header de solicitação para obter os seguintes valores neste `Prefer: include-unknown-enum-members` [número evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `deviceFilterIncludeRuleNotMatched` , `allDeviceStates` .|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessRuleSatisfied"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessRuleSatisfied",
  "conditionalAccessCondition": "String",
  "ruleSatisfied": "String"
}
```
