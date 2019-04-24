---
title: tipo de recurso educationSynchronizationLicenseAssignment
description: Representa as informações de licença a serem atribuídas às contas de usuário. O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ce1ae196ba4f014a039e81713119b01fa69e6170
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507093"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="31087-104">tipo de recurso educationSynchronizationLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="31087-104">educationSynchronizationLicenseAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31087-105">Representa as informações de licença a serem atribuídas às contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="31087-105">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="31087-106">O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="31087-106">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="31087-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="31087-107">Properties</span></span>

| <span data-ttu-id="31087-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31087-108">Property</span></span> | <span data-ttu-id="31087-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="31087-109">Type</span></span> | <span data-ttu-id="31087-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="31087-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="31087-111">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="31087-111">**appliesTo**</span></span> | <span data-ttu-id="31087-112">string</span><span class="sxs-lookup"><span data-stu-id="31087-112">string</span></span> | <span data-ttu-id="31087-113">O tipo de função de usuário a ser atribuído à licença.</span><span class="sxs-lookup"><span data-stu-id="31087-113">The user role type to assign to license.</span></span> <span data-ttu-id="31087-114">Os valores possíveis são: `student` e `teacher`.</span><span class="sxs-lookup"><span data-stu-id="31087-114">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="31087-115">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="31087-115">**skuIds**</span></span> | <span data-ttu-id="31087-116">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="31087-116">collection of strings</span></span> |  <span data-ttu-id="31087-117">Representa os identificadores de SKU das licenças a serem atribuídas.</span><span class="sxs-lookup"><span data-stu-id="31087-117">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="31087-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="31087-118">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationlicenseassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
