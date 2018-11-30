---
title: tipo de recurso da Web
description: Especifica as configurações para um aplicativo web.
ms.openlocfilehash: c040de0c323e57f20e04dcf662ea088b1018c144
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039067"
---
# <a name="web-resource-type"></a><span data-ttu-id="52224-103">tipo de recurso da Web</span><span class="sxs-lookup"><span data-stu-id="52224-103">web resource type</span></span>

> <span data-ttu-id="52224-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="52224-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52224-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="52224-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="52224-106">Especifica as configurações para um aplicativo web.</span><span class="sxs-lookup"><span data-stu-id="52224-106">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="52224-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52224-107">Properties</span></span>

| <span data-ttu-id="52224-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52224-108">Property</span></span> | <span data-ttu-id="52224-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="52224-109">Type</span></span> | <span data-ttu-id="52224-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="52224-110">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="52224-111">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="52224-111">implicitGrantSettings</span></span>|[<span data-ttu-id="52224-112">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="52224-112">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="52224-113">Especifica se esse aplicativo web pode solicitar tokens usando o fluxo de implícita OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="52224-113">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="52224-114">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="52224-114">logoutUrl</span></span>|<span data-ttu-id="52224-115">String</span><span class="sxs-lookup"><span data-stu-id="52224-115">String</span></span>| <span data-ttu-id="52224-116">Especifica a URL que será usada pelo serviço de autorização da Microsoft para logout um usuário usando o [canal de frente](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou protocolos de logout SAML.</span><span class="sxs-lookup"><span data-stu-id="52224-116">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="52224-117">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="52224-117">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="52224-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="52224-118">Boolean</span></span>| <span data-ttu-id="52224-119">Obsoleto.</span><span class="sxs-lookup"><span data-stu-id="52224-119">Deprecated.</span></span> <span data-ttu-id="52224-120">Não a use.</span><span class="sxs-lookup"><span data-stu-id="52224-120">Do not use.</span></span> | 
|<span data-ttu-id="52224-121">redirectUris</span><span class="sxs-lookup"><span data-stu-id="52224-121">redirectUris</span></span>|<span data-ttu-id="52224-122">String collection</span><span class="sxs-lookup"><span data-stu-id="52224-122">String collection</span></span>| <span data-ttu-id="52224-123">Especifica o redirecionamento de códigos de autorização de URIs que OAuth 2.0 e tokens de acesso são enviados para ou as URLs que os tokens do usuário são enviados para entrar.</span><span class="sxs-lookup"><span data-stu-id="52224-123">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="52224-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52224-124">JSON representation</span></span>
<span data-ttu-id="52224-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52224-125">Here is a JSON representation of the resource.</span></span>

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
