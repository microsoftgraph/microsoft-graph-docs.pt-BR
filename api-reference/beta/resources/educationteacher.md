---
title: Tipo de recurso educationTeacher
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `teacher`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2a94eb2c6a1d145c51fef8c35b3b2f9083cf598a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972318"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="16efb-103">Tipo de recurso educationTeacher</span><span class="sxs-lookup"><span data-stu-id="16efb-103">educationTeacher resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16efb-104">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `teacher`.</span><span class="sxs-lookup"><span data-stu-id="16efb-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="16efb-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16efb-105">Properties</span></span>
| <span data-ttu-id="16efb-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16efb-106">Property</span></span>     | <span data-ttu-id="16efb-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="16efb-107">Type</span></span>   |<span data-ttu-id="16efb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="16efb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16efb-109">externalId</span><span class="sxs-lookup"><span data-stu-id="16efb-109">externalId</span></span>|<span data-ttu-id="16efb-110">String</span><span class="sxs-lookup"><span data-stu-id="16efb-110">String</span></span>| <span data-ttu-id="16efb-111">ID do professor no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="16efb-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="16efb-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="16efb-112">teacherNumber</span></span>|<span data-ttu-id="16efb-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16efb-113">String</span></span>|<span data-ttu-id="16efb-114">Número do professor.</span><span class="sxs-lookup"><span data-stu-id="16efb-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16efb-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16efb-115">JSON representation</span></span>

<span data-ttu-id="16efb-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16efb-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
