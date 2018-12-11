---
title: tipo de recurso de directoryObjectPartnerReference
description: Representa uma referência a um objeto de diretório em um locatário de parceiro. Herda de directoryObject.
ms.openlocfilehash: ebdd7380eaa6b59488aca46120339f7175b640fa
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2018
ms.locfileid: "27224124"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="73306-104">tipo de recurso de directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="73306-104">directoryObjectPartnerReference resource type</span></span>

> <span data-ttu-id="73306-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="73306-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73306-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="73306-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73306-107">Representa uma referência a um objeto de diretório em uma organização parceira.</span><span class="sxs-lookup"><span data-stu-id="73306-107">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="73306-108">Herda de [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="73306-108">Inherits from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="73306-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73306-109">Properties</span></span>

| <span data-ttu-id="73306-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73306-110">Property</span></span> | <span data-ttu-id="73306-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="73306-111">Type</span></span> | <span data-ttu-id="73306-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="73306-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="73306-113">description</span><span class="sxs-lookup"><span data-stu-id="73306-113">description</span></span>|<span data-ttu-id="73306-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73306-114">String</span></span>| <span data-ttu-id="73306-115">Descrição do objeto retornado.</span><span class="sxs-lookup"><span data-stu-id="73306-115">Description of the object returned.</span></span> <span data-ttu-id="73306-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73306-116">Read-only.</span></span> |
|<span data-ttu-id="73306-117">displayName</span><span class="sxs-lookup"><span data-stu-id="73306-117">displayName</span></span>|<span data-ttu-id="73306-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73306-118">String</span></span>| <span data-ttu-id="73306-119">Nome do objeto de diretório retornado, como o grupo ou aplicativo.</span><span class="sxs-lookup"><span data-stu-id="73306-119">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="73306-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73306-120">Read-only.</span></span> |
|<span data-ttu-id="73306-121">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="73306-121">externalPartnerTenantId</span></span>|<span data-ttu-id="73306-122">Guid</span><span class="sxs-lookup"><span data-stu-id="73306-122">Guid</span></span>| <span data-ttu-id="73306-123">O identificador do locatário para o locatário de parceiro.</span><span class="sxs-lookup"><span data-stu-id="73306-123">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="73306-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73306-124">Read-only.</span></span> |
|<span data-ttu-id="73306-125">id</span><span class="sxs-lookup"><span data-stu-id="73306-125">id</span></span>|<span data-ttu-id="73306-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73306-126">String</span></span>| <span data-ttu-id="73306-127">O identificador exclusivo para o recurso.</span><span class="sxs-lookup"><span data-stu-id="73306-127">The unique identifier for the resource.</span></span> <span data-ttu-id="73306-128">Herdado de [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="73306-128">Inherited from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span> <span data-ttu-id="73306-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73306-129">Read-only.</span></span> |
|<span data-ttu-id="73306-130">objectType</span><span class="sxs-lookup"><span data-stu-id="73306-130">objectType</span></span>|<span data-ttu-id="73306-131">String</span><span class="sxs-lookup"><span data-stu-id="73306-131">String</span></span>| <span data-ttu-id="73306-132">O tipo do objeto referenciado no locatário parceiro.</span><span class="sxs-lookup"><span data-stu-id="73306-132">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="73306-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73306-133">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="73306-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73306-134">JSON representation</span></span>

<span data-ttu-id="73306-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73306-135">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="73306-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="73306-136">See also</span></span>

- [<span data-ttu-id="73306-137">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="73306-137">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
