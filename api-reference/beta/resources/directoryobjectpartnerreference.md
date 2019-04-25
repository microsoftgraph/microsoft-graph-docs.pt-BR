---
title: tipo de recurso directoryObjectPartnerReference
description: Representa uma referência a um objeto Directory em um locatário do parceiro. Herda de directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a031586d1f92bf2b8b331e9b71058211b4617382
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543270"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="2c9b7-104">tipo de recurso directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="2c9b7-104">directoryObjectPartnerReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c9b7-105">Representa uma referência a um objeto Directory em uma organização parceira.</span><span class="sxs-lookup"><span data-stu-id="2c9b7-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="2c9b7-106">Herda de [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="2c9b7-106">Inherits from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="2c9b7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c9b7-107">Properties</span></span>

| <span data-ttu-id="2c9b7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c9b7-108">Property</span></span> | <span data-ttu-id="2c9b7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c9b7-109">Type</span></span> | <span data-ttu-id="2c9b7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c9b7-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2c9b7-111">description</span><span class="sxs-lookup"><span data-stu-id="2c9b7-111">description</span></span>|<span data-ttu-id="2c9b7-112">String</span><span class="sxs-lookup"><span data-stu-id="2c9b7-112">String</span></span>| <span data-ttu-id="2c9b7-113">Descrição do objeto retornado.</span><span class="sxs-lookup"><span data-stu-id="2c9b7-113">Description of the object returned.</span></span> <span data-ttu-id="2c9b7-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2c9b7-114">Read-only.</span></span> |
|<span data-ttu-id="2c9b7-115">displayName</span><span class="sxs-lookup"><span data-stu-id="2c9b7-115">displayName</span></span>|<span data-ttu-id="2c9b7-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c9b7-116">String</span></span>| <span data-ttu-id="2c9b7-117">Nome do objeto de diretório que está sendo retornado, como o grupo ou o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2c9b7-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="2c9b7-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2c9b7-118">Read-only.</span></span> |
|<span data-ttu-id="2c9b7-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="2c9b7-119">externalPartnerTenantId</span></span>|<span data-ttu-id="2c9b7-120">Guid</span><span class="sxs-lookup"><span data-stu-id="2c9b7-120">Guid</span></span>| <span data-ttu-id="2c9b7-121">O identificador de locatário para o locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="2c9b7-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="2c9b7-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2c9b7-122">Read-only.</span></span> |
|<span data-ttu-id="2c9b7-123">id</span><span class="sxs-lookup"><span data-stu-id="2c9b7-123">id</span></span>|<span data-ttu-id="2c9b7-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c9b7-124">String</span></span>| <span data-ttu-id="2c9b7-125">O identificador exclusivo do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c9b7-125">The unique identifier for the resource.</span></span> <span data-ttu-id="2c9b7-126">Herdado de [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="2c9b7-126">Inherited from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span> <span data-ttu-id="2c9b7-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2c9b7-127">Read-only.</span></span> |
|<span data-ttu-id="2c9b7-128">objectType</span><span class="sxs-lookup"><span data-stu-id="2c9b7-128">objectType</span></span>|<span data-ttu-id="2c9b7-129">String</span><span class="sxs-lookup"><span data-stu-id="2c9b7-129">String</span></span>| <span data-ttu-id="2c9b7-130">O tipo do objeto referenciado no locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="2c9b7-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="2c9b7-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2c9b7-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2c9b7-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c9b7-132">JSON representation</span></span>

<span data-ttu-id="2c9b7-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c9b7-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="2c9b7-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="2c9b7-134">See also</span></span>

- [<span data-ttu-id="2c9b7-135">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="2c9b7-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

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
