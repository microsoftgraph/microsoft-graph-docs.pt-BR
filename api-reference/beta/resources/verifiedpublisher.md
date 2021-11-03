---
title: Tipo de recurso verifiedPublisher
description: Representa o editor verificado do aplicativo.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: jesakowi
ms.openlocfilehash: 64c96fe5146095f778b239dc7e4e2031e484afc6
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696669"
---
# <a name="verifiedpublisher-resource-type"></a>Tipo de recurso verifiedPublisher

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um editor verificado de um [aplicativo](application.md). Para obter mais informações, [consulte Publisher verificação](/azure/active-directory/develop/publisher-verification-overview). Os editores verificados são definidos usando [setVerifiedPublisher](../api/application-setverifiedpublisher.md) e só podem ser removidos usando [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|addedDateTime|DateTimeOffSet| O timestamp quando o editor verificado foi adicionado pela primeira vez ou atualizado mais recentemente. |
|displayName|String|O nome do editor verificado da conta do Microsoft Partner Network (MPN) do editor de aplicativos.|
|verifiedPublisherId|String| A ID do editor verificado na conta do Partner Center do editor de aplicativos. |


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
