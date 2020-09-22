---
title: tipo de recurso institutionData
description: tipo de recurso institutionData
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a528bf5bc8800b10deed2c45d84613b5ab4bd6b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986060"
---
# <a name="institutiondata-resource-type"></a><span data-ttu-id="eb888-103">tipo de recurso institutionData</span><span class="sxs-lookup"><span data-stu-id="eb888-103">institutionData resource type</span></span>

<span data-ttu-id="eb888-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb888-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb888-105">Representa detalhes adicionais sobre um Undergraduate, graduação, graduação ou outras atividades educacionais que um usuário fez e é usado em um recurso do [educationalActivity](educationalActivity.md) .</span><span class="sxs-lookup"><span data-stu-id="eb888-105">Represents additional detail about an undergraduate, graduate, postgraduate degree or other educational activity that a user has undertaken and is used within an [educationalActivity](educationalActivity.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="eb888-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb888-106">Properties</span></span>

| <span data-ttu-id="eb888-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb888-107">Property</span></span>     | <span data-ttu-id="eb888-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb888-108">Type</span></span>                                 | <span data-ttu-id="eb888-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb888-109">Description</span></span>                                              |
|:-------------|:-------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb888-110">description</span><span class="sxs-lookup"><span data-stu-id="eb888-110">description</span></span>   |<span data-ttu-id="eb888-111">String</span><span class="sxs-lookup"><span data-stu-id="eb888-111">String</span></span>                                |<span data-ttu-id="eb888-112">Descrição resumida da instituição em que o usuário estudou.</span><span class="sxs-lookup"><span data-stu-id="eb888-112">Short description of the institution the user studied at.</span></span> |
|<span data-ttu-id="eb888-113">displayName</span><span class="sxs-lookup"><span data-stu-id="eb888-113">displayName</span></span>   |<span data-ttu-id="eb888-114">String</span><span class="sxs-lookup"><span data-stu-id="eb888-114">String</span></span>                                |<span data-ttu-id="eb888-115">Nome da instituição em que o usuário estudou.</span><span class="sxs-lookup"><span data-stu-id="eb888-115">Name of the institution the user studied at.</span></span>              |
|<span data-ttu-id="eb888-116">localização</span><span class="sxs-lookup"><span data-stu-id="eb888-116">location</span></span>      |[<span data-ttu-id="eb888-117">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="eb888-117">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="eb888-118">Endereço ou local da instituição.</span><span class="sxs-lookup"><span data-stu-id="eb888-118">Address or location of the institute.</span></span>                     |
|<span data-ttu-id="eb888-119">webUrl</span><span class="sxs-lookup"><span data-stu-id="eb888-119">webUrl</span></span>        |<span data-ttu-id="eb888-120">String</span><span class="sxs-lookup"><span data-stu-id="eb888-120">String</span></span>                                |<span data-ttu-id="eb888-121">Link para a instituição ou a home page do departamento.</span><span class="sxs-lookup"><span data-stu-id="eb888-121">Link to the institution or department homepage.</span></span>           |

## <a name="json-representation"></a><span data-ttu-id="eb888-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb888-122">JSON representation</span></span>

<span data-ttu-id="eb888-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb888-123">The following is a JSON representation of the resource.</span></span>

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

