---
title: Tipo de recurso keyValue
description: Fornece informações relevantes adicionais sobre a solicitação de login
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3459f827f35049b383e732c805d61371577b2260
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135391"
---
# <a name="keyvalue-resource-type"></a>Tipo de recurso keyValue

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece informações adicionais de processamento de autenticação, como o nome do servidor e a presença de dicas para entrar e domínio.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|key|String|Contém o nome do campo ao que um valor está associado. Quando uma dica de login ou domínio é incluída na solicitação de login, os campos correspondentes são incluídos como pares chave-valor. Chaves possíveis: `Login hint present` , `Domain hint present` .|
|value|Cadeia de caracteres|Contém o valor correspondente para a chave especificada. O valor é `true` se uma dica de login foi incluída na solicitação de login; caso `false` contrário. O valor é `true` se uma dica de domínio foi incluída na solicitação de login; caso `false` contrário.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValue",
  "baseType": null
}-->

```json
{
  "key": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


