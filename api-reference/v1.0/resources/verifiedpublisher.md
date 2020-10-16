---
title: tipo de recurso verifiedPublisher
description: Representa o fornecedor verificado do aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jesakowi
ms.openlocfilehash: 0285eb767a2fc4606dceaf74693a570f14dd6612
ms.sourcegitcommit: c28da0e5feea4791c19663a30b223a0a5da0ed02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/15/2020
ms.locfileid: "48471501"
---
# <a name="verifiedpublisher-resource-type"></a>tipo de recurso verifiedPublisher

Namespace: microsoft.graph

Representa o fornecedor verificado do [aplicativo](application.md). Para obter mais informações, consulte [Publisher Verification](https://docs.microsoft.com/azure/active-directory/develop/publisher-verification-overview). Os editores verificados são definidos usando o [setVerifiedPublisher](../api/application-setverifiedpublisher.md) e só podem ser removidos usando o [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|displayName|Cadeia de caracteres|O nome do editor verificado da conta do centro de parceria do fornecedor de aplicativos.|
|verifiedPublisherId|Cadeia de caracteres| A ID do editor verificado da conta do centro de parceria do fornecedor de aplicativos. |
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


<!-- uuid: 7a355221-34dd-4579-9bdd-4c3e1909e1bb
2020-09-09 20:45:56 UTC -->
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
