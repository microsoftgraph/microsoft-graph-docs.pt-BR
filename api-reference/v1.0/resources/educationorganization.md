---
title: tipo de recurso de educationOrganization
description: Entidade abstrata usada para modelar o comum entre os tipos de organização diferentes dentro do setor de educação.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 99f3294f76a246e4e78f0f61b0fc1f62532c3a03
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977420"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="63314-103">tipo de recurso de educationOrganization</span><span class="sxs-lookup"><span data-stu-id="63314-103">educationOrganization resource type</span></span>

<span data-ttu-id="63314-104">Entidade abstrata usada para modelar o comum entre os tipos de organização diferentes dentro do setor de educação.</span><span class="sxs-lookup"><span data-stu-id="63314-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="63314-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63314-105">Properties</span></span>
| <span data-ttu-id="63314-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63314-106">Property</span></span>     | <span data-ttu-id="63314-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="63314-107">Type</span></span>   |<span data-ttu-id="63314-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="63314-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63314-109">description</span><span class="sxs-lookup"><span data-stu-id="63314-109">description</span></span>|<span data-ttu-id="63314-110">String</span><span class="sxs-lookup"><span data-stu-id="63314-110">String</span></span>| <span data-ttu-id="63314-111">Descrição da organização.</span><span class="sxs-lookup"><span data-stu-id="63314-111">Organization description.</span></span>|
|<span data-ttu-id="63314-112">displayName</span><span class="sxs-lookup"><span data-stu-id="63314-112">displayName</span></span>|<span data-ttu-id="63314-113">String</span><span class="sxs-lookup"><span data-stu-id="63314-113">String</span></span>| <span data-ttu-id="63314-114">Nome de exibição da organização.</span><span class="sxs-lookup"><span data-stu-id="63314-114">Organization display name.</span></span>|
|<span data-ttu-id="63314-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="63314-115">externalSource</span></span>|<span data-ttu-id="63314-116">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="63314-116">educationExternalSource</span></span>| <span data-ttu-id="63314-117">Fonte local a partir do qual esta organização foi criada.</span><span class="sxs-lookup"><span data-stu-id="63314-117">Source where this organization was created from.</span></span> <span data-ttu-id="63314-118">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="63314-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63314-119">Relações</span><span class="sxs-lookup"><span data-stu-id="63314-119">Relationships</span></span>
<span data-ttu-id="63314-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="63314-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="63314-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63314-121">JSON representation</span></span>

<span data-ttu-id="63314-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="63314-122">The following is a JSON representation of the resource.</span></span>

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
