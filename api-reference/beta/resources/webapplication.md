---
title: Tipo de recurso webApplication
description: Especifica configurações para um aplicativo Web.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: f4f6ec9d65dd6d30b54b030651178484392fba06
ms.sourcegitcommit: 0ec845f93eaa140ad833ba163c76c5308197a92f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2021
ms.locfileid: "60068541"
---
# <a name="webapplication-resource-type"></a>Tipo de recurso webApplication

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica configurações para um aplicativo Web.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| homePageUrl | String | Página inicial ou página de aterrissagem do aplicativo. |
| implicitGrantSettings | [implicitGrantSettings](implicitgrantsettings.md)| Especifica se esse aplicativo Web pode solicitar tokens usando o fluxo implícito OAuth 2.0. |
| logoutUrl | String | Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML. |
| redirectUris | Coleção de cadeia de caracteres | Especifica as URLs para as quais os tokens de usuário são enviados para entrar ou as URIs de redirecionamento para as quais os códigos de autorização do OAuth 2.0 e tokens de acesso são enviados. |
|redirectUriSettings| [Coleção redirectUriSettings](redirecturisettings.md) | Especifica o índice das URLs onde os tokens de usuário são enviados para entrar. Isso só é válido para aplicativos que usam SAML.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.webApplication"
}-->

```json
{
  "homePageUrl": "String",
  "implicitGrantSettings": {"@odata.type": "microsoft.graph.implicitGrantSettings"},
  "logoutUrl": "String",
  "redirectUris": ["String"],
  "redirectUriSettings": [
    {
      "@odata.type": "microsoft.graph.redirectUriSettings"
    }
  ],
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "webApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


