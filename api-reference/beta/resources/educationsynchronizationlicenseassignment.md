---
title: tipo de recurso de educationSynchronizationLicenseAssignment
description: Representa as informações de licença para atribuir às contas de usuário. O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ce1ae196ba4f014a039e81713119b01fa69e6170
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525819"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="e6c3e-104">tipo de recurso de educationSynchronizationLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="e6c3e-104">educationSynchronizationLicenseAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6c3e-105">Representa as informações de licença para atribuir às contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="e6c3e-105">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="e6c3e-106">O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="e6c3e-106">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="e6c3e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6c3e-107">Properties</span></span>

| <span data-ttu-id="e6c3e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6c3e-108">Property</span></span> | <span data-ttu-id="e6c3e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6c3e-109">Type</span></span> | <span data-ttu-id="e6c3e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6c3e-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="e6c3e-111">appliesTo</span><span class="sxs-lookup"><span data-stu-id="e6c3e-111">**appliesTo**</span></span> | <span data-ttu-id="e6c3e-112">string</span><span class="sxs-lookup"><span data-stu-id="e6c3e-112">string</span></span> | <span data-ttu-id="e6c3e-113">O tipo de função de usuário para atribuir a licença.</span><span class="sxs-lookup"><span data-stu-id="e6c3e-113">The user role type to assign to license.</span></span> <span data-ttu-id="e6c3e-114">Os valores possíveis são: `student` e `teacher`.</span><span class="sxs-lookup"><span data-stu-id="e6c3e-114">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="e6c3e-115">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="e6c3e-115">**skuIds**</span></span> | <span data-ttu-id="e6c3e-116">coleção de sequências de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6c3e-116">collection of strings</span></span> |  <span data-ttu-id="e6c3e-117">Representa os identificadores SKU das licenças para atribuir.</span><span class="sxs-lookup"><span data-stu-id="e6c3e-117">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="e6c3e-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6c3e-118">JSON representation</span></span>
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
