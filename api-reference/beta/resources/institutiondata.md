---
title: tipo de recurso institutionData
description: tipo de recurso institutionData
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 5724f56a5e68c059126eaac910d34999dcded632
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939450"
---
# <a name="institutiondata-resource-type"></a><span data-ttu-id="9ba55-103">tipo de recurso institutionData</span><span class="sxs-lookup"><span data-stu-id="9ba55-103">institutionData resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ba55-104">Representa detalhes adicionais sobre um Undergraduate, graduação, graduação ou outras atividades educacionais que um usuário fez e é usado em um recurso do [educationalActivity](educationalActivity.md) .</span><span class="sxs-lookup"><span data-stu-id="9ba55-104">Represents additional detail about an undergraduate, graduate, postgraduate degree or other educational activity that a user has undertaken and is used within an [educationalActivity](educationalActivity.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="9ba55-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ba55-105">Properties</span></span>

| <span data-ttu-id="9ba55-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ba55-106">Property</span></span>     | <span data-ttu-id="9ba55-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ba55-107">Type</span></span>                                 | <span data-ttu-id="9ba55-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ba55-108">Description</span></span>                                              |
|:-------------|:-------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ba55-109">description</span><span class="sxs-lookup"><span data-stu-id="9ba55-109">description</span></span>   |<span data-ttu-id="9ba55-110">String</span><span class="sxs-lookup"><span data-stu-id="9ba55-110">String</span></span>                                |<span data-ttu-id="9ba55-111">Descrição resumida da instituição em que o usuário estudou.</span><span class="sxs-lookup"><span data-stu-id="9ba55-111">Short description of the institution the user studied at.</span></span> |
|<span data-ttu-id="9ba55-112">displayName</span><span class="sxs-lookup"><span data-stu-id="9ba55-112">displayName</span></span>   |<span data-ttu-id="9ba55-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ba55-113">String</span></span>                                |<span data-ttu-id="9ba55-114">Nome da instituição em que o usuário estudou.</span><span class="sxs-lookup"><span data-stu-id="9ba55-114">Name of the institution the user studied at.</span></span>              |
|<span data-ttu-id="9ba55-115">location</span><span class="sxs-lookup"><span data-stu-id="9ba55-115">location</span></span>      |[<span data-ttu-id="9ba55-116">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="9ba55-116">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="9ba55-117">Endereço ou local da instituição.</span><span class="sxs-lookup"><span data-stu-id="9ba55-117">Address or location of the institute.</span></span>                     |
|<span data-ttu-id="9ba55-118">webUrl</span><span class="sxs-lookup"><span data-stu-id="9ba55-118">webUrl</span></span>        |<span data-ttu-id="9ba55-119">String</span><span class="sxs-lookup"><span data-stu-id="9ba55-119">String</span></span>                                |<span data-ttu-id="9ba55-120">Link para a instituição ou a home page do departamento.</span><span class="sxs-lookup"><span data-stu-id="9ba55-120">Link to the institution or department homepage.</span></span>           |

## <a name="json-representation"></a><span data-ttu-id="9ba55-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ba55-121">JSON representation</span></span>

<span data-ttu-id="9ba55-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ba55-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.institutionData",
  "baseType": null
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "location": {"@odata.type": "microsoft.graph.physicalAddress"},
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "institutionData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->