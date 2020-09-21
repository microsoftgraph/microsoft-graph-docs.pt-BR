---
title: tipo de recurso educationSynchronizationLicenseAssignment
description: Representa as informações de licença a serem atribuídas às contas de usuário. O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b5aea834ff2943046aff8a390ae110d775fd2f20
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989637"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="ec9ca-104">tipo de recurso educationSynchronizationLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="ec9ca-104">educationSynchronizationLicenseAssignment resource type</span></span>

<span data-ttu-id="ec9ca-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec9ca-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec9ca-106">Representa as informações de licença a serem atribuídas às contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="ec9ca-106">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="ec9ca-107">O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="ec9ca-107">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="ec9ca-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec9ca-108">Properties</span></span>

| <span data-ttu-id="ec9ca-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec9ca-109">Property</span></span>  | <span data-ttu-id="ec9ca-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec9ca-110">Type</span></span>              | <span data-ttu-id="ec9ca-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec9ca-111">Description</span></span>                                                                                    |
| :-------- | :---------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ec9ca-112">appliesTo</span><span class="sxs-lookup"><span data-stu-id="ec9ca-112">appliesTo</span></span> | <span data-ttu-id="ec9ca-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec9ca-113">String</span></span>            | <span data-ttu-id="ec9ca-114">O tipo de função de usuário a ser atribuído à licença.</span><span class="sxs-lookup"><span data-stu-id="ec9ca-114">The user role type to assign to license.</span></span> <span data-ttu-id="ec9ca-115">Os valores possíveis são: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="ec9ca-115">Possible values are: `student`, `teacher`, `faculty`.</span></span> |
| <span data-ttu-id="ec9ca-116">skuIds</span><span class="sxs-lookup"><span data-stu-id="ec9ca-116">skuIds</span></span>    | <span data-ttu-id="ec9ca-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec9ca-117">String collection</span></span> | <span data-ttu-id="ec9ca-118">Representa os identificadores de SKU das licenças a serem atribuídas.</span><span class="sxs-lookup"><span data-stu-id="ec9ca-118">Represents the SKU identifiers of the licenses to assign.</span></span>                                      |

## <a name="json-representation"></a><span data-ttu-id="ec9ca-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec9ca-119">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
  "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
  "skuIds": ["String"]
}
```


