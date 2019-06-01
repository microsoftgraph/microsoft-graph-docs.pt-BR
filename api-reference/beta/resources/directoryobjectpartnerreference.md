---
title: tipo de recurso directoryObjectPartnerReference
description: Representa uma referência a um objeto Directory em um locatário do parceiro. Herda de directoryObject.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 327528f41795360e0da109b513f3f3f08ac0b268
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657928"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="09cf6-104">tipo de recurso directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="09cf6-104">directoryObjectPartnerReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09cf6-105">Representa uma referência a um objeto Directory em uma organização parceira.</span><span class="sxs-lookup"><span data-stu-id="09cf6-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="09cf6-106">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="09cf6-106">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="properties"></a><span data-ttu-id="09cf6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09cf6-107">Properties</span></span>

| <span data-ttu-id="09cf6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09cf6-108">Property</span></span> | <span data-ttu-id="09cf6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="09cf6-109">Type</span></span> | <span data-ttu-id="09cf6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="09cf6-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="09cf6-111">description</span><span class="sxs-lookup"><span data-stu-id="09cf6-111">description</span></span>|<span data-ttu-id="09cf6-112">String</span><span class="sxs-lookup"><span data-stu-id="09cf6-112">String</span></span>| <span data-ttu-id="09cf6-113">Descrição do objeto retornado.</span><span class="sxs-lookup"><span data-stu-id="09cf6-113">Description of the object returned.</span></span> <span data-ttu-id="09cf6-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="09cf6-114">Read-only.</span></span> |
|<span data-ttu-id="09cf6-115">displayName</span><span class="sxs-lookup"><span data-stu-id="09cf6-115">displayName</span></span>|<span data-ttu-id="09cf6-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09cf6-116">String</span></span>| <span data-ttu-id="09cf6-117">Nome do objeto de diretório que está sendo retornado, como o grupo ou o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="09cf6-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="09cf6-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="09cf6-118">Read-only.</span></span> |
|<span data-ttu-id="09cf6-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="09cf6-119">externalPartnerTenantId</span></span>|<span data-ttu-id="09cf6-120">Guid</span><span class="sxs-lookup"><span data-stu-id="09cf6-120">Guid</span></span>| <span data-ttu-id="09cf6-121">O identificador de locatário para o locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="09cf6-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="09cf6-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="09cf6-122">Read-only.</span></span> |
|<span data-ttu-id="09cf6-123">id</span><span class="sxs-lookup"><span data-stu-id="09cf6-123">id</span></span>|<span data-ttu-id="09cf6-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09cf6-124">String</span></span>| <span data-ttu-id="09cf6-125">O identificador exclusivo do recurso.</span><span class="sxs-lookup"><span data-stu-id="09cf6-125">The unique identifier for the resource.</span></span> <span data-ttu-id="09cf6-126">Herdado de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="09cf6-126">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="09cf6-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="09cf6-127">Read-only.</span></span> |
|<span data-ttu-id="09cf6-128">objectType</span><span class="sxs-lookup"><span data-stu-id="09cf6-128">objectType</span></span>|<span data-ttu-id="09cf6-129">String</span><span class="sxs-lookup"><span data-stu-id="09cf6-129">String</span></span>| <span data-ttu-id="09cf6-130">O tipo do objeto referenciado no locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="09cf6-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="09cf6-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="09cf6-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="09cf6-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09cf6-132">JSON representation</span></span>

<span data-ttu-id="09cf6-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09cf6-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="09cf6-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="09cf6-134">See also</span></span>

- [<span data-ttu-id="09cf6-135">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="09cf6-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

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
