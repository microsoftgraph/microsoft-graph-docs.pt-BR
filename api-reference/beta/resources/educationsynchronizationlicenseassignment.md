---
title: tipo de recurso educationSynchronizationLicenseAssignment
description: Representa as informações de licença a serem atribuídas às contas de usuário. O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d5c806b451cc7f757da09927a5732426b0971f2c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500188"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="a60b7-104">tipo de recurso educationSynchronizationLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="a60b7-104">educationSynchronizationLicenseAssignment resource type</span></span>

<span data-ttu-id="a60b7-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a60b7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a60b7-106">Representa as informações de licença a serem atribuídas às contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="a60b7-106">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="a60b7-107">O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="a60b7-107">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="a60b7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a60b7-108">Properties</span></span>

| <span data-ttu-id="a60b7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a60b7-109">Property</span></span> | <span data-ttu-id="a60b7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a60b7-110">Type</span></span> | <span data-ttu-id="a60b7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a60b7-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="a60b7-112">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="a60b7-112">**appliesTo**</span></span> | <span data-ttu-id="a60b7-113">string</span><span class="sxs-lookup"><span data-stu-id="a60b7-113">string</span></span> | <span data-ttu-id="a60b7-114">O tipo de função de usuário a ser atribuído à licença.</span><span class="sxs-lookup"><span data-stu-id="a60b7-114">The user role type to assign to license.</span></span> <span data-ttu-id="a60b7-115">Os valores possíveis são: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="a60b7-115">Possible values are: `student`, `teacher`, `faculty`.</span></span>         |
| <span data-ttu-id="a60b7-116">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="a60b7-116">**skuIds**</span></span> | <span data-ttu-id="a60b7-117">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a60b7-117">collection of strings</span></span> |  <span data-ttu-id="a60b7-118">Representa os identificadores de SKU das licenças a serem atribuídas.</span><span class="sxs-lookup"><span data-stu-id="a60b7-118">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="a60b7-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a60b7-119">JSON representation</span></span>
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
