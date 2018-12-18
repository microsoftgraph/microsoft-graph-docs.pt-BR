---
title: tipo de recurso de educationOrganization
description: Entidade abstrata usada para modelar o comum entre os tipos de organização diferentes dentro do setor de educação.
author: mmast-msft
ms.openlocfilehash: e4c0f69d63108cc88b88f530e99cbd55b23f49ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326142"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="e0609-103">tipo de recurso de educationOrganization</span><span class="sxs-lookup"><span data-stu-id="e0609-103">educationOrganization resource type</span></span>

<span data-ttu-id="e0609-104">Entidade abstrata usada para modelar o comum entre os tipos de organização diferentes dentro do setor de educação.</span><span class="sxs-lookup"><span data-stu-id="e0609-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="e0609-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e0609-105">Properties</span></span>
| <span data-ttu-id="e0609-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0609-106">Property</span></span>     | <span data-ttu-id="e0609-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0609-107">Type</span></span>   |<span data-ttu-id="e0609-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0609-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0609-109">description</span><span class="sxs-lookup"><span data-stu-id="e0609-109">description</span></span>|<span data-ttu-id="e0609-110">String</span><span class="sxs-lookup"><span data-stu-id="e0609-110">String</span></span>| <span data-ttu-id="e0609-111">Descrição da organização.</span><span class="sxs-lookup"><span data-stu-id="e0609-111">Organization description.</span></span>|
|<span data-ttu-id="e0609-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e0609-112">displayName</span></span>|<span data-ttu-id="e0609-113">String</span><span class="sxs-lookup"><span data-stu-id="e0609-113">String</span></span>| <span data-ttu-id="e0609-114">Nome de exibição da organização.</span><span class="sxs-lookup"><span data-stu-id="e0609-114">Organization display name.</span></span>|
|<span data-ttu-id="e0609-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="e0609-115">externalSource</span></span>|<span data-ttu-id="e0609-116">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="e0609-116">educationExternalSource</span></span>| <span data-ttu-id="e0609-117">Fonte local a partir do qual esta organização foi criada.</span><span class="sxs-lookup"><span data-stu-id="e0609-117">Source where this organization was created from.</span></span> <span data-ttu-id="e0609-118">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e0609-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0609-119">Relações</span><span class="sxs-lookup"><span data-stu-id="e0609-119">Relationships</span></span>
<span data-ttu-id="e0609-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e0609-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e0609-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e0609-121">JSON representation</span></span>

<span data-ttu-id="e0609-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e0609-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->