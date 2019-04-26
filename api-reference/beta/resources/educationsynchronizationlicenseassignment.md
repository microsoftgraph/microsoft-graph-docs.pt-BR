---
title: tipo de recurso educationSynchronizationLicenseAssignment
description: Representa as informações de licença a serem atribuídas às contas de usuário. O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ae9b89d9fe921967b50b8e290ce29026dbc35ec1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334048"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="c6f52-104">tipo de recurso educationSynchronizationLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="c6f52-104">educationSynchronizationLicenseAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6f52-105">Representa as informações de licença a serem atribuídas às contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="c6f52-105">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="c6f52-106">O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="c6f52-106">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="c6f52-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6f52-107">Properties</span></span>

| <span data-ttu-id="c6f52-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6f52-108">Property</span></span> | <span data-ttu-id="c6f52-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6f52-109">Type</span></span> | <span data-ttu-id="c6f52-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6f52-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="c6f52-111">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="c6f52-111">**appliesTo**</span></span> | <span data-ttu-id="c6f52-112">string</span><span class="sxs-lookup"><span data-stu-id="c6f52-112">string</span></span> | <span data-ttu-id="c6f52-113">O tipo de função de usuário a ser atribuído à licença.</span><span class="sxs-lookup"><span data-stu-id="c6f52-113">The user role type to assign to license.</span></span> <span data-ttu-id="c6f52-114">Os valores possíveis são: `student` e `teacher`.</span><span class="sxs-lookup"><span data-stu-id="c6f52-114">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="c6f52-115">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="c6f52-115">**skuIds**</span></span> | <span data-ttu-id="c6f52-116">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6f52-116">collection of strings</span></span> |  <span data-ttu-id="c6f52-117">Representa os identificadores de SKU das licenças a serem atribuídas.</span><span class="sxs-lookup"><span data-stu-id="c6f52-117">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="c6f52-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6f52-118">JSON representation</span></span>
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
