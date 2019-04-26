---
title: Tipo de recurso educationTeacher
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `teacher`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 092d8fb9d7c358114159428d676ab1a21ea9d091
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333880"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="af093-103">Tipo de recurso educationTeacher</span><span class="sxs-lookup"><span data-stu-id="af093-103">educationTeacher resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af093-104">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `teacher`.</span><span class="sxs-lookup"><span data-stu-id="af093-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="af093-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af093-105">Properties</span></span>
| <span data-ttu-id="af093-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af093-106">Property</span></span>     | <span data-ttu-id="af093-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="af093-107">Type</span></span>   |<span data-ttu-id="af093-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="af093-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af093-109">externalId</span><span class="sxs-lookup"><span data-stu-id="af093-109">externalId</span></span>|<span data-ttu-id="af093-110">String</span><span class="sxs-lookup"><span data-stu-id="af093-110">String</span></span>| <span data-ttu-id="af093-111">ID do professor no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="af093-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="af093-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="af093-112">teacherNumber</span></span>|<span data-ttu-id="af093-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af093-113">String</span></span>|<span data-ttu-id="af093-114">Número do professor.</span><span class="sxs-lookup"><span data-stu-id="af093-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af093-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af093-115">JSON representation</span></span>

<span data-ttu-id="af093-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="af093-116">The following is a JSON representation of the resource.</span></span>

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
