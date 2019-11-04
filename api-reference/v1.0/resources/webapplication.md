---
title: tipo de recurso webApplication
description: Especifica configurações para um aplicativo Web.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: c9b0c2f36913d3d89edb1bd119b2473158f0a9bb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939050"
---
# <a name="webapplication-resource-type"></a><span data-ttu-id="dd9a7-103">tipo de recurso webApplication</span><span class="sxs-lookup"><span data-stu-id="dd9a7-103">webApplication resource type</span></span>

<span data-ttu-id="dd9a7-104">Especifica configurações para um aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="dd9a7-104">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="dd9a7-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd9a7-105">Properties</span></span>

| <span data-ttu-id="dd9a7-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd9a7-106">Property</span></span> | <span data-ttu-id="dd9a7-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd9a7-107">Type</span></span> | <span data-ttu-id="dd9a7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd9a7-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="dd9a7-109">homePageUrl</span><span class="sxs-lookup"><span data-stu-id="dd9a7-109">homePageUrl</span></span> | <span data-ttu-id="dd9a7-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd9a7-110">String</span></span> | <span data-ttu-id="dd9a7-111">Página inicial ou página de aterrissagem do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dd9a7-111">Home page or landing page of the application.</span></span> |
| <span data-ttu-id="dd9a7-112">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="dd9a7-112">implicitGrantSettings</span></span> | [<span data-ttu-id="dd9a7-113">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="dd9a7-113">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="dd9a7-114">Especifica se este aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="dd9a7-114">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> |
| <span data-ttu-id="dd9a7-115">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="dd9a7-115">logoutUrl</span></span> | <span data-ttu-id="dd9a7-116">String</span><span class="sxs-lookup"><span data-stu-id="dd9a7-116">String</span></span> | <span data-ttu-id="dd9a7-117">Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML.</span><span class="sxs-lookup"><span data-stu-id="dd9a7-117">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
| <span data-ttu-id="dd9a7-118">redirectUris</span><span class="sxs-lookup"><span data-stu-id="dd9a7-118">redirectUris</span></span> | <span data-ttu-id="dd9a7-119">String collection</span><span class="sxs-lookup"><span data-stu-id="dd9a7-119">String collection</span></span> | <span data-ttu-id="dd9a7-120">Especifica as URLs nas quais os tokens de usuário são enviados para entrada ou os URIs de redirecionamento nos quais os códigos de autorização OAuth 2,0 e tokens de acesso são enviados.</span><span class="sxs-lookup"><span data-stu-id="dd9a7-120">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dd9a7-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd9a7-121">JSON representation</span></span>
<span data-ttu-id="dd9a7-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd9a7-122">Here is a JSON representation of the resource.</span></span>

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
