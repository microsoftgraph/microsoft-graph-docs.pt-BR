---
title: Tipo de recurso verifiedPublisher
description: Representa o editor verificado do aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: jesakowi
ms.openlocfilehash: 5acc66bd72c65b25d8301c4870fa5ff0f98a0d73
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135622"
---
# <a name="verifiedpublisher-resource-type"></a>tipo de recurso verifiedPublisher

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um editor verificado de um [aplicativo](application.md). Para obter mais informações, consulte Verificação [do Publisher.](/azure/active-directory/develop/publisher-verification-overview) Os editores verificados são definidos usando [setVerifiedPublisher](../api/application-setverifiedpublisher.md) e só podem ser removidos usando [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|displayName|String|O nome do editor verificado da conta do Microsoft Partner Network (MPN) do editor de aplicativos.|
|verifiedPublisherId|String| A ID do editor verificado da conta do Partner Center do editor de aplicativos. |
|addedDateTime|DateTimeOffSet| O timestamp quando o editor verificado foi adicionado pela primeira vez ou atualizado mais recentemente. |


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
