---
title: Tipo de recurso educationTeacher
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `teacher`.
author: mmast-msft
ms.openlocfilehash: a880c3908b70e0b9d7c580492f45183b8f15425d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334458"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="4f7f1-103">Tipo de recurso educationTeacher</span><span class="sxs-lookup"><span data-stu-id="4f7f1-103">educationTeacher resource type</span></span>

<span data-ttu-id="4f7f1-104">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `teacher`.</span><span class="sxs-lookup"><span data-stu-id="4f7f1-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="4f7f1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4f7f1-105">Properties</span></span>
| <span data-ttu-id="4f7f1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f7f1-106">Property</span></span>     | <span data-ttu-id="4f7f1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f7f1-107">Type</span></span>   |<span data-ttu-id="4f7f1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f7f1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f7f1-109">externalId</span><span class="sxs-lookup"><span data-stu-id="4f7f1-109">externalId</span></span>|<span data-ttu-id="4f7f1-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f7f1-110">String</span></span>| <span data-ttu-id="4f7f1-111">ID do professor no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="4f7f1-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="4f7f1-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="4f7f1-112">teacherNumber</span></span>|<span data-ttu-id="4f7f1-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f7f1-113">String</span></span>|<span data-ttu-id="4f7f1-114">Número do professor.</span><span class="sxs-lookup"><span data-stu-id="4f7f1-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f7f1-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4f7f1-115">JSON representation</span></span>

<span data-ttu-id="4f7f1-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4f7f1-116">The following is a JSON representation of the resource.</span></span>

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