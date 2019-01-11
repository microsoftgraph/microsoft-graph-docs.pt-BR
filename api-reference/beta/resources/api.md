---
title: tipo de recurso da API
description: Especifica as configurações para um aplicativo Web API.
localization_priority: Normal
ms.openlocfilehash: 50c21c31fec7434514408e1a214c6edf2b838c98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845203"
---
# <a name="api-resource-type"></a><span data-ttu-id="87661-103">tipo de recurso da API</span><span class="sxs-lookup"><span data-stu-id="87661-103">api resource type</span></span>

> <span data-ttu-id="87661-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="87661-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87661-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="87661-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="87661-106">Especifica as configurações para um aplicativo Web API.</span><span class="sxs-lookup"><span data-stu-id="87661-106">Specifies settings for a Web API application.</span></span>

## <a name="properties"></a><span data-ttu-id="87661-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87661-107">Properties</span></span>

| <span data-ttu-id="87661-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87661-108">Property</span></span> | <span data-ttu-id="87661-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="87661-109">Type</span></span> | <span data-ttu-id="87661-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="87661-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="87661-111">requestedAccessTokenVersion</span><span class="sxs-lookup"><span data-stu-id="87661-111">requestedAccessTokenVersion</span></span>|<span data-ttu-id="87661-112">Int32</span><span class="sxs-lookup"><span data-stu-id="87661-112">Int32</span></span>| <span data-ttu-id="87661-113">Especifica a versão de token de acesso aceito para o recurso de API atual.</span><span class="sxs-lookup"><span data-stu-id="87661-113">Specifies the accepted access token version for the current API resource.</span></span> <span data-ttu-id="87661-114">Valores possíveis são 1 ou 2.</span><span class="sxs-lookup"><span data-stu-id="87661-114">Possible values are 1 or 2.</span></span>  |
|<span data-ttu-id="87661-115">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="87661-115">oauth2PermissionScopes</span></span>|<span data-ttu-id="87661-116">coleção [permissionScope](permissionscope.md)</span><span class="sxs-lookup"><span data-stu-id="87661-116">[permissionScope](permissionscope.md) collection</span></span>| <span data-ttu-id="87661-117">A coleção de escopos de permissão OAuth 2.0 que a web application API (recurso) expõe para os aplicativos cliente.</span><span class="sxs-lookup"><span data-stu-id="87661-117">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="87661-118">Estes escopos de permissão podem ser concedidos aos aplicativos de cliente durante o consentimento.</span><span class="sxs-lookup"><span data-stu-id="87661-118">These permission scopes may be granted to client applications during consent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="87661-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87661-119">JSON representation</span></span>
<span data-ttu-id="87661-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87661-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.api"
}-->

```json
{
  "requestedAccessTokenVersion": 1,
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
