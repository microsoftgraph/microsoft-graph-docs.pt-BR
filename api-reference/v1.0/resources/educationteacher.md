---
title: Tipo de recurso educationTeacher
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `teacher`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b58d74e6b53b1721a5139d050c7e89197b8721be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929554"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="5fefd-103">Tipo de recurso educationTeacher</span><span class="sxs-lookup"><span data-stu-id="5fefd-103">educationTeacher resource type</span></span>

<span data-ttu-id="5fefd-104">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `teacher`.</span><span class="sxs-lookup"><span data-stu-id="5fefd-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="5fefd-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5fefd-105">Properties</span></span>
| <span data-ttu-id="5fefd-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5fefd-106">Property</span></span>     | <span data-ttu-id="5fefd-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5fefd-107">Type</span></span>   |<span data-ttu-id="5fefd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fefd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5fefd-109">externalId</span><span class="sxs-lookup"><span data-stu-id="5fefd-109">externalId</span></span>|<span data-ttu-id="5fefd-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5fefd-110">String</span></span>| <span data-ttu-id="5fefd-111">ID do professor no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="5fefd-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="5fefd-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="5fefd-112">teacherNumber</span></span>|<span data-ttu-id="5fefd-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5fefd-113">String</span></span>|<span data-ttu-id="5fefd-114">Número do professor.</span><span class="sxs-lookup"><span data-stu-id="5fefd-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5fefd-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5fefd-115">JSON representation</span></span>

<span data-ttu-id="5fefd-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5fefd-116">The following is a JSON representation of the resource.</span></span>

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
