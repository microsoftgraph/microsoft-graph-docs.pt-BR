---
title: Tipo de recurso educationTeacher
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `teacher`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 494fc0d3bed992a8df4921fe8601024e7eb01668
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533004"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="6896c-103">Tipo de recurso educationTeacher</span><span class="sxs-lookup"><span data-stu-id="6896c-103">educationTeacher resource type</span></span>

<span data-ttu-id="6896c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6896c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6896c-105">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `teacher`.</span><span class="sxs-lookup"><span data-stu-id="6896c-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="6896c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6896c-106">Properties</span></span>
| <span data-ttu-id="6896c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6896c-107">Property</span></span>     | <span data-ttu-id="6896c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6896c-108">Type</span></span>   |<span data-ttu-id="6896c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6896c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6896c-110">externalId</span><span class="sxs-lookup"><span data-stu-id="6896c-110">externalId</span></span>|<span data-ttu-id="6896c-111">String</span><span class="sxs-lookup"><span data-stu-id="6896c-111">String</span></span>| <span data-ttu-id="6896c-112">ID do professor no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="6896c-112">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="6896c-113">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="6896c-113">teacherNumber</span></span>|<span data-ttu-id="6896c-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6896c-114">String</span></span>|<span data-ttu-id="6896c-115">Número do professor.</span><span class="sxs-lookup"><span data-stu-id="6896c-115">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6896c-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6896c-116">JSON representation</span></span>

<span data-ttu-id="6896c-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6896c-117">The following is a JSON representation of the resource.</span></span>

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
