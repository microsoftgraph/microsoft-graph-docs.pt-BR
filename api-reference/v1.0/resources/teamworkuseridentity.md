---
title: tipo de recurso teamworkUserIdentity
description: Representa um usuário no Microsoft Teams.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d6989f7b3c5689fefe8e9516e25fd6ff3777fe16
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128155"
---
# <a name="teamworkuseridentity-resource-type"></a>tipo de recurso teamworkUserIdentity

Namespace: microsoft.graph

Representa um **usuário** em Microsoft Teams.


Herda da [identidade](../resources/identity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Herdado da [identidade](../resources/identity.md). Nome de exibição do usuário. Opcional.|
|id|Cadeia de caracteres|Herdado da [identidade](../resources/identity.md). ID do usuário. |
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

