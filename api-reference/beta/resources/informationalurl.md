---
title: tipo de recurso informationalUrl
description: Informações de perfil básicas do aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 88b3ae7af8604b6092ad87f2751791f48d273a68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496093"
---
# <a name="informationalurl-resource-type"></a>tipo de recurso informationalUrl

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
