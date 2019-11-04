---
title: tipo de recurso informationalUrl
description: Informações de perfil básicas do aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: e81d8cc4a1ef25364727049269b420cf426eb0c8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939478"
---
# <a name="informationalurl-resource-type"></a>tipo de recurso informationalUrl

Informações de perfil básicas do aplicativo.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|logoUrl|Cadeia de caracteres|A URL da CDN para o logotipo do aplicativo, somente leitura.|
|marketingUrl|Cadeia de caracteres| Link para a página de marketing do aplicativo. Por exemplo, https://www.contoso.com/app/marketing |
|privacyStatementUrl|Cadeia de caracteres| Link para a política de privacidade do aplicativo. Por exemplo, https://www.contoso.com/app/privacy |
|supportUrl|Cadeia de caracteres| Link para a página de suporte do aplicativo. Por exemplo, https://www.contoso.com/app/support |
|termsOfServiceUrl|Cadeia de caracteres| Link para a instrução de termos de serviço do aplicativo. Por exemplo, https://www.contoso.com/app/termsofservice |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationalUrl"
}-->

```json
{
  "logoUrl": "String",
  "marketingUrl": "String",
  "privacyStatementUrl": "String",
  "supportUrl": "String",
  "termsOfServiceUrl": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
