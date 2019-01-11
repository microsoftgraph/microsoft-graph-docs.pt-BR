---
title: Tipo de recurso educationTeacher
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `teacher`.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 612e319699bac9bbb5776f7692d6d6f3b7da3867
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849522"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="12dec-103">Tipo de recurso educationTeacher</span><span class="sxs-lookup"><span data-stu-id="12dec-103">educationTeacher resource type</span></span>

<span data-ttu-id="12dec-104">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `teacher`.</span><span class="sxs-lookup"><span data-stu-id="12dec-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="12dec-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12dec-105">Properties</span></span>
| <span data-ttu-id="12dec-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12dec-106">Property</span></span>     | <span data-ttu-id="12dec-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="12dec-107">Type</span></span>   |<span data-ttu-id="12dec-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="12dec-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12dec-109">externalId</span><span class="sxs-lookup"><span data-stu-id="12dec-109">externalId</span></span>|<span data-ttu-id="12dec-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12dec-110">String</span></span>| <span data-ttu-id="12dec-111">ID do professor no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="12dec-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="12dec-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="12dec-112">teacherNumber</span></span>|<span data-ttu-id="12dec-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12dec-113">String</span></span>|<span data-ttu-id="12dec-114">Número do professor.</span><span class="sxs-lookup"><span data-stu-id="12dec-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12dec-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12dec-115">JSON representation</span></span>

<span data-ttu-id="12dec-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12dec-116">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
