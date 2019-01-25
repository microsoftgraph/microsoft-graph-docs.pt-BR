---
title: Tipo de recurso educationTeacher
description: Informações adicionais incluídas a um `teacher` que está presente quando a primaryRole de um usuário é .
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 17019d5ff5c2bc9614e934ef66d63e459371469a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510852"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="1efb4-103">Tipo de recurso educationTeacher</span><span class="sxs-lookup"><span data-stu-id="1efb4-103">educationTeacher resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1efb4-104">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `teacher`.</span><span class="sxs-lookup"><span data-stu-id="1efb4-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="1efb4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1efb4-105">Properties</span></span>
| <span data-ttu-id="1efb4-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1efb4-106">Property</span></span>     | <span data-ttu-id="1efb4-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1efb4-107">Type</span></span>   |<span data-ttu-id="1efb4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1efb4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1efb4-109">externalId</span><span class="sxs-lookup"><span data-stu-id="1efb4-109">externalId</span></span>|<span data-ttu-id="1efb4-110">String</span><span class="sxs-lookup"><span data-stu-id="1efb4-110">String</span></span>| <span data-ttu-id="1efb4-111">ID do professor no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="1efb4-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="1efb4-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="1efb4-112">teacherNumber</span></span>|<span data-ttu-id="1efb4-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1efb4-113">String</span></span>|<span data-ttu-id="1efb4-114">Número do professor.</span><span class="sxs-lookup"><span data-stu-id="1efb4-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1efb4-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1efb4-115">JSON representation</span></span>

<span data-ttu-id="1efb4-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1efb4-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeacher"
}-->

```json
{
  "externalId": "String",
  "teacherNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationteacher.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
