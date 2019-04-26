---
title: tipo de recurso educationOrganization
description: Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização dentro do setor educacional.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 99f3294f76a246e4e78f0f61b0fc1f62532c3a03
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562801"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="a47f5-103">tipo de recurso educationOrganization</span><span class="sxs-lookup"><span data-stu-id="a47f5-103">educationOrganization resource type</span></span>

<span data-ttu-id="a47f5-104">Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização dentro do setor educacional.</span><span class="sxs-lookup"><span data-stu-id="a47f5-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="a47f5-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a47f5-105">Properties</span></span>
| <span data-ttu-id="a47f5-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a47f5-106">Property</span></span>     | <span data-ttu-id="a47f5-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a47f5-107">Type</span></span>   |<span data-ttu-id="a47f5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a47f5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a47f5-109">description</span><span class="sxs-lookup"><span data-stu-id="a47f5-109">description</span></span>|<span data-ttu-id="a47f5-110">String</span><span class="sxs-lookup"><span data-stu-id="a47f5-110">String</span></span>| <span data-ttu-id="a47f5-111">Descrição da organização.</span><span class="sxs-lookup"><span data-stu-id="a47f5-111">Organization description.</span></span>|
|<span data-ttu-id="a47f5-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a47f5-112">displayName</span></span>|<span data-ttu-id="a47f5-113">String</span><span class="sxs-lookup"><span data-stu-id="a47f5-113">String</span></span>| <span data-ttu-id="a47f5-114">Nome de exibição da organização.</span><span class="sxs-lookup"><span data-stu-id="a47f5-114">Organization display name.</span></span>|
|<span data-ttu-id="a47f5-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="a47f5-115">externalSource</span></span>|<span data-ttu-id="a47f5-116">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="a47f5-116">educationExternalSource</span></span>| <span data-ttu-id="a47f5-117">Origem de onde esta organização foi criada.</span><span class="sxs-lookup"><span data-stu-id="a47f5-117">Source where this organization was created from.</span></span> <span data-ttu-id="a47f5-118">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a47f5-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a47f5-119">Relações</span><span class="sxs-lookup"><span data-stu-id="a47f5-119">Relationships</span></span>
<span data-ttu-id="a47f5-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a47f5-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a47f5-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a47f5-121">JSON representation</span></span>

<span data-ttu-id="a47f5-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a47f5-122">The following is a JSON representation of the resource.</span></span>

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
