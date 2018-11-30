---
title: tipo de recurso de informationalUrl
description: Informações básicas de perfil do aplicativo.
ms.openlocfilehash: c8a13f4f686fe3b6ffd460ab05342b7da9b4a808
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038196"
---
# <a name="informationalurl-resource-type"></a>tipo de recurso de informationalUrl

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Informações básicas de perfil do aplicativo.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|marketing|String| Link para a página de marketing do aplicativo. Por exemplo, https://www.contoso.com/app/marketing |
|privacidade|String| Link para a declaração de privacidade do aplicativo. Por exemplo, https://www.contoso.com/app/privacy |
|suporte|String| Link para a página de suporte do aplicativo. Por exemplo, https://www.contoso.com/app/support |
|termsOfService|String| Link para os termos do aplicativo de instrução de serviço. Por exemplo, https://www.contoso.com/app/termsofservice |

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
  "marketing": "String",
  "privacy": "String",
  "support": "String",
  "termsOfService": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->