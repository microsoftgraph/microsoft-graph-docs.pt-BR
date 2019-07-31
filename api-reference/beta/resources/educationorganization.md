---
title: tipo de recurso educationOrganization
description: 'Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização dentro do setor educacional.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a28577dca488cb11bc6c34c7c653e0db1ede3d4e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972618"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="e660d-103">tipo de recurso educationOrganization</span><span class="sxs-lookup"><span data-stu-id="e660d-103">educationOrganization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e660d-104">Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização dentro do setor educacional.</span><span class="sxs-lookup"><span data-stu-id="e660d-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="e660d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e660d-105">Properties</span></span>
| <span data-ttu-id="e660d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e660d-106">Property</span></span>     | <span data-ttu-id="e660d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e660d-107">Type</span></span>   |<span data-ttu-id="e660d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e660d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e660d-109">description</span><span class="sxs-lookup"><span data-stu-id="e660d-109">description</span></span>|<span data-ttu-id="e660d-110">String</span><span class="sxs-lookup"><span data-stu-id="e660d-110">String</span></span>| <span data-ttu-id="e660d-111">Descrição da organização.</span><span class="sxs-lookup"><span data-stu-id="e660d-111">Organization description.</span></span>|
|<span data-ttu-id="e660d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e660d-112">displayName</span></span>|<span data-ttu-id="e660d-113">String</span><span class="sxs-lookup"><span data-stu-id="e660d-113">String</span></span>| <span data-ttu-id="e660d-114">Nome de exibição da organização.</span><span class="sxs-lookup"><span data-stu-id="e660d-114">Organization display name.</span></span>|
|<span data-ttu-id="e660d-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="e660d-115">externalSource</span></span>|<span data-ttu-id="e660d-116">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e660d-116">string</span></span>| <span data-ttu-id="e660d-117">Origem de onde esta organização foi criada.</span><span class="sxs-lookup"><span data-stu-id="e660d-117">Source where this organization was created from.</span></span> <span data-ttu-id="e660d-118">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e660d-118">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e660d-119">Relações</span><span class="sxs-lookup"><span data-stu-id="e660d-119">Relationships</span></span>
<span data-ttu-id="e660d-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e660d-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e660d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e660d-121">JSON representation</span></span>

<span data-ttu-id="e660d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e660d-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
