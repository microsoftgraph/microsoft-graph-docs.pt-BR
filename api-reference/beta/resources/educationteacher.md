---
title: Tipo de recurso educationTeacher
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `teacher`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4cd8b11d5f398177ec301e6cb7d834268e97c005
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909700"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="7ff80-103">Tipo de recurso educationTeacher</span><span class="sxs-lookup"><span data-stu-id="7ff80-103">educationTeacher resource type</span></span>

<span data-ttu-id="7ff80-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ff80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ff80-105">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `teacher`.</span><span class="sxs-lookup"><span data-stu-id="7ff80-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7ff80-106">Ao usar escopos de permissão delegada, o Graph retornará apenas as `externalId` Propriedades.</span><span class="sxs-lookup"><span data-stu-id="7ff80-106">When using Delegated permission scopes, Graph will only return the `externalId` properties.</span></span> <span data-ttu-id="7ff80-107">Todas as outras propriedades exigem escopos de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ff80-107">All other properties require Application scopes.</span></span>

## <a name="properties"></a><span data-ttu-id="7ff80-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ff80-108">Properties</span></span>

| <span data-ttu-id="7ff80-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ff80-109">Property</span></span>      | <span data-ttu-id="7ff80-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ff80-110">Type</span></span>   | <span data-ttu-id="7ff80-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ff80-111">Description</span></span>                                  |
| :------------ | :----- | :------------------------------------------- |
| <span data-ttu-id="7ff80-112">externalId</span><span class="sxs-lookup"><span data-stu-id="7ff80-112">externalId</span></span>    | <span data-ttu-id="7ff80-113">String</span><span class="sxs-lookup"><span data-stu-id="7ff80-113">String</span></span> | <span data-ttu-id="7ff80-114">ID do professor no sistema de origem externo.</span><span class="sxs-lookup"><span data-stu-id="7ff80-114">Id of the Teacher in external source system.</span></span> |
| <span data-ttu-id="7ff80-115">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="7ff80-115">teacherNumber</span></span> | <span data-ttu-id="7ff80-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ff80-116">String</span></span> | <span data-ttu-id="7ff80-117">Número do professor.</span><span class="sxs-lookup"><span data-stu-id="7ff80-117">Teacher number.</span></span>                              |

## <a name="json-representation"></a><span data-ttu-id="7ff80-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ff80-118">JSON representation</span></span>

<span data-ttu-id="7ff80-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ff80-119">The following is a JSON representation of the resource.</span></span>

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
