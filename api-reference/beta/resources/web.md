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
# <a name="web-resource-type"></a><span data-ttu-id="f5d0d-103">tipo de recurso da Web</span><span class="sxs-lookup"><span data-stu-id="f5d0d-103">web resource type</span></span>

> <span data-ttu-id="f5d0d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f5d0d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5d0d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f5d0d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5d0d-106">Especifica as configurações para um aplicativo web.</span><span class="sxs-lookup"><span data-stu-id="f5d0d-106">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="f5d0d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5d0d-107">Properties</span></span>

| <span data-ttu-id="f5d0d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5d0d-108">Property</span></span> | <span data-ttu-id="f5d0d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5d0d-109">Type</span></span> | <span data-ttu-id="f5d0d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5d0d-110">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="f5d0d-111">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="f5d0d-111">implicitGrantSettings</span></span>|[<span data-ttu-id="f5d0d-112">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="f5d0d-112">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="f5d0d-113">Especifica se esse aplicativo web pode solicitar tokens usando o fluxo de implícita OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="f5d0d-113">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="f5d0d-114">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="f5d0d-114">logoutUrl</span></span>|<span data-ttu-id="f5d0d-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5d0d-115">String</span></span>| <span data-ttu-id="f5d0d-116">Especifica a URL que será usada pelo serviço de autorização da Microsoft para logout um usuário usando o [canal de frente](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou protocolos de logout SAML.</span><span class="sxs-lookup"><span data-stu-id="f5d0d-116">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="f5d0d-117">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="f5d0d-117">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="f5d0d-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5d0d-118">Boolean</span></span>| <span data-ttu-id="f5d0d-119">Obsoleto.</span><span class="sxs-lookup"><span data-stu-id="f5d0d-119">Deprecated.</span></span> <span data-ttu-id="f5d0d-120">Não a use.</span><span class="sxs-lookup"><span data-stu-id="f5d0d-120">Do not use.</span></span> | 
|<span data-ttu-id="f5d0d-121">redirectUris</span><span class="sxs-lookup"><span data-stu-id="f5d0d-121">redirectUris</span></span>|<span data-ttu-id="f5d0d-122">String collection</span><span class="sxs-lookup"><span data-stu-id="f5d0d-122">String collection</span></span>| <span data-ttu-id="f5d0d-123">Especifica o redirecionamento de códigos de autorização de URIs que OAuth 2.0 e tokens de acesso são enviados para ou as URLs que os tokens do usuário são enviados para entrar.</span><span class="sxs-lookup"><span data-stu-id="f5d0d-123">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f5d0d-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5d0d-124">JSON representation</span></span>
<span data-ttu-id="f5d0d-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5d0d-125">Here is a JSON representation of the resource.</span></span>

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
