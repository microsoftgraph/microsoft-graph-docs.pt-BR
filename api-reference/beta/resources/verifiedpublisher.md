---
title: tipo de recurso verifiedPublisher
description: Representa o fornecedor verificado do aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jesakowi
ms.openlocfilehash: 0d704b42c83a853d094406c0ba62010da30ce142
ms.sourcegitcommit: c28da0e5feea4791c19663a30b223a0a5da0ed02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/15/2020
ms.locfileid: "48471545"
---
# <a name="verifiedpublisher-resource-type"></a>tipo de recurso verifiedPublisher

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um fornecedor verificado de um [aplicativo](application.md). Para obter mais informações, consulte [Publisher Verification](/azure/active-directory/develop/publisher-verification-overview). Os editores verificados são definidos usando o [setVerifiedPublisher](../api/application-setverifiedpublisher.md) e só podem ser removidos usando o [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|displayName|String|O nome do editor verificado da conta do Microsoft Partner Network (MPN) do editor de aplicativos.|
|verifiedPublisherId|String| A ID do editor verificado da conta do centro de parceria do fornecedor de aplicativos. |
|addedDateTime|DateTimeOffSet| O carimbo de data/hora da primeira adição ou atualização mais recente do editor verificado. |


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedPublisher"
}-->

```json
{
  "displayName": "String",
  "verifiedPublisherId": "String",
  "addedDateTime": "DateTimeOffSet"
}

```


<!-- uuid: e9aa37e1-f0b7-4201-a6b2-d26ce091dff6
2020-09-09 20:42:32 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "verifiedPublisher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
