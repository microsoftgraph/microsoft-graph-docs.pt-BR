---
title: tipo de recurso educationOrganization
description: Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização dentro do setor educacional.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c62e65ffb6c6a0e3a8af92bda6a8b1e1c241ada7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032631"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="e9915-103">tipo de recurso educationOrganization</span><span class="sxs-lookup"><span data-stu-id="e9915-103">educationOrganization resource type</span></span>

<span data-ttu-id="e9915-104">Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização dentro do setor educacional.</span><span class="sxs-lookup"><span data-stu-id="e9915-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="e9915-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e9915-105">Properties</span></span>
| <span data-ttu-id="e9915-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9915-106">Property</span></span>     | <span data-ttu-id="e9915-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9915-107">Type</span></span>   |<span data-ttu-id="e9915-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9915-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9915-109">description</span><span class="sxs-lookup"><span data-stu-id="e9915-109">description</span></span>|<span data-ttu-id="e9915-110">String</span><span class="sxs-lookup"><span data-stu-id="e9915-110">String</span></span>| <span data-ttu-id="e9915-111">Descrição da organização.</span><span class="sxs-lookup"><span data-stu-id="e9915-111">Organization description.</span></span>|
|<span data-ttu-id="e9915-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e9915-112">displayName</span></span>|<span data-ttu-id="e9915-113">String</span><span class="sxs-lookup"><span data-stu-id="e9915-113">String</span></span>| <span data-ttu-id="e9915-114">Nome de exibição da organização.</span><span class="sxs-lookup"><span data-stu-id="e9915-114">Organization display name.</span></span>|
|<span data-ttu-id="e9915-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="e9915-115">externalSource</span></span>|<span data-ttu-id="e9915-116">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="e9915-116">educationExternalSource</span></span>| <span data-ttu-id="e9915-117">Origem de onde esta organização foi criada.</span><span class="sxs-lookup"><span data-stu-id="e9915-117">Source where this organization was created from.</span></span> <span data-ttu-id="e9915-118">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e9915-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9915-119">Relações</span><span class="sxs-lookup"><span data-stu-id="e9915-119">Relationships</span></span>
<span data-ttu-id="e9915-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e9915-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e9915-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e9915-121">JSON representation</span></span>

<span data-ttu-id="e9915-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e9915-122">The following is a JSON representation of the resource.</span></span>

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
