---
title: tipo de recurso passwordSingleSignOnCredentialSet
description: Indica um conjunto de credenciais que definem completamente um fluxo de entrada para um usuário ou grupo para um aplicativo.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 87aafa6e21171088f9b4b5eac318f6c9551e18ee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998198"
---
# <a name="passwordsinglesignoncredentialset-resource-type"></a>tipo de recurso passwordSingleSignOnCredentialSet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica um conjunto de credenciais que definem completamente um fluxo de entrada para um usuário ou grupo para um aplicativo.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|las|coleção [Credential](credential.md)|Uma lista de objetos de credencial que definem o fluxo de entrada completo.|
|id|String|A ID do usuário ou grupo ao qual esse conjunto de credenciais pertence.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnCredentialSet",
  "baseType": null
}-->

```json
{
  "credentials": [{"@odata.type": "microsoft.graph.credential"}],
  "id": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnCredentialSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


