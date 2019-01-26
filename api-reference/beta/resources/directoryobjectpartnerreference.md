---
title: tipo de recurso de directoryObjectPartnerReference
description: Representa uma referência a um objeto de diretório em um locatário de parceiro. Herda de directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ba72f70a29e778127454ec3bd4f259331d1fe4c5
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570741"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="ea155-104">tipo de recurso de directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="ea155-104">directoryObjectPartnerReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea155-105">Representa uma referência a um objeto de diretório em uma organização parceira.</span><span class="sxs-lookup"><span data-stu-id="ea155-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="ea155-106">Herda de [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="ea155-106">Inherits from [directoryObject](../resources/directoryobject.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ea155-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea155-107">Properties</span></span>

| <span data-ttu-id="ea155-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea155-108">Property</span></span> | <span data-ttu-id="ea155-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea155-109">Type</span></span> | <span data-ttu-id="ea155-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea155-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ea155-111">description</span><span class="sxs-lookup"><span data-stu-id="ea155-111">description</span></span>|<span data-ttu-id="ea155-112">String</span><span class="sxs-lookup"><span data-stu-id="ea155-112">String</span></span>| <span data-ttu-id="ea155-113">Descrição do objeto retornado.</span><span class="sxs-lookup"><span data-stu-id="ea155-113">Description of the object returned.</span></span> <span data-ttu-id="ea155-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea155-114">Read-only.</span></span> |
|<span data-ttu-id="ea155-115">displayName</span><span class="sxs-lookup"><span data-stu-id="ea155-115">displayName</span></span>|<span data-ttu-id="ea155-116">String</span><span class="sxs-lookup"><span data-stu-id="ea155-116">String</span></span>| <span data-ttu-id="ea155-117">Nome do objeto de diretório retornado, como o grupo ou aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea155-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="ea155-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea155-118">Read-only.</span></span> |
|<span data-ttu-id="ea155-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="ea155-119">externalPartnerTenantId</span></span>|<span data-ttu-id="ea155-120">Guid</span><span class="sxs-lookup"><span data-stu-id="ea155-120">Guid</span></span>| <span data-ttu-id="ea155-121">O identificador do locatário para o locatário de parceiro.</span><span class="sxs-lookup"><span data-stu-id="ea155-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="ea155-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea155-122">Read-only.</span></span> |
|<span data-ttu-id="ea155-123">id</span><span class="sxs-lookup"><span data-stu-id="ea155-123">id</span></span>|<span data-ttu-id="ea155-124">String</span><span class="sxs-lookup"><span data-stu-id="ea155-124">String</span></span>| <span data-ttu-id="ea155-125">O identificador exclusivo para o recurso.</span><span class="sxs-lookup"><span data-stu-id="ea155-125">The unique identifier for the resource.</span></span> <span data-ttu-id="ea155-126">Herdado de [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="ea155-126">Inherited from [directoryObject](../resources/directoryobject.md).</span></span> <span data-ttu-id="ea155-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea155-127">Read-only.</span></span> |
|<span data-ttu-id="ea155-128">objectType</span><span class="sxs-lookup"><span data-stu-id="ea155-128">objectType</span></span>|<span data-ttu-id="ea155-129">String</span><span class="sxs-lookup"><span data-stu-id="ea155-129">String</span></span>| <span data-ttu-id="ea155-130">O tipo do objeto referenciado no locatário parceiro.</span><span class="sxs-lookup"><span data-stu-id="ea155-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="ea155-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea155-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ea155-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea155-132">JSON representation</span></span>

<span data-ttu-id="ea155-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea155-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="ea155-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="ea155-134">See also</span></span>

- [<span data-ttu-id="ea155-135">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="ea155-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

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
