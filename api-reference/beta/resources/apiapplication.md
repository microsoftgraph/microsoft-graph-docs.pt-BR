---
title: tipo de recurso de API
description: Especifica as configurações para um aplicativo da API Web.
localization_priority: Normal
ms.openlocfilehash: f26a568d05c85059e914b355d971755f19627cac
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348332"
---
# <a name="api-resource-type"></a><span data-ttu-id="94dd5-103">tipo de recurso de API</span><span class="sxs-lookup"><span data-stu-id="94dd5-103">api resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94dd5-104">Especifica as configurações para um aplicativo da API Web.</span><span class="sxs-lookup"><span data-stu-id="94dd5-104">Specifies settings for a Web API application.</span></span>

## <a name="properties"></a><span data-ttu-id="94dd5-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94dd5-105">Properties</span></span>

| <span data-ttu-id="94dd5-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94dd5-106">Property</span></span> | <span data-ttu-id="94dd5-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="94dd5-107">Type</span></span> | <span data-ttu-id="94dd5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="94dd5-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="94dd5-109">requestedAccessTokenVersion</span><span class="sxs-lookup"><span data-stu-id="94dd5-109">requestedAccessTokenVersion</span></span>|<span data-ttu-id="94dd5-110">Int32</span><span class="sxs-lookup"><span data-stu-id="94dd5-110">Int32</span></span>| <span data-ttu-id="94dd5-111">Especifica a versão do token de acesso aceito para o recurso de API atual.</span><span class="sxs-lookup"><span data-stu-id="94dd5-111">Specifies the accepted access token version for the current API resource.</span></span> <span data-ttu-id="94dd5-112">Os valores possíveis são 1 ou 2.</span><span class="sxs-lookup"><span data-stu-id="94dd5-112">Possible values are 1 or 2.</span></span>  |
|<span data-ttu-id="94dd5-113">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="94dd5-113">oauth2PermissionScopes</span></span>|<span data-ttu-id="94dd5-114">coleção [permissionScope](permissionscope.md)</span><span class="sxs-lookup"><span data-stu-id="94dd5-114">[permissionScope](permissionscope.md) collection</span></span>| <span data-ttu-id="94dd5-115">A coleção de escopos de permissão OAuth 2,0 que o aplicativo Web API (recurso) expõe para aplicativos cliente.</span><span class="sxs-lookup"><span data-stu-id="94dd5-115">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="94dd5-116">Esses escopos de permissão podem ser concedidos aos aplicativos cliente durante o consentimento.</span><span class="sxs-lookup"><span data-stu-id="94dd5-116">These permission scopes may be granted to client applications during consent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="94dd5-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94dd5-117">JSON representation</span></span>
<span data-ttu-id="94dd5-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94dd5-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.apiApplication"
}-->

```json
{
  "requestedAccessTokenVersion": 1,
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
