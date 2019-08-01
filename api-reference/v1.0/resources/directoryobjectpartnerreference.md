---
title: tipo de recurso directoryObjectPartnerReference
description: Representa uma referência a um objeto Directory em um locatário do parceiro. Herda de directoryObject.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7b8fb49ac74d7f1a603f5f0b74d47751242ae01a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029467"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="ca0d8-104">tipo de recurso directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="ca0d8-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="ca0d8-105">Representa uma referência a um objeto Directory em uma organização parceira.</span><span class="sxs-lookup"><span data-stu-id="ca0d8-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="ca0d8-106">Herda de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="ca0d8-106">Inherits from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span>

## <a name="properties"></a><span data-ttu-id="ca0d8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ca0d8-107">Properties</span></span>

| <span data-ttu-id="ca0d8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca0d8-108">Property</span></span> | <span data-ttu-id="ca0d8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca0d8-109">Type</span></span> | <span data-ttu-id="ca0d8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca0d8-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ca0d8-111">description</span><span class="sxs-lookup"><span data-stu-id="ca0d8-111">description</span></span>|<span data-ttu-id="ca0d8-112">String</span><span class="sxs-lookup"><span data-stu-id="ca0d8-112">String</span></span>| <span data-ttu-id="ca0d8-113">Descrição do objeto retornado.</span><span class="sxs-lookup"><span data-stu-id="ca0d8-113">Description of the object returned.</span></span> <span data-ttu-id="ca0d8-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca0d8-114">Read-only.</span></span> |
|<span data-ttu-id="ca0d8-115">displayName</span><span class="sxs-lookup"><span data-stu-id="ca0d8-115">displayName</span></span>|<span data-ttu-id="ca0d8-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca0d8-116">String</span></span>| <span data-ttu-id="ca0d8-117">Nome do objeto de diretório que está sendo retornado, como o grupo ou o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca0d8-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="ca0d8-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca0d8-118">Read-only.</span></span> |
|<span data-ttu-id="ca0d8-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="ca0d8-119">externalPartnerTenantId</span></span>|<span data-ttu-id="ca0d8-120">Guid</span><span class="sxs-lookup"><span data-stu-id="ca0d8-120">Guid</span></span>| <span data-ttu-id="ca0d8-121">O identificador de locatário para o locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="ca0d8-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="ca0d8-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca0d8-122">Read-only.</span></span> |
|<span data-ttu-id="ca0d8-123">id</span><span class="sxs-lookup"><span data-stu-id="ca0d8-123">id</span></span>|<span data-ttu-id="ca0d8-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca0d8-124">String</span></span>| <span data-ttu-id="ca0d8-125">O identificador exclusivo do recurso.</span><span class="sxs-lookup"><span data-stu-id="ca0d8-125">The unique identifier for the resource.</span></span> <span data-ttu-id="ca0d8-126">Herdado de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="ca0d8-126">Inherited from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span> <span data-ttu-id="ca0d8-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca0d8-127">Read-only.</span></span> |
|<span data-ttu-id="ca0d8-128">objectType</span><span class="sxs-lookup"><span data-stu-id="ca0d8-128">objectType</span></span>|<span data-ttu-id="ca0d8-129">String</span><span class="sxs-lookup"><span data-stu-id="ca0d8-129">String</span></span>| <span data-ttu-id="ca0d8-130">O tipo do objeto referenciado no locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="ca0d8-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="ca0d8-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca0d8-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ca0d8-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ca0d8-132">JSON representation</span></span>

<span data-ttu-id="ca0d8-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ca0d8-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="ca0d8-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="ca0d8-134">See also</span></span>

- [<span data-ttu-id="ca0d8-135">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="ca0d8-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-v1.0)

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
