---
title: tipo de recurso directoryObjectPartnerReference
description: Representa uma referência a um objeto Directory em um locatário do parceiro. Herda do directoryObject.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1b9f042f970109a348b637636749778ed95e55e6
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402566"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="67a40-104">tipo de recurso directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="67a40-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="67a40-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67a40-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67a40-106">Representa uma referência a um objeto Directory em uma organização parceira.</span><span class="sxs-lookup"><span data-stu-id="67a40-106">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="67a40-107">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="67a40-107">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="properties"></a><span data-ttu-id="67a40-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="67a40-108">Properties</span></span>

| <span data-ttu-id="67a40-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67a40-109">Property</span></span> | <span data-ttu-id="67a40-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="67a40-110">Type</span></span> | <span data-ttu-id="67a40-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="67a40-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="67a40-112">description</span><span class="sxs-lookup"><span data-stu-id="67a40-112">description</span></span>|<span data-ttu-id="67a40-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67a40-113">String</span></span>| <span data-ttu-id="67a40-114">Descrição do objeto retornado.</span><span class="sxs-lookup"><span data-stu-id="67a40-114">Description of the object returned.</span></span> <span data-ttu-id="67a40-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="67a40-115">Read-only.</span></span> |
|<span data-ttu-id="67a40-116">displayName</span><span class="sxs-lookup"><span data-stu-id="67a40-116">displayName</span></span>|<span data-ttu-id="67a40-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67a40-117">String</span></span>| <span data-ttu-id="67a40-118">Nome do objeto de diretório que está sendo retornado, como o grupo ou o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="67a40-118">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="67a40-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="67a40-119">Read-only.</span></span> |
|<span data-ttu-id="67a40-120">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="67a40-120">externalPartnerTenantId</span></span>|<span data-ttu-id="67a40-121">Guid</span><span class="sxs-lookup"><span data-stu-id="67a40-121">Guid</span></span>| <span data-ttu-id="67a40-122">O identificador de locatário para o locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="67a40-122">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="67a40-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="67a40-123">Read-only.</span></span> |
|<span data-ttu-id="67a40-124">id</span><span class="sxs-lookup"><span data-stu-id="67a40-124">id</span></span>|<span data-ttu-id="67a40-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67a40-125">String</span></span>| <span data-ttu-id="67a40-126">O identificador exclusivo do recurso.</span><span class="sxs-lookup"><span data-stu-id="67a40-126">The unique identifier for the resource.</span></span> <span data-ttu-id="67a40-127">Herdado de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="67a40-127">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="67a40-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="67a40-128">Read-only.</span></span> |
|<span data-ttu-id="67a40-129">objectType</span><span class="sxs-lookup"><span data-stu-id="67a40-129">objectType</span></span>|<span data-ttu-id="67a40-130">String</span><span class="sxs-lookup"><span data-stu-id="67a40-130">String</span></span>| <span data-ttu-id="67a40-131">O tipo do objeto referenciado no locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="67a40-131">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="67a40-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="67a40-132">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="67a40-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="67a40-133">JSON representation</span></span>

<span data-ttu-id="67a40-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="67a40-134">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="67a40-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="67a40-135">See also</span></span>

- [<span data-ttu-id="67a40-136">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="67a40-136">Get directory objects from a list of ids</span></span>](../api/directoryobject-getbyids.md)

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
