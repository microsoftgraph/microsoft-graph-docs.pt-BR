---
title: tipo de recurso webApplication
description: Especifica configurações para um aplicativo Web.
localization_priority: Normal
ms.openlocfilehash: cdb210d5193167138ecec216b1e4084554f05c78
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348343"
---
# <a name="webapplication-resource-type"></a><span data-ttu-id="4f827-103">tipo de recurso webApplication</span><span class="sxs-lookup"><span data-stu-id="4f827-103">webApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f827-104">Especifica configurações para um aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="4f827-104">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="4f827-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4f827-105">Properties</span></span>

| <span data-ttu-id="4f827-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f827-106">Property</span></span> | <span data-ttu-id="4f827-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f827-107">Type</span></span> | <span data-ttu-id="4f827-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f827-108">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="4f827-109">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="4f827-109">implicitGrantSettings</span></span>|[<span data-ttu-id="4f827-110">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="4f827-110">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="4f827-111">Especifica se este aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="4f827-111">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="4f827-112">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="4f827-112">logoutUrl</span></span>|<span data-ttu-id="4f827-113">String</span><span class="sxs-lookup"><span data-stu-id="4f827-113">String</span></span>| <span data-ttu-id="4f827-114">Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML.</span><span class="sxs-lookup"><span data-stu-id="4f827-114">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="4f827-115">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="4f827-115">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="4f827-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f827-116">Boolean</span></span>| <span data-ttu-id="4f827-117">Obsoleto.</span><span class="sxs-lookup"><span data-stu-id="4f827-117">Deprecated.</span></span> <span data-ttu-id="4f827-118">Não usar.</span><span class="sxs-lookup"><span data-stu-id="4f827-118">Do not use.</span></span> | 
|<span data-ttu-id="4f827-119">redirectUris</span><span class="sxs-lookup"><span data-stu-id="4f827-119">redirectUris</span></span>|<span data-ttu-id="4f827-120">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f827-120">String collection</span></span>| <span data-ttu-id="4f827-121">Especifica as URLs às quais os tokens de usuário são enviados para entrar ou os URIs de redirecionamento aos quais os códigos de autorização OAuth 2,0 e tokens de acesso são enviados.</span><span class="sxs-lookup"><span data-stu-id="4f827-121">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4f827-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4f827-122">JSON representation</span></span>
<span data-ttu-id="4f827-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4f827-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.webApplication"
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
