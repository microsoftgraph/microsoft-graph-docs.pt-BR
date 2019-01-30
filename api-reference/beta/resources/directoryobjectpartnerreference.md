---
title: tipo de recurso de directoryObjectPartnerReference
description: Representa uma referência a um objeto de diretório em um locatário de parceiro. Herda do directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a031586d1f92bf2b8b331e9b71058211b4617382
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640305"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="0eec1-104">tipo de recurso de directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="0eec1-104">directoryObjectPartnerReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0eec1-105">Representa uma referência a um objeto de diretório em uma organização parceira.</span><span class="sxs-lookup"><span data-stu-id="0eec1-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="0eec1-106">Herda do [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="0eec1-106">Inherits from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="0eec1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0eec1-107">Properties</span></span>

| <span data-ttu-id="0eec1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0eec1-108">Property</span></span> | <span data-ttu-id="0eec1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0eec1-109">Type</span></span> | <span data-ttu-id="0eec1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0eec1-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0eec1-111">description</span><span class="sxs-lookup"><span data-stu-id="0eec1-111">description</span></span>|<span data-ttu-id="0eec1-112">String</span><span class="sxs-lookup"><span data-stu-id="0eec1-112">String</span></span>| <span data-ttu-id="0eec1-113">Descrição do objeto retornado.</span><span class="sxs-lookup"><span data-stu-id="0eec1-113">Description of the object returned.</span></span> <span data-ttu-id="0eec1-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0eec1-114">Read-only.</span></span> |
|<span data-ttu-id="0eec1-115">displayName</span><span class="sxs-lookup"><span data-stu-id="0eec1-115">displayName</span></span>|<span data-ttu-id="0eec1-116">String</span><span class="sxs-lookup"><span data-stu-id="0eec1-116">String</span></span>| <span data-ttu-id="0eec1-117">Nome do objeto de diretório retornado, como o grupo ou aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0eec1-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="0eec1-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0eec1-118">Read-only.</span></span> |
|<span data-ttu-id="0eec1-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="0eec1-119">externalPartnerTenantId</span></span>|<span data-ttu-id="0eec1-120">Guid</span><span class="sxs-lookup"><span data-stu-id="0eec1-120">Guid</span></span>| <span data-ttu-id="0eec1-121">O identificador do locatário para o locatário de parceiro.</span><span class="sxs-lookup"><span data-stu-id="0eec1-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="0eec1-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0eec1-122">Read-only.</span></span> |
|<span data-ttu-id="0eec1-123">id</span><span class="sxs-lookup"><span data-stu-id="0eec1-123">id</span></span>|<span data-ttu-id="0eec1-124">String</span><span class="sxs-lookup"><span data-stu-id="0eec1-124">String</span></span>| <span data-ttu-id="0eec1-125">O identificador exclusivo para o recurso.</span><span class="sxs-lookup"><span data-stu-id="0eec1-125">The unique identifier for the resource.</span></span> <span data-ttu-id="0eec1-126">Herdado de [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="0eec1-126">Inherited from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span> <span data-ttu-id="0eec1-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0eec1-127">Read-only.</span></span> |
|<span data-ttu-id="0eec1-128">objectType</span><span class="sxs-lookup"><span data-stu-id="0eec1-128">objectType</span></span>|<span data-ttu-id="0eec1-129">String</span><span class="sxs-lookup"><span data-stu-id="0eec1-129">String</span></span>| <span data-ttu-id="0eec1-130">O tipo do objeto referenciado no locatário parceiro.</span><span class="sxs-lookup"><span data-stu-id="0eec1-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="0eec1-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0eec1-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0eec1-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0eec1-132">JSON representation</span></span>

<span data-ttu-id="0eec1-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0eec1-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObjectPartnerReference"
}-->

```json
{
  "description": "string ",
  "displayName": "string",
  "externalPartnerTenantId": "string (identifier)",
  "id": "string (identifier)",
  "objectType": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="0eec1-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="0eec1-134">See also</span></span>

- [<span data-ttu-id="0eec1-135">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="0eec1-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryobjectpartnerreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
