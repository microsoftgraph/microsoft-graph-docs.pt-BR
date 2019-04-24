---
title: tipo de recurso de telefone
description: Representa um número de telefone.
localization_priority: Normal
ms.openlocfilehash: 6c34033b0895f81619589e7500441fc655842995
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462533"
---
# <a name="phone-resource-type"></a><span data-ttu-id="898cd-103">tipo de recurso de telefone</span><span class="sxs-lookup"><span data-stu-id="898cd-103">phone resource type</span></span>

<span data-ttu-id="898cd-104">Representa um número de telefone.</span><span class="sxs-lookup"><span data-stu-id="898cd-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="898cd-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="898cd-105">Properties</span></span>
| <span data-ttu-id="898cd-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="898cd-106">Property</span></span>     | <span data-ttu-id="898cd-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="898cd-107">Type</span></span>   |<span data-ttu-id="898cd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="898cd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="898cd-109">number</span><span class="sxs-lookup"><span data-stu-id="898cd-109">number</span></span>|<span data-ttu-id="898cd-110">string</span><span class="sxs-lookup"><span data-stu-id="898cd-110">string</span></span>|<span data-ttu-id="898cd-111">O número de telefone.</span><span class="sxs-lookup"><span data-stu-id="898cd-111">The phone number.</span></span>|
|<span data-ttu-id="898cd-112">type</span><span class="sxs-lookup"><span data-stu-id="898cd-112">type</span></span>|<span data-ttu-id="898cd-113">PhoneType</span><span class="sxs-lookup"><span data-stu-id="898cd-113">phoneType</span></span>|<span data-ttu-id="898cd-114">O tipo de número de telefone.</span><span class="sxs-lookup"><span data-stu-id="898cd-114">The type of phone number.</span></span> <span data-ttu-id="898cd-115">Os valores possíveis são `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="898cd-115">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="898cd-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="898cd-116">JSON representation</span></span>

<span data-ttu-id="898cd-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="898cd-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phone"
}-->

```json
{
  "number": "string",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
