---
title: tipo de recurso directoryObjectPartnerReference
description: Representa uma referência a um objeto Directory em um locatário do parceiro. Herda de directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 91d33993ea83ea7eba883534efb513fa80287a64
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340841"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="9048b-104">tipo de recurso directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="9048b-104">directoryObjectPartnerReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9048b-105">Representa uma referência a um objeto Directory em uma organização parceira.</span><span class="sxs-lookup"><span data-stu-id="9048b-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="9048b-106">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="9048b-106">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9048b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9048b-107">Properties</span></span>

| <span data-ttu-id="9048b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9048b-108">Property</span></span> | <span data-ttu-id="9048b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9048b-109">Type</span></span> | <span data-ttu-id="9048b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9048b-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9048b-111">description</span><span class="sxs-lookup"><span data-stu-id="9048b-111">description</span></span>|<span data-ttu-id="9048b-112">String</span><span class="sxs-lookup"><span data-stu-id="9048b-112">String</span></span>| <span data-ttu-id="9048b-113">Descrição do objeto retornado.</span><span class="sxs-lookup"><span data-stu-id="9048b-113">Description of the object returned.</span></span> <span data-ttu-id="9048b-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9048b-114">Read-only.</span></span> |
|<span data-ttu-id="9048b-115">displayName</span><span class="sxs-lookup"><span data-stu-id="9048b-115">displayName</span></span>|<span data-ttu-id="9048b-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9048b-116">String</span></span>| <span data-ttu-id="9048b-117">Nome do objeto de diretório que está sendo retornado, como o grupo ou o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9048b-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="9048b-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9048b-118">Read-only.</span></span> |
|<span data-ttu-id="9048b-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="9048b-119">externalPartnerTenantId</span></span>|<span data-ttu-id="9048b-120">Guid</span><span class="sxs-lookup"><span data-stu-id="9048b-120">Guid</span></span>| <span data-ttu-id="9048b-121">O identificador de locatário para o locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="9048b-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="9048b-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9048b-122">Read-only.</span></span> |
|<span data-ttu-id="9048b-123">id</span><span class="sxs-lookup"><span data-stu-id="9048b-123">id</span></span>|<span data-ttu-id="9048b-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9048b-124">String</span></span>| <span data-ttu-id="9048b-125">O identificador exclusivo do recurso.</span><span class="sxs-lookup"><span data-stu-id="9048b-125">The unique identifier for the resource.</span></span> <span data-ttu-id="9048b-126">Herdado de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="9048b-126">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="9048b-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9048b-127">Read-only.</span></span> |
|<span data-ttu-id="9048b-128">objectType</span><span class="sxs-lookup"><span data-stu-id="9048b-128">objectType</span></span>|<span data-ttu-id="9048b-129">String</span><span class="sxs-lookup"><span data-stu-id="9048b-129">String</span></span>| <span data-ttu-id="9048b-130">O tipo do objeto referenciado no locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="9048b-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="9048b-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9048b-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9048b-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9048b-132">JSON representation</span></span>

<span data-ttu-id="9048b-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9048b-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="9048b-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="9048b-134">See also</span></span>

- [<span data-ttu-id="9048b-135">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="9048b-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
