---
title: Tipo de recurso writebackConfiguration
description: Representa um estado de write-back Azure AD grupos de nuvem (Microsoft 365 e grupos de segurança).
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 5b2dffd738684838ac0265f1f745f0071ec0aa60
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447495"
---
# <a name="writebackconfiguration-resource-type"></a>Tipo de recurso writebackConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um estado de write-back Azure AD grupos de nuvem (Microsoft 365 e grupos de segurança).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isEnabled|Booliano|Indica se o write-back de grupos de nuvem para o Active Directory local está habilitado. O valor padrão é `true` para grupos do Microsoft 365 e para `false` grupos de segurança.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.writebackConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.writebackConfiguration",
  "isEnabled": "Boolean"
}
```

