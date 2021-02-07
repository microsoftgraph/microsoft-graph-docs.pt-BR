---
title: Tipo de recurso webApplication
description: Especifica configurações para um aplicativo Web.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: cd524b0692775368c6426012d1829b5cf2119827
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135486"
---
# <a name="webapplication-resource-type"></a><span data-ttu-id="b475e-103">Tipo de recurso webApplication</span><span class="sxs-lookup"><span data-stu-id="b475e-103">webApplication resource type</span></span>

<span data-ttu-id="b475e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b475e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b475e-105">Especifica configurações para um aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="b475e-105">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="b475e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b475e-106">Properties</span></span>

| <span data-ttu-id="b475e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b475e-107">Property</span></span> | <span data-ttu-id="b475e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b475e-108">Type</span></span> | <span data-ttu-id="b475e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b475e-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="b475e-110">homePageUrl</span><span class="sxs-lookup"><span data-stu-id="b475e-110">homePageUrl</span></span> | <span data-ttu-id="b475e-111">String</span><span class="sxs-lookup"><span data-stu-id="b475e-111">String</span></span> | <span data-ttu-id="b475e-112">Página inicial ou página de aterrissagem do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b475e-112">Home page or landing page of the application.</span></span> |
| <span data-ttu-id="b475e-113">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="b475e-113">implicitGrantSettings</span></span> | [<span data-ttu-id="b475e-114">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="b475e-114">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="b475e-115">Especifica se esse aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="b475e-115">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> |
| <span data-ttu-id="b475e-116">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="b475e-116">logoutUrl</span></span> | <span data-ttu-id="b475e-117">String</span><span class="sxs-lookup"><span data-stu-id="b475e-117">String</span></span> | <span data-ttu-id="b475e-118">Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML.</span><span class="sxs-lookup"><span data-stu-id="b475e-118">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
| <span data-ttu-id="b475e-119">redirectUris</span><span class="sxs-lookup"><span data-stu-id="b475e-119">redirectUris</span></span> | <span data-ttu-id="b475e-120">String collection</span><span class="sxs-lookup"><span data-stu-id="b475e-120">String collection</span></span> | <span data-ttu-id="b475e-121">Especifica as URLs para onde os tokens de usuário são enviados para entrada ou os URIs de redirecionamento para os quais os códigos de autorização e tokens de acesso do OAuth 2.0 são enviados.</span><span class="sxs-lookup"><span data-stu-id="b475e-121">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b475e-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b475e-122">JSON representation</span></span>
<span data-ttu-id="b475e-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b475e-123">Here is a JSON representation of the resource.</span></span>

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

