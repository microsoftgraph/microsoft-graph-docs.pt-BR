---
title: tipo de recurso da Web
description: Especifica as configurações para um aplicativo web.
localization_priority: Normal
ms.openlocfilehash: 26efe59eda739597e7193fa1ff79443f3d64b5a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890199"
---
# <a name="web-resource-type"></a>tipo de recurso da Web

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Especifica as configurações para um aplicativo web.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
|implicitGrantSettings|[implicitGrantSettings](implicitgrantsettings.md)| Especifica se esse aplicativo web pode solicitar tokens usando o fluxo de implícita OAuth 2.0.|
|logoutUrl|Cadeia de caracteres| Especifica a URL que será usada pelo serviço de autorização da Microsoft para logout um usuário usando o [canal de frente](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou protocolos de logout SAML. |
|oauth2AllowImplicitFlow|Booliano| Obsoleto. Não a use. | 
|redirectUris|String collection| Especifica o redirecionamento de códigos de autorização de URIs que OAuth 2.0 e tokens de acesso são enviados para ou as URLs que os tokens do usuário são enviados para entrar. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.web"
}-->

```json
{
  "implicitGrantSettings": {"@odata.type": "microsoft.graph.implicitGrantSettings"},
  "logoutUrl": "String",
  "oauth2AllowImplicitFlow": false,
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "web resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
