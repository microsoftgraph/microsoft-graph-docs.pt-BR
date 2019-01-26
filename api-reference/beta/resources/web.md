---
title: tipo de recurso da Web
description: Especifica as configurações para um aplicativo web.
localization_priority: Normal
ms.openlocfilehash: 281a3f23dd0e22cae6b3ca2b67e2e9cd8b400740
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572714"
---
# <a name="web-resource-type"></a><span data-ttu-id="35f2b-103">tipo de recurso da Web</span><span class="sxs-lookup"><span data-stu-id="35f2b-103">web resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35f2b-104">Especifica as configurações para um aplicativo web.</span><span class="sxs-lookup"><span data-stu-id="35f2b-104">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="35f2b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35f2b-105">Properties</span></span>

| <span data-ttu-id="35f2b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35f2b-106">Property</span></span> | <span data-ttu-id="35f2b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="35f2b-107">Type</span></span> | <span data-ttu-id="35f2b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f2b-108">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="35f2b-109">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="35f2b-109">implicitGrantSettings</span></span>|[<span data-ttu-id="35f2b-110">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="35f2b-110">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="35f2b-111">Especifica se esse aplicativo web pode solicitar tokens usando o fluxo de implícita OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="35f2b-111">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="35f2b-112">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="35f2b-112">logoutUrl</span></span>|<span data-ttu-id="35f2b-113">String</span><span class="sxs-lookup"><span data-stu-id="35f2b-113">String</span></span>| <span data-ttu-id="35f2b-114">Especifica a URL que será usada pelo serviço de autorização da Microsoft para logout um usuário usando o [canal de frente](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou protocolos de logout SAML.</span><span class="sxs-lookup"><span data-stu-id="35f2b-114">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="35f2b-115">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="35f2b-115">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="35f2b-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f2b-116">Boolean</span></span>| <span data-ttu-id="35f2b-117">Obsoleto.</span><span class="sxs-lookup"><span data-stu-id="35f2b-117">Deprecated.</span></span> <span data-ttu-id="35f2b-118">Não a use.</span><span class="sxs-lookup"><span data-stu-id="35f2b-118">Do not use.</span></span> | 
|<span data-ttu-id="35f2b-119">redirectUris</span><span class="sxs-lookup"><span data-stu-id="35f2b-119">redirectUris</span></span>|<span data-ttu-id="35f2b-120">String collection</span><span class="sxs-lookup"><span data-stu-id="35f2b-120">String collection</span></span>| <span data-ttu-id="35f2b-121">Especifica o redirecionamento de códigos de autorização de URIs que OAuth 2.0 e tokens de acesso são enviados para ou as URLs que os tokens do usuário são enviados para entrar.</span><span class="sxs-lookup"><span data-stu-id="35f2b-121">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35f2b-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35f2b-122">JSON representation</span></span>
<span data-ttu-id="35f2b-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35f2b-123">Here is a JSON representation of the resource.</span></span>

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
  "description": "web resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/web.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
