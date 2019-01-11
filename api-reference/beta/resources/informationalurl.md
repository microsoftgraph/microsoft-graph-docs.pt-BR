---
title: tipo de recurso de informationalUrl
description: Informações básicas de perfil do aplicativo.
localization_priority: Normal
ms.openlocfilehash: 78fd03a2673b342d1a0c904f521fe5a0f8cba205
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816979"
---
# <a name="informationalurl-resource-type"></a>tipo de recurso de informationalUrl

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Informações básicas de perfil do aplicativo.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|marketing|Cadeia de caracteres| Link para a página de marketing do aplicativo. Por exemplo, https://www.contoso.com/app/marketing |
|privacidade|Cadeia de caracteres| Link para a declaração de privacidade do aplicativo. Por exemplo, https://www.contoso.com/app/privacy |
|suporte|Cadeia de caracteres| Link para a página de suporte do aplicativo. Por exemplo, https://www.contoso.com/app/support |
|termsOfService|Cadeia de caracteres| Link para os termos do aplicativo de instrução de serviço. Por exemplo, https://www.contoso.com/app/termsofservice |

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
