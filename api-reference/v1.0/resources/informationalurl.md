---
title: tipo de recurso informationalUrl
description: Informações de perfil básicas do aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 31a8096ebe5cb8aecba56a1a6f6c6367adf4b7af
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054872"
---
# <a name="informationalurl-resource-type"></a>tipo de recurso informationalUrl

Namespace: microsoft.graph

Informações de perfil básicas do aplicativo.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|logoUrl|String|A URL da CDN para o logotipo do aplicativo, somente leitura.|
|marketingUrl|String| Link para a página de marketing do aplicativo. Por exemplo, https://www.contoso.com/app/marketing |
|privacyStatementUrl|String| Link para a política de privacidade do aplicativo. Por exemplo, https://www.contoso.com/app/privacy |
|supportUrl|String| Link para a página de suporte do aplicativo. Por exemplo, https://www.contoso.com/app/support |
|termsOfServiceUrl|String| Link para a instrução de termos de serviço do aplicativo. Por exemplo, https://www.contoso.com/app/termsofservice |

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

