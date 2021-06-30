---
title: Tipo de recurso teamworkApplicationIdentity
description: Representa um aplicativo em Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b7e6c17b70e7f30e102e270d2d98b406e01dcae3
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211206"
---
# <a name="teamworkapplicationidentity-resource-type"></a>Tipo de recurso teamworkApplicationIdentity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um **aplicativo** em Microsoft Teams. `teamworkApplicationIdentity` é usado para representar bots e webhooks de saída @mentioned mensagens.


Herda da [identidade](../resources/identity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|applicationIdentityType|teamworkApplicationIdentityType| Tipo de aplicativo referenciado. Os valores possíveis são: `aadApplication` , , , e `bot` `tenantBot` `office365Connector` `outgoingWebhook` .|
|displayName|String|Herdado da [identidade](../resources/identity.md). Nome de exibição do aplicativo. Opcional.|
|id|String|Herdado da [identidade](../resources/identity.md). ID do aplicativo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkApplicationIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkApplicationIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "applicationIdentityType": "String"
}
```

