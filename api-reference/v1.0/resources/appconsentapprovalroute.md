---
title: Tipo de recurso appConsentApprovalRoute
description: Contêiner para recursos básicos que expõem a API e os recursos de solicitação de consentimento do aplicativo. Atualmente, expõe apenas a relação appConsentRequests.
author: psignoret
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cb5e5c3c060c255d7c5154494cc0226031665e5f
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651555"
---
# <a name="appconsentapprovalroute-resource-type"></a>Tipo de recurso appConsentApprovalRoute

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contêiner para recursos básicos que expõem a API e os recursos de solicitação de consentimento do aplicativo. Atualmente, expõe apenas a relação [appConsentRequests.](appconsentrequest.md)

Herda da [entidade](entity.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|appConsentRequests|[Coleção appConsentRequest](../resources/appconsentrequest.md)| Uma coleção de [objetos userConsentRequest](../resources/userconsentrequest.md) para um aplicativo específico.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appConsentApprovalRoute",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConsentApprovalRoute"
}
```

