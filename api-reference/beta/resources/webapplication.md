---
title: Tipo de recurso webApplication
description: Especifica configurações para um aplicativo Web.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 68266c75995fed51038319cf50e0925d5057fa91
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964531"
---
# <a name="webapplication-resource-type"></a><span data-ttu-id="910f5-103">Tipo de recurso webApplication</span><span class="sxs-lookup"><span data-stu-id="910f5-103">webApplication resource type</span></span>

<span data-ttu-id="910f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="910f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="910f5-105">Especifica configurações para um aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="910f5-105">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="910f5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="910f5-106">Properties</span></span>

| <span data-ttu-id="910f5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="910f5-107">Property</span></span> | <span data-ttu-id="910f5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="910f5-108">Type</span></span> | <span data-ttu-id="910f5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="910f5-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="910f5-110">homePageUrl</span><span class="sxs-lookup"><span data-stu-id="910f5-110">homePageUrl</span></span> | <span data-ttu-id="910f5-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="910f5-111">String</span></span> | <span data-ttu-id="910f5-112">Página inicial ou página de aterrissagem do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="910f5-112">Home page or landing page of the application.</span></span> |
| <span data-ttu-id="910f5-113">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="910f5-113">implicitGrantSettings</span></span> | [<span data-ttu-id="910f5-114">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="910f5-114">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="910f5-115">Especifica se esse aplicativo Web pode solicitar tokens usando o fluxo implícito OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="910f5-115">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> |
| <span data-ttu-id="910f5-116">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="910f5-116">logoutUrl</span></span> | <span data-ttu-id="910f5-117">String</span><span class="sxs-lookup"><span data-stu-id="910f5-117">String</span></span> | <span data-ttu-id="910f5-118">Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML.</span><span class="sxs-lookup"><span data-stu-id="910f5-118">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
| <span data-ttu-id="910f5-119">redirectUris</span><span class="sxs-lookup"><span data-stu-id="910f5-119">redirectUris</span></span> | <span data-ttu-id="910f5-120">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="910f5-120">String collection</span></span> | <span data-ttu-id="910f5-121">Especifica as URLs para as quais os tokens de usuário são enviados para entrar ou as URIs de redirecionamento para as quais os códigos de autorização do OAuth 2.0 e tokens de acesso são enviados.</span><span class="sxs-lookup"><span data-stu-id="910f5-121">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="910f5-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="910f5-122">JSON representation</span></span>
<span data-ttu-id="910f5-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="910f5-123">Here is a JSON representation of the resource.</span></span>

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


