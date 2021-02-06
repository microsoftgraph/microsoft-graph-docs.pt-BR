---
title: Tipo de recurso webApplication
description: Especifica configurações para um aplicativo Web.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 630423c787f8a89734c56362b079a402a5606929
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135611"
---
# <a name="webapplication-resource-type"></a><span data-ttu-id="43fa6-103">Tipo de recurso webApplication</span><span class="sxs-lookup"><span data-stu-id="43fa6-103">webApplication resource type</span></span>

<span data-ttu-id="43fa6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43fa6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43fa6-105">Especifica configurações para um aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="43fa6-105">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="43fa6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43fa6-106">Properties</span></span>

| <span data-ttu-id="43fa6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43fa6-107">Property</span></span> | <span data-ttu-id="43fa6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="43fa6-108">Type</span></span> | <span data-ttu-id="43fa6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="43fa6-109">Description</span></span> |
|:---------|:-----|:------------|
| `homePageUrl` | <span data-ttu-id="43fa6-110">String</span><span class="sxs-lookup"><span data-stu-id="43fa6-110">String</span></span> | <span data-ttu-id="43fa6-111">Página inicial ou página de aterrissagem do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="43fa6-111">Home page or landing page of the application.</span></span> |
| `implicitGrantSettings` | [<span data-ttu-id="43fa6-112">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="43fa6-112">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="43fa6-113">Especifica se esse aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="43fa6-113">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> |
| `logoutUrl` | <span data-ttu-id="43fa6-114">String</span><span class="sxs-lookup"><span data-stu-id="43fa6-114">String</span></span> | <span data-ttu-id="43fa6-115">Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML.</span><span class="sxs-lookup"><span data-stu-id="43fa6-115">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
| `redirectUris` | <span data-ttu-id="43fa6-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="43fa6-116">String collection</span></span> | <span data-ttu-id="43fa6-117">Especifica as URLs para onde os tokens de usuário são enviados para entrada ou os URIs de redirecionamento para os quais os códigos de autorização e tokens de acesso do OAuth 2.0 são enviados.</span><span class="sxs-lookup"><span data-stu-id="43fa6-117">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="43fa6-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43fa6-118">JSON representation</span></span>
<span data-ttu-id="43fa6-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43fa6-119">Here is a JSON representation of the resource.</span></span>

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


