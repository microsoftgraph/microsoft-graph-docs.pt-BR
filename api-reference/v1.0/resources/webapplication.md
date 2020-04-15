---
title: tipo de recurso webApplication
description: Especifica configurações para um aplicativo Web.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: fc216874ae2b8e11a1a52443c8d255a936fc5223
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442285"
---
# <a name="webapplication-resource-type"></a><span data-ttu-id="7bb07-103">tipo de recurso webApplication</span><span class="sxs-lookup"><span data-stu-id="7bb07-103">webApplication resource type</span></span>

<span data-ttu-id="7bb07-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bb07-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7bb07-105">Especifica configurações para um aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="7bb07-105">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="7bb07-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7bb07-106">Properties</span></span>

| <span data-ttu-id="7bb07-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bb07-107">Property</span></span> | <span data-ttu-id="7bb07-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bb07-108">Type</span></span> | <span data-ttu-id="7bb07-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bb07-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="7bb07-110">homePageUrl</span><span class="sxs-lookup"><span data-stu-id="7bb07-110">homePageUrl</span></span> | <span data-ttu-id="7bb07-111">String</span><span class="sxs-lookup"><span data-stu-id="7bb07-111">String</span></span> | <span data-ttu-id="7bb07-112">Página inicial ou página de aterrissagem do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7bb07-112">Home page or landing page of the application.</span></span> |
| <span data-ttu-id="7bb07-113">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="7bb07-113">implicitGrantSettings</span></span> | [<span data-ttu-id="7bb07-114">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="7bb07-114">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="7bb07-115">Especifica se este aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="7bb07-115">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> |
| <span data-ttu-id="7bb07-116">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="7bb07-116">logoutUrl</span></span> | <span data-ttu-id="7bb07-117">String</span><span class="sxs-lookup"><span data-stu-id="7bb07-117">String</span></span> | <span data-ttu-id="7bb07-118">Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML.</span><span class="sxs-lookup"><span data-stu-id="7bb07-118">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
| <span data-ttu-id="7bb07-119">redirectUris</span><span class="sxs-lookup"><span data-stu-id="7bb07-119">redirectUris</span></span> | <span data-ttu-id="7bb07-120">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bb07-120">String collection</span></span> | <span data-ttu-id="7bb07-121">Especifica as URLs nas quais os tokens de usuário são enviados para entrada ou os URIs de redirecionamento nos quais os códigos de autorização OAuth 2,0 e tokens de acesso são enviados.</span><span class="sxs-lookup"><span data-stu-id="7bb07-121">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7bb07-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7bb07-122">JSON representation</span></span>
<span data-ttu-id="7bb07-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7bb07-123">Here is a JSON representation of the resource.</span></span>

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
