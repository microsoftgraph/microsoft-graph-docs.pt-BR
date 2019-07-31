---
title: tipo de recurso educationSynchronizationLicenseAssignment
description: Representa as informações de licença a serem atribuídas às contas de usuário. O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b00550c1a4d2d02efc983ab345fbc429b443a5bf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972394"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="6fd02-104">tipo de recurso educationSynchronizationLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="6fd02-104">educationSynchronizationLicenseAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fd02-105">Representa as informações de licença a serem atribuídas às contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="6fd02-105">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="6fd02-106">O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="6fd02-106">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="6fd02-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6fd02-107">Properties</span></span>

| <span data-ttu-id="6fd02-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6fd02-108">Property</span></span> | <span data-ttu-id="6fd02-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fd02-109">Type</span></span> | <span data-ttu-id="6fd02-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fd02-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="6fd02-111">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="6fd02-111">**appliesTo**</span></span> | <span data-ttu-id="6fd02-112">string</span><span class="sxs-lookup"><span data-stu-id="6fd02-112">string</span></span> | <span data-ttu-id="6fd02-113">O tipo de função de usuário a ser atribuído à licença.</span><span class="sxs-lookup"><span data-stu-id="6fd02-113">The user role type to assign to license.</span></span> <span data-ttu-id="6fd02-114">Os valores possíveis são: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="6fd02-114">Possible values are: `student`, `teacher`, `faculty`.</span></span>         |
| <span data-ttu-id="6fd02-115">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="6fd02-115">**skuIds**</span></span> | <span data-ttu-id="6fd02-116">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6fd02-116">collection of strings</span></span> |  <span data-ttu-id="6fd02-117">Representa os identificadores de SKU das licenças a serem atribuídas.</span><span class="sxs-lookup"><span data-stu-id="6fd02-117">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="6fd02-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6fd02-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
