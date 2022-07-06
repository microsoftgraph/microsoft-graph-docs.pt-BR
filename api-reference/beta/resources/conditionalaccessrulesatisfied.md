---
title: Tipo de recurso conditionalAccessRulesSatisfied
description: Indica as regras de acesso condicional atendidas durante um evento de autenticação.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 50ebb20c38275a7ab0192b56ca67058ff640948f
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645436"
---
# <a name="conditionalaccessrulessatisfied-resource-type"></a>Tipo de recurso conditionalAccessRulesSatisfied

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica os atributos relacionados à política de acesso condicional aplicada ou às políticas disparadas pela atividade de entrada correspondente.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|conditionalAccessCondition|conditionalAccessConditions|Refere-se às condições de política de acesso condicional que são atendidas. Os valores possíveis são: `none`, `application`, `users`, `devicePlatform`, `location`, , , `clientType`, `userRisk``signInRisk`, `time`, , `deviceState``client`, , `ipAddressSeenByAzureAD`, `ipAddressSeenByResourceProvider`, , `unknownFutureValue`, , , `servicePrincipals`. `servicePrincipalRisk` Observe que você deve usar o `Prefer: include-unknown-enum-members` cabeçalho da solicitação para obter os seguintes valores nesta [enumeração evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `servicePrincipals`, `servicePrincipalRisk`.|
|ruleSatisfied|conditionalAccessRule|Refere-se às condições de política de acesso condicional que foram atendidas. Os valores possíveis são: `allApps`, `firstPartyApps`, `office365`, `appId`, `acr`, , `appFilter`, , `roleId``allUsers``serviceProvider``allDevicePlatforms``otherExternalUser``devicePlatform``userId``unfamiliarFeatures``allLocations``nationStateIPAddress``insideCorpnet``realTimeThreatIntelligence``b2bCollaborationMember``anonymizedIPAddress``b2bDirectConnectUser``b2bCollaborationGuest``internalGuest``allDeviceStates``deviceFilterIncludeRuleNotMatched``unknownFutureValue``deviceState``allDevices``allTrustedLocations``deviceFilter``guest``groupId``locationId`. Observe que você deve usar o `Prefer: include-unknown-enum-members` cabeçalho da solicitação para obter os seguintes valores nesta [enumeração evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `deviceFilterIncludeRuleNotMatched`, `allDeviceStates`.|


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
