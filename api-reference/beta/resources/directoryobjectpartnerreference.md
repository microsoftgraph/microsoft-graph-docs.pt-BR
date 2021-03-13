---
title: Tipo de recurso directoryObjectPartnerReference
description: Representa uma referência a um objeto de diretório em um locatário parceiro. Herda de directoryObject.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 8b9d6a8826c38171dc7b32c281c371e841906f82
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761553"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="8f6a4-104">Tipo de recurso directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="8f6a4-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="8f6a4-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f6a4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f6a4-106">Representa uma referência a um objeto de diretório em uma organização parceira.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-106">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="8f6a4-107">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="8f6a4-107">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8f6a4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8f6a4-108">Properties</span></span>

| <span data-ttu-id="8f6a4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f6a4-109">Property</span></span> | <span data-ttu-id="8f6a4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f6a4-110">Type</span></span> | <span data-ttu-id="8f6a4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f6a4-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8f6a4-112">description</span><span class="sxs-lookup"><span data-stu-id="8f6a4-112">description</span></span>|<span data-ttu-id="8f6a4-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f6a4-113">String</span></span>| <span data-ttu-id="8f6a4-114">Descrição do objeto retornado.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-114">Description of the object returned.</span></span> <span data-ttu-id="8f6a4-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-115">Read-only.</span></span> |
|<span data-ttu-id="8f6a4-116">displayName</span><span class="sxs-lookup"><span data-stu-id="8f6a4-116">displayName</span></span>|<span data-ttu-id="8f6a4-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f6a4-117">String</span></span>| <span data-ttu-id="8f6a4-118">Nome do objeto de diretório sendo retornado, como grupo ou aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-118">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="8f6a4-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-119">Read-only.</span></span> |
|<span data-ttu-id="8f6a4-120">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="8f6a4-120">externalPartnerTenantId</span></span>|<span data-ttu-id="8f6a4-121">Guid</span><span class="sxs-lookup"><span data-stu-id="8f6a4-121">Guid</span></span>| <span data-ttu-id="8f6a4-122">O identificador de locatário do locatário parceiro.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-122">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="8f6a4-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-123">Read-only.</span></span> |
|<span data-ttu-id="8f6a4-124">id</span><span class="sxs-lookup"><span data-stu-id="8f6a4-124">id</span></span>|<span data-ttu-id="8f6a4-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f6a4-125">String</span></span>| <span data-ttu-id="8f6a4-126">O identificador exclusivo do recurso.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-126">The unique identifier for the resource.</span></span> <span data-ttu-id="8f6a4-127">Herdado de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="8f6a4-127">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="8f6a4-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-128">Read-only.</span></span> |
|<span data-ttu-id="8f6a4-129">objectType</span><span class="sxs-lookup"><span data-stu-id="8f6a4-129">objectType</span></span>|<span data-ttu-id="8f6a4-130">String</span><span class="sxs-lookup"><span data-stu-id="8f6a4-130">String</span></span>| <span data-ttu-id="8f6a4-131">O tipo do objeto referenciado no locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-131">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="8f6a4-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-132">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8f6a4-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f6a4-133">JSON representation</span></span>

<span data-ttu-id="8f6a4-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8f6a4-134">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="8f6a4-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="8f6a4-135">See also</span></span>

- [<span data-ttu-id="8f6a4-136">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="8f6a4-136">Get directory objects from a list of ids</span></span>](../api/directoryobject-getbyids.md)

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
