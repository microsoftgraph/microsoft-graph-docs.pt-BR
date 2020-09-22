---
title: tipo de recurso webApplication
description: Especifica configurações para um aplicativo Web.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: aae3184a025757b910e0b19daa8a8d8057128506
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015257"
---
# <a name="webapplication-resource-type"></a>tipo de recurso webApplication

Namespace: microsoft.graph

Especifica configurações para um aplicativo Web.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| homePageUrl | Cadeia de caracteres | Página inicial ou página de aterrissagem do aplicativo. |
| implicitGrantSettings | [implicitGrantSettings](implicitgrantsettings.md)| Especifica se este aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2,0. |
| logoutUrl | String | Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML. |
| redirectUris | Coleção de cadeias de caracteres | Especifica as URLs nas quais os tokens de usuário são enviados para entrada ou os URIs de redirecionamento nos quais os códigos de autorização OAuth 2,0 e tokens de acesso são enviados. |

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
  "redirectUris": ["String"]
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

