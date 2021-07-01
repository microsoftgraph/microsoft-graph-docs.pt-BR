---
title: tipo de recurso teamworkUserIdentity
description: Representa um usuário no Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7ae7655a5b2c84cc01d354d32d25eb724d5f4a6c
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211063"
---
# <a name="teamworkuseridentity-resource-type"></a>tipo de recurso teamworkUserIdentity

Namespace: microsoft.graph

Representa um **usuário** em Microsoft Teams.


Herda da [identidade](../resources/identity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Herdado da [identidade](../resources/identity.md). Nome de exibição do usuário. Opcional.|
|id|String|Herdado da [identidade](../resources/identity.md). ID do usuário. |
|userIdentityType|teamworkUserIdentityType| Tipo de usuário. Os valores possíveis são: `aadUser` , , , , , , e `onPremiseAadUser` `anonymousGuest` `federatedUser` `personalMicrosoftAccountUser` `skypeUser` `phoneUser` `unknownFutureValue` .|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkUserIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkUserIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "userIdentityType": "String"
}
```

