---
title: tipo de recurso de API
description: Especifica as configurações para um aplicativo da API Web.
localization_priority: Normal
ms.openlocfilehash: 9d9259911464feb545b97a9eb8585723a9c3e20e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535687"
---
# <a name="api-resource-type"></a><span data-ttu-id="7ecb7-103">tipo de recurso de API</span><span class="sxs-lookup"><span data-stu-id="7ecb7-103">api resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ecb7-104">Especifica as configurações para um aplicativo da API Web.</span><span class="sxs-lookup"><span data-stu-id="7ecb7-104">Specifies settings for a Web API application.</span></span>

## <a name="properties"></a><span data-ttu-id="7ecb7-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ecb7-105">Properties</span></span>

| <span data-ttu-id="7ecb7-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ecb7-106">Property</span></span> | <span data-ttu-id="7ecb7-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ecb7-107">Type</span></span> | <span data-ttu-id="7ecb7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ecb7-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7ecb7-109">requestedAccessTokenVersion</span><span class="sxs-lookup"><span data-stu-id="7ecb7-109">requestedAccessTokenVersion</span></span>|<span data-ttu-id="7ecb7-110">Int32</span><span class="sxs-lookup"><span data-stu-id="7ecb7-110">Int32</span></span>| <span data-ttu-id="7ecb7-111">Especifica a versão do token de acesso aceito para o recurso de API atual.</span><span class="sxs-lookup"><span data-stu-id="7ecb7-111">Specifies the accepted access token version for the current API resource.</span></span> <span data-ttu-id="7ecb7-112">Os valores possíveis são 1 ou 2.</span><span class="sxs-lookup"><span data-stu-id="7ecb7-112">Possible values are 1 or 2.</span></span>  |
|<span data-ttu-id="7ecb7-113">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="7ecb7-113">oauth2PermissionScopes</span></span>|<span data-ttu-id="7ecb7-114">coleção [permissionScope](permissionscope.md)</span><span class="sxs-lookup"><span data-stu-id="7ecb7-114">[permissionScope](permissionscope.md) collection</span></span>| <span data-ttu-id="7ecb7-115">A coleção de escopos de permissão OAuth 2,0 que o aplicativo Web API (recurso) expõe para aplicativos cliente.</span><span class="sxs-lookup"><span data-stu-id="7ecb7-115">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="7ecb7-116">Esses escopos de permissão podem ser concedidos aos aplicativos cliente durante o consentimento.</span><span class="sxs-lookup"><span data-stu-id="7ecb7-116">These permission scopes may be granted to client applications during consent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7ecb7-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ecb7-117">JSON representation</span></span>
<span data-ttu-id="7ecb7-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ecb7-118">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/api.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
