---
title: tipo de recurso de educationOrganization
description: Entidade abstrata usada para modelar o comum entre os tipos de organização diferentes dentro do setor de educação.
ms.openlocfilehash: ed7a01072fe3adf00cb09082ad17954b9a921083
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004291"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="50276-103">tipo de recurso de educationOrganization</span><span class="sxs-lookup"><span data-stu-id="50276-103">educationOrganization resource type</span></span>

<span data-ttu-id="50276-104">Entidade abstrata usada para modelar o comum entre os tipos de organização diferentes dentro do setor de educação.</span><span class="sxs-lookup"><span data-stu-id="50276-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="50276-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50276-105">Properties</span></span>
| <span data-ttu-id="50276-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50276-106">Property</span></span>     | <span data-ttu-id="50276-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="50276-107">Type</span></span>   |<span data-ttu-id="50276-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="50276-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50276-109">description</span><span class="sxs-lookup"><span data-stu-id="50276-109">description</span></span>|<span data-ttu-id="50276-110">String</span><span class="sxs-lookup"><span data-stu-id="50276-110">String</span></span>| <span data-ttu-id="50276-111">Descrição da organização.</span><span class="sxs-lookup"><span data-stu-id="50276-111">Organization description.</span></span>|
|<span data-ttu-id="50276-112">displayName</span><span class="sxs-lookup"><span data-stu-id="50276-112">displayName</span></span>|<span data-ttu-id="50276-113">String</span><span class="sxs-lookup"><span data-stu-id="50276-113">String</span></span>| <span data-ttu-id="50276-114">Nome de exibição da organização.</span><span class="sxs-lookup"><span data-stu-id="50276-114">Organization display name.</span></span>|
|<span data-ttu-id="50276-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="50276-115">externalSource</span></span>|<span data-ttu-id="50276-116">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="50276-116">educationExternalSource</span></span>| <span data-ttu-id="50276-117">Fonte local a partir do qual esta organização foi criada.</span><span class="sxs-lookup"><span data-stu-id="50276-117">Source where this organization was created from.</span></span> <span data-ttu-id="50276-118">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="50276-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50276-119">Relações</span><span class="sxs-lookup"><span data-stu-id="50276-119">Relationships</span></span>
<span data-ttu-id="50276-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="50276-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="50276-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50276-121">JSON representation</span></span>

<span data-ttu-id="50276-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50276-122">The following is a JSON representation of the resource.</span></span>

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