---
title: tipo de recurso verifiedPublisher
description: Representa o fornecedor verificado do aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jesakowi
ms.openlocfilehash: d998b8bf3e5ab4ad253e31a96794e8e531e6803e
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921896"
---
# <a name="verifiedpublisher-resource-type"></a>tipo de recurso verifiedPublisher

Namespace: microsoft.graph

Representa o fornecedor verificado do [aplicativo](application.md). Para obter mais informações, consulte [Publisher Verification](/azure/active-directory/develop/publisher-verification-overview). Os editores verificados são definidos usando o [setVerifiedPublisher](../api/application-setverifiedpublisher.md) e só podem ser removidos usando o [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).

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
