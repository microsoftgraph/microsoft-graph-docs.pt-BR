---
title: tipo de recurso de directoryObjectPartnerReference
description: Representa uma referência a um objeto de diretório em um locatário de parceiro. Herda de directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a031586d1f92bf2b8b331e9b71058211b4617382
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511048"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="4e1b4-104">tipo de recurso de directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="4e1b4-104">directoryObjectPartnerReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e1b4-105">Representa uma referência a um objeto de diretório em uma organização parceira.</span><span class="sxs-lookup"><span data-stu-id="4e1b4-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="4e1b4-106">Herda de [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="4e1b4-106">Inherits from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="4e1b4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e1b4-107">Properties</span></span>

| <span data-ttu-id="4e1b4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e1b4-108">Property</span></span> | <span data-ttu-id="4e1b4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e1b4-109">Type</span></span> | <span data-ttu-id="4e1b4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e1b4-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4e1b4-111">description</span><span class="sxs-lookup"><span data-stu-id="4e1b4-111">description</span></span>|<span data-ttu-id="4e1b4-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e1b4-112">String</span></span>| <span data-ttu-id="4e1b4-113">Descrição do objeto retornado.</span><span class="sxs-lookup"><span data-stu-id="4e1b4-113">Description of the object returned.</span></span> <span data-ttu-id="4e1b4-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4e1b4-114">Read-only.</span></span> |
|<span data-ttu-id="4e1b4-115">displayName</span><span class="sxs-lookup"><span data-stu-id="4e1b4-115">displayName</span></span>|<span data-ttu-id="4e1b4-116">String</span><span class="sxs-lookup"><span data-stu-id="4e1b4-116">String</span></span>| <span data-ttu-id="4e1b4-117">Nome do objeto de diretório retornado, como o grupo ou aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4e1b4-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="4e1b4-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4e1b4-118">Read-only.</span></span> |
|<span data-ttu-id="4e1b4-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="4e1b4-119">externalPartnerTenantId</span></span>|<span data-ttu-id="4e1b4-120">Guid</span><span class="sxs-lookup"><span data-stu-id="4e1b4-120">Guid</span></span>| <span data-ttu-id="4e1b4-121">O identificador do locatário para o locatário de parceiro.</span><span class="sxs-lookup"><span data-stu-id="4e1b4-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="4e1b4-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4e1b4-122">Read-only.</span></span> |
|<span data-ttu-id="4e1b4-123">id</span><span class="sxs-lookup"><span data-stu-id="4e1b4-123">id</span></span>|<span data-ttu-id="4e1b4-124">String</span><span class="sxs-lookup"><span data-stu-id="4e1b4-124">String</span></span>| <span data-ttu-id="4e1b4-125">O identificador exclusivo para o recurso.</span><span class="sxs-lookup"><span data-stu-id="4e1b4-125">The unique identifier for the resource.</span></span> <span data-ttu-id="4e1b4-126">Herdado de [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="4e1b4-126">Inherited from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span> <span data-ttu-id="4e1b4-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4e1b4-127">Read-only.</span></span> |
|<span data-ttu-id="4e1b4-128">objectType</span><span class="sxs-lookup"><span data-stu-id="4e1b4-128">objectType</span></span>|<span data-ttu-id="4e1b4-129">String</span><span class="sxs-lookup"><span data-stu-id="4e1b4-129">String</span></span>| <span data-ttu-id="4e1b4-130">O tipo do objeto referenciado no locatário parceiro.</span><span class="sxs-lookup"><span data-stu-id="4e1b4-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="4e1b4-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4e1b4-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4e1b4-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e1b4-132">JSON representation</span></span>

<span data-ttu-id="4e1b4-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e1b4-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="4e1b4-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="4e1b4-134">See also</span></span>

- <span data-ttu-id="4e1b4-135">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="4e1b4-135">[Get directory objects from a list of ids](/graph/api/directoryobject-getbyids?view=graph-rest-beta)</span></span>

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
