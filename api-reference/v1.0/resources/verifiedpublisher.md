---
title: Tipo de recurso verifiedPublisher
description: Representa o editor verificado do aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: jesakowi
ms.openlocfilehash: f53559da47f61de645661c1acc8e0a94e4a6e6e6e9cf3c55e6faa8e2149452a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129901"
---
# <a name="verifiedpublisher-resource-type"></a>Tipo de recurso verifiedPublisher

Namespace: microsoft.graph

Representa o editor verificado do [aplicativo](application.md). Para obter mais informações, [consulte Publisher verificação](/azure/active-directory/develop/publisher-verification-overview). Os editores verificados são definidos usando [setVerifiedPublisher](../api/application-setverifiedpublisher.md) e só podem ser removidos usando [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|displayName|Cadeia de caracteres|O nome do editor verificado da conta do Partner Center do editor de aplicativos.|
|verifiedPublisherId|String| A ID do editor verificado na conta do Partner Center do editor de aplicativos. |
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
