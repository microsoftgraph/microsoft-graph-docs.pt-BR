---
title: Tipo de recurso verifiedPublisher
description: Representa o editor verificado do aplicativo.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: jesakowi
ms.openlocfilehash: 4c63c0cdcfb6324077092923eeff91eed65e7b60
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134280"
---
# <a name="verifiedpublisher-resource-type"></a>Tipo de recurso verifiedPublisher

Namespace: microsoft.graph

Representa o editor verificado do [aplicativo](application.md). Para obter mais informações, [consulte Publisher verificação](/azure/active-directory/develop/publisher-verification-overview). Os editores verificados são definidos usando [setVerifiedPublisher](../api/application-setverifiedpublisher.md) e só podem ser removidos usando [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|displayName|Cadeia de caracteres|O nome do editor verificado da conta do Partner Center do editor de aplicativos.|
|verifiedPublisherId|Cadeia de caracteres| A ID do editor verificado na conta do Partner Center do editor de aplicativos. |
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
