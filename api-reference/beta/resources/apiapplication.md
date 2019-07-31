---
title: tipo de recurso de API
description: Especifica as configurações para um aplicativo da API Web.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3bf5ffc21c13e0952efd0f5ea773f76dc3f7b46f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974336"
---
# <a name="api-resource-type"></a><span data-ttu-id="e3580-103">tipo de recurso de API</span><span class="sxs-lookup"><span data-stu-id="e3580-103">api resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3580-104">Especifica as configurações para um aplicativo da API Web.</span><span class="sxs-lookup"><span data-stu-id="e3580-104">Specifies settings for a Web API application.</span></span>

## <a name="properties"></a><span data-ttu-id="e3580-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3580-105">Properties</span></span>

| <span data-ttu-id="e3580-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3580-106">Property</span></span> | <span data-ttu-id="e3580-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3580-107">Type</span></span> | <span data-ttu-id="e3580-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3580-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e3580-109">requestedAccessTokenVersion</span><span class="sxs-lookup"><span data-stu-id="e3580-109">requestedAccessTokenVersion</span></span>|<span data-ttu-id="e3580-110">Int32</span><span class="sxs-lookup"><span data-stu-id="e3580-110">Int32</span></span>| <span data-ttu-id="e3580-111">Especifica a versão do token de acesso aceito para o recurso de API atual.</span><span class="sxs-lookup"><span data-stu-id="e3580-111">Specifies the accepted access token version for the current API resource.</span></span> <span data-ttu-id="e3580-112">Os valores possíveis são 1 ou 2.</span><span class="sxs-lookup"><span data-stu-id="e3580-112">Possible values are 1 or 2.</span></span>  |
|<span data-ttu-id="e3580-113">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="e3580-113">oauth2PermissionScopes</span></span>|<span data-ttu-id="e3580-114">coleção [permissionScope](permissionscope.md)</span><span class="sxs-lookup"><span data-stu-id="e3580-114">[permissionScope](permissionscope.md) collection</span></span>| <span data-ttu-id="e3580-115">A coleção de escopos de permissão OAuth 2,0 que o aplicativo Web API (recurso) expõe para aplicativos cliente.</span><span class="sxs-lookup"><span data-stu-id="e3580-115">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="e3580-116">Esses escopos de permissão podem ser concedidos aos aplicativos cliente durante o consentimento.</span><span class="sxs-lookup"><span data-stu-id="e3580-116">These permission scopes may be granted to client applications during consent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e3580-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3580-117">JSON representation</span></span>
<span data-ttu-id="e3580-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3580-118">Here is a JSON representation of the resource.</span></span>

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
