---
title: tipo de recurso educationOrganization
description: Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização dentro do setor educacional.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a6e32f7bf9c635423ca1aace92aea160f6cc2706
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531521"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="b9af4-103">tipo de recurso educationOrganization</span><span class="sxs-lookup"><span data-stu-id="b9af4-103">educationOrganization resource type</span></span>

<span data-ttu-id="b9af4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9af4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9af4-105">Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização dentro do setor educacional.</span><span class="sxs-lookup"><span data-stu-id="b9af4-105">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="b9af4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9af4-106">Properties</span></span>
| <span data-ttu-id="b9af4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9af4-107">Property</span></span>     | <span data-ttu-id="b9af4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9af4-108">Type</span></span>   |<span data-ttu-id="b9af4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9af4-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9af4-110">description</span><span class="sxs-lookup"><span data-stu-id="b9af4-110">description</span></span>|<span data-ttu-id="b9af4-111">String</span><span class="sxs-lookup"><span data-stu-id="b9af4-111">String</span></span>| <span data-ttu-id="b9af4-112">Descrição da organização.</span><span class="sxs-lookup"><span data-stu-id="b9af4-112">Organization description.</span></span>|
|<span data-ttu-id="b9af4-113">displayName</span><span class="sxs-lookup"><span data-stu-id="b9af4-113">displayName</span></span>|<span data-ttu-id="b9af4-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9af4-114">String</span></span>| <span data-ttu-id="b9af4-115">Nome de exibição da organização.</span><span class="sxs-lookup"><span data-stu-id="b9af4-115">Organization display name.</span></span>|
|<span data-ttu-id="b9af4-116">externalSource</span><span class="sxs-lookup"><span data-stu-id="b9af4-116">externalSource</span></span>|<span data-ttu-id="b9af4-117">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="b9af4-117">educationExternalSource</span></span>| <span data-ttu-id="b9af4-118">Origem de onde esta organização foi criada.</span><span class="sxs-lookup"><span data-stu-id="b9af4-118">Source where this organization was created from.</span></span> <span data-ttu-id="b9af4-119">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b9af4-119">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9af4-120">Relações</span><span class="sxs-lookup"><span data-stu-id="b9af4-120">Relationships</span></span>
<span data-ttu-id="b9af4-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9af4-121">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b9af4-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9af4-122">JSON representation</span></span>

<span data-ttu-id="b9af4-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9af4-123">The following is a JSON representation of the resource.</span></span>

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
