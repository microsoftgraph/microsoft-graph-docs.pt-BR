---
title: tipo de recurso webApplication
description: Especifica configurações para um aplicativo Web.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: af9f183011ee8774387288f8d02c4bade8352f6b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033507"
---
# <a name="webapplication-resource-type"></a><span data-ttu-id="33b46-103">tipo de recurso webApplication</span><span class="sxs-lookup"><span data-stu-id="33b46-103">webApplication resource type</span></span>

<span data-ttu-id="33b46-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33b46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33b46-105">Especifica configurações para um aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="33b46-105">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="33b46-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33b46-106">Properties</span></span>

| <span data-ttu-id="33b46-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33b46-107">Property</span></span> | <span data-ttu-id="33b46-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="33b46-108">Type</span></span> | <span data-ttu-id="33b46-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="33b46-109">Description</span></span> |
|:---------|:-----|:------------|
| `homePageUrl` | <span data-ttu-id="33b46-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33b46-110">String</span></span> | <span data-ttu-id="33b46-111">Página inicial ou página de aterrissagem do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="33b46-111">Home page or landing page of the application.</span></span> |
| `implicitGrantSettings` | [<span data-ttu-id="33b46-112">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="33b46-112">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="33b46-113">Especifica se este aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="33b46-113">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> |
| `logoutUrl` | <span data-ttu-id="33b46-114">String</span><span class="sxs-lookup"><span data-stu-id="33b46-114">String</span></span> | <span data-ttu-id="33b46-115">Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML.</span><span class="sxs-lookup"><span data-stu-id="33b46-115">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
| `redirectUris` | <span data-ttu-id="33b46-116">Coleção String</span><span class="sxs-lookup"><span data-stu-id="33b46-116">String collection</span></span> | <span data-ttu-id="33b46-117">Especifica as URLs nas quais os tokens de usuário são enviados para entrada ou os URIs de redirecionamento nos quais os códigos de autorização OAuth 2,0 e tokens de acesso são enviados.</span><span class="sxs-lookup"><span data-stu-id="33b46-117">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="33b46-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33b46-118">JSON representation</span></span>
<span data-ttu-id="33b46-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="33b46-119">Here is a JSON representation of the resource.</span></span>

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


