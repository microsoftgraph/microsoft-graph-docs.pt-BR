---
title: tipo de recurso educationOrganization
description: 'Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização dentro do setor educacional.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8652e6841c39442d8b9875ea48c785a0275073ef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501483"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="280f0-103">tipo de recurso educationOrganization</span><span class="sxs-lookup"><span data-stu-id="280f0-103">educationOrganization resource type</span></span>

<span data-ttu-id="280f0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="280f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="280f0-105">Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização dentro do setor educacional.</span><span class="sxs-lookup"><span data-stu-id="280f0-105">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="280f0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="280f0-106">Properties</span></span>
| <span data-ttu-id="280f0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="280f0-107">Property</span></span>     | <span data-ttu-id="280f0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="280f0-108">Type</span></span>   |<span data-ttu-id="280f0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="280f0-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="280f0-110">description</span><span class="sxs-lookup"><span data-stu-id="280f0-110">description</span></span>|<span data-ttu-id="280f0-111">String</span><span class="sxs-lookup"><span data-stu-id="280f0-111">String</span></span>| <span data-ttu-id="280f0-112">Descrição da organização.</span><span class="sxs-lookup"><span data-stu-id="280f0-112">Organization description.</span></span>|
|<span data-ttu-id="280f0-113">displayName</span><span class="sxs-lookup"><span data-stu-id="280f0-113">displayName</span></span>|<span data-ttu-id="280f0-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="280f0-114">String</span></span>| <span data-ttu-id="280f0-115">Nome de exibição da organização.</span><span class="sxs-lookup"><span data-stu-id="280f0-115">Organization display name.</span></span>|
|<span data-ttu-id="280f0-116">externalSource</span><span class="sxs-lookup"><span data-stu-id="280f0-116">externalSource</span></span>|<span data-ttu-id="280f0-117">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="280f0-117">string</span></span>| <span data-ttu-id="280f0-118">Origem de onde esta organização foi criada.</span><span class="sxs-lookup"><span data-stu-id="280f0-118">Source where this organization was created from.</span></span> <span data-ttu-id="280f0-119">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="280f0-119">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="280f0-120">Relações</span><span class="sxs-lookup"><span data-stu-id="280f0-120">Relationships</span></span>
<span data-ttu-id="280f0-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="280f0-121">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="280f0-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="280f0-122">JSON representation</span></span>

<span data-ttu-id="280f0-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="280f0-123">The following is a JSON representation of the resource.</span></span>

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
