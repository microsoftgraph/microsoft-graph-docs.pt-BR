---
title: tipo de recurso passwordSingleSignOnCredentialSet
description: Indica um conjunto de credenciais que definem completamente um fluxo de entrada para um usuário ou grupo para um aplicativo.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6293c6a2fbdffd124a8e011bd00a22c30efa77e5
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658790"
---
# <a name="passwordsinglesignoncredentialset-resource-type"></a>tipo de recurso passwordSingleSignOnCredentialSet

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
