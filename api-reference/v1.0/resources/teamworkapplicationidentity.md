---
title: Tipo de recurso teamworkApplicationIdentity
description: Representa um aplicativo em Microsoft Teams.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: af3f0205bf53137791414c2e4777877220ed6ca5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113522"
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

