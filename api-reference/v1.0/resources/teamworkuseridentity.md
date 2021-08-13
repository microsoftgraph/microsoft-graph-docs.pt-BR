---
title: tipo de recurso teamworkUserIdentity
description: Representa um usuário no Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 107ff351d17cf999fa0d2dce085587f5b2ea16edd6bf5315ded551fe78554629
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146381"
---
# <a name="teamworkuseridentity-resource-type"></a>tipo de recurso teamworkUserIdentity

Namespace: microsoft.graph

Representa um **usuário** em Microsoft Teams.


Herda da [identidade](../resources/identity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Herdado da [identidade](../resources/identity.md). Nome de exibição do usuário. Opcional.|
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

