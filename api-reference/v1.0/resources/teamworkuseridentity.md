---
title: Tipo de recurso teamworkUserIdentity
description: Representa um usuário no Microsoft Teams.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 86b827be0a7d947a627f41f97b4002b7406006ca
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917609"
---
# <a name="teamworkuseridentity-resource-type"></a>Tipo de recurso teamworkUserIdentity

Namespace: microsoft.graph

Representa um **usuário** no Microsoft Teams.


Herda da [identidade](../resources/identity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Herdado da [identidade](../resources/identity.md). Nome de exibição do usuário. Opcional.|
|id|Cadeia de caracteres|Herdado da [identidade](../resources/identity.md). ID do usuário. |
|userIdentityType|teamworkUserIdentityType| Tipo de usuário. Os valores possíveis são: `aadUser`, `onPremiseAadUser`, `anonymousGuest`, `federatedUser`, `personalMicrosoftAccountUser`, `skypeUser`, `phoneUser`e `unknownFutureValue` `emailUser`.|

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

