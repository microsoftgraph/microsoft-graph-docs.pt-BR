---
title: Tipo de recurso educationTeacher
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `teacher`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ad01c29313198b0feab2b4258c9eaafcb9a4f727
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500013"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="f5f26-103">Tipo de recurso educationTeacher</span><span class="sxs-lookup"><span data-stu-id="f5f26-103">educationTeacher resource type</span></span>

<span data-ttu-id="f5f26-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f5f26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5f26-105">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `teacher`.</span><span class="sxs-lookup"><span data-stu-id="f5f26-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="f5f26-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5f26-106">Properties</span></span>
| <span data-ttu-id="f5f26-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5f26-107">Property</span></span>     | <span data-ttu-id="f5f26-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5f26-108">Type</span></span>   |<span data-ttu-id="f5f26-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5f26-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5f26-110">externalId</span><span class="sxs-lookup"><span data-stu-id="f5f26-110">externalId</span></span>|<span data-ttu-id="f5f26-111">String</span><span class="sxs-lookup"><span data-stu-id="f5f26-111">String</span></span>| <span data-ttu-id="f5f26-112">ID do professor no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="f5f26-112">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="f5f26-113">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="f5f26-113">teacherNumber</span></span>|<span data-ttu-id="f5f26-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5f26-114">String</span></span>|<span data-ttu-id="f5f26-115">Número do professor.</span><span class="sxs-lookup"><span data-stu-id="f5f26-115">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5f26-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5f26-116">JSON representation</span></span>

<span data-ttu-id="f5f26-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5f26-117">The following is a JSON representation of the resource.</span></span>

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
