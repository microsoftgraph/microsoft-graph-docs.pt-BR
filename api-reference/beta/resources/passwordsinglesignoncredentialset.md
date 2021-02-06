---
title: Tipo de recurso passwordSingleSignOnCredentialSet
description: Indica um conjunto de credenciais que definem completamente um fluxo de login de um usuário ou grupo para um aplicativo.
localization_priority: Normal
author: bharathramh92
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 95526942bcedfc20d983a8873699af6902482b2c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130871"
---
# <a name="passwordsinglesignoncredentialset-resource-type"></a>Tipo de recurso passwordSingleSignOnCredentialSet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica um conjunto de credenciais que definem completamente um fluxo de login de um usuário ou grupo para um aplicativo.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|credenciais|[coleção de](credential.md) credenciais|Uma lista de objetos de credencial que definem o fluxo de login completo.|
|id|String|A ID do usuário ou grupo ao que esse conjunto de credenciais pertence.|

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


