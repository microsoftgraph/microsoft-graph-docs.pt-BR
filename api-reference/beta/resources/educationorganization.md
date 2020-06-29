---
title: tipo de recurso educationOrganization
description: 'Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização dentro do setor educacional.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 015b1c886f439e3c5952d1c1a5fcce02fb21773b
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909650"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="7a34c-103">tipo de recurso educationOrganization</span><span class="sxs-lookup"><span data-stu-id="7a34c-103">educationOrganization resource type</span></span>

<span data-ttu-id="7a34c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a34c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a34c-105">Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização dentro do setor educacional.</span><span class="sxs-lookup"><span data-stu-id="7a34c-105">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="7a34c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a34c-106">Properties</span></span>

| <span data-ttu-id="7a34c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a34c-107">Property</span></span>       | <span data-ttu-id="7a34c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a34c-108">Type</span></span>   | <span data-ttu-id="7a34c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a34c-109">Description</span></span>                                                                       |
| :------------- | :----- | :-------------------------------------------------------------------------------- |
| <span data-ttu-id="7a34c-110">description</span><span class="sxs-lookup"><span data-stu-id="7a34c-110">description</span></span>    | <span data-ttu-id="7a34c-111">String</span><span class="sxs-lookup"><span data-stu-id="7a34c-111">String</span></span> | <span data-ttu-id="7a34c-112">Descrição da organização.</span><span class="sxs-lookup"><span data-stu-id="7a34c-112">Organization description.</span></span>                                                         |
| <span data-ttu-id="7a34c-113">displayName</span><span class="sxs-lookup"><span data-stu-id="7a34c-113">displayName</span></span>    | <span data-ttu-id="7a34c-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a34c-114">String</span></span> | <span data-ttu-id="7a34c-115">Nome de exibição da organização.</span><span class="sxs-lookup"><span data-stu-id="7a34c-115">Organization display name.</span></span>                                                        |
| <span data-ttu-id="7a34c-116">externalSource</span><span class="sxs-lookup"><span data-stu-id="7a34c-116">externalSource</span></span> | <span data-ttu-id="7a34c-117">String</span><span class="sxs-lookup"><span data-stu-id="7a34c-117">String</span></span> | <span data-ttu-id="7a34c-118">De onde esse usuário foi criado.</span><span class="sxs-lookup"><span data-stu-id="7a34c-118">Where this user was created from.</span></span> <span data-ttu-id="7a34c-119">Os valores possíveis são: `sis` , `lms` , ou `manual` .</span><span class="sxs-lookup"><span data-stu-id="7a34c-119">Possible values are: `sis`, `lms`, or `manual`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7a34c-120">Relações</span><span class="sxs-lookup"><span data-stu-id="7a34c-120">Relationships</span></span>

<span data-ttu-id="7a34c-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7a34c-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a34c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a34c-122">JSON representation</span></span>

<span data-ttu-id="7a34c-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a34c-123">The following is a JSON representation of the resource.</span></span>

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
