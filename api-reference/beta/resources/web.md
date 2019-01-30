---
title: tipo de recurso da Web
description: Especifica configurações para um aplicativo Web.
localization_priority: Normal
ms.openlocfilehash: 7e03977481f0c021b7d67ec44fd4db275642cdf8
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643507"
---
# <a name="web-resource-type"></a><span data-ttu-id="f139a-103">tipo de recurso da Web</span><span class="sxs-lookup"><span data-stu-id="f139a-103">web resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f139a-104">Especifica configurações para um aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="f139a-104">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="f139a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f139a-105">Properties</span></span>

| <span data-ttu-id="f139a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f139a-106">Property</span></span> | <span data-ttu-id="f139a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f139a-107">Type</span></span> | <span data-ttu-id="f139a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f139a-108">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="f139a-109">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="f139a-109">implicitGrantSettings</span></span>|[<span data-ttu-id="f139a-110">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="f139a-110">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="f139a-111">Especifica se esse aplicativo web pode solicitar tokens usando o fluxo de implícita OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="f139a-111">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="f139a-112">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="f139a-112">logoutUrl</span></span>|<span data-ttu-id="f139a-113">String</span><span class="sxs-lookup"><span data-stu-id="f139a-113">String</span></span>| <span data-ttu-id="f139a-114">Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML.</span><span class="sxs-lookup"><span data-stu-id="f139a-114">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="f139a-115">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="f139a-115">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="f139a-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="f139a-116">Boolean</span></span>| <span data-ttu-id="f139a-117">Obsoleto.</span><span class="sxs-lookup"><span data-stu-id="f139a-117">Deprecated.</span></span> <span data-ttu-id="f139a-118">Não a use.</span><span class="sxs-lookup"><span data-stu-id="f139a-118">Do not use.</span></span> | 
|<span data-ttu-id="f139a-119">redirectUris</span><span class="sxs-lookup"><span data-stu-id="f139a-119">redirectUris</span></span>|<span data-ttu-id="f139a-120">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f139a-120">String collection</span></span>| <span data-ttu-id="f139a-121">Especifica o redirecionamento de códigos de autorização de URIs que OAuth 2.0 e tokens de acesso são enviados para ou as URLs que os tokens do usuário são enviados para entrar.</span><span class="sxs-lookup"><span data-stu-id="f139a-121">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f139a-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f139a-122">JSON representation</span></span>
<span data-ttu-id="f139a-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f139a-123">Here is a JSON representation of the resource.</span></span>

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
