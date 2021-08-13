---
title: Tipo de recurso teamworkApplicationIdentity
description: Representa um aplicativo em Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 78f5a4c681cae391037c6dc73d7d102d94dda6ce9c349fe6d5eeeed3fd9f3d8d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249115"
---
# <a name="teamworkapplicationidentity-resource-type"></a>Tipo de recurso teamworkApplicationIdentity

Namespace: microsoft.graph

Representa um **aplicativo** em Microsoft Teams. `teamworkApplicationIdentity` é usado para representar bots e webhooks de saída @mentioned mensagens.


Herda da [identidade](../resources/identity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|applicationIdentityType|teamworkApplicationIdentityType| Tipo de aplicativo referenciado. Os valores possíveis são: `aadApplication` , , , , e `bot` `tenantBot` `office365Connector` `outgoingWebhook` `unknownFutureValue` .|
|displayName|Cadeia de caracteres|Herdado da [identidade](../resources/identity.md). Nome de exibição do aplicativo. Opcional.|
|id|Cadeia de caracteres|Herdado da [identidade](../resources/identity.md). ID do aplicativo.|

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

