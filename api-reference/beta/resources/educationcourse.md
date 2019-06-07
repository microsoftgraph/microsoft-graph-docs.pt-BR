---
title: tipo de recurso educationCourse
description: Representa as informações de curso de uma aula.
author: mlafleur
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: eac609f787621e30d4707d477296fc53af77dad0
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764729"
---
# <a name="educationcourse-resource-type"></a><span data-ttu-id="5f5a7-103">tipo de recurso educationCourse</span><span class="sxs-lookup"><span data-stu-id="5f5a7-103">educationCourse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f5a7-104">Representa as informações de curso de uma aula.</span><span class="sxs-lookup"><span data-stu-id="5f5a7-104">Represents the course information for a class.</span></span> <span data-ttu-id="5f5a7-105">É usada dentro de [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="5f5a7-105">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5f5a7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f5a7-106">Properties</span></span>

| <span data-ttu-id="5f5a7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f5a7-107">Property</span></span>     | <span data-ttu-id="5f5a7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f5a7-108">Type</span></span>   | <span data-ttu-id="5f5a7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f5a7-109">Description</span></span>                               |
| :----------- | :----- | :---------------------------------------- |
| <span data-ttu-id="5f5a7-110">courseNumber</span><span class="sxs-lookup"><span data-stu-id="5f5a7-110">courseNumber</span></span> | <span data-ttu-id="5f5a7-111">String</span><span class="sxs-lookup"><span data-stu-id="5f5a7-111">String</span></span> | <span data-ttu-id="5f5a7-112">Identificador exclusivo do curso.</span><span class="sxs-lookup"><span data-stu-id="5f5a7-112">Unique identifier for the course.</span></span>         |
| <span data-ttu-id="5f5a7-113">descrição</span><span class="sxs-lookup"><span data-stu-id="5f5a7-113">description</span></span>  | <span data-ttu-id="5f5a7-114">String</span><span class="sxs-lookup"><span data-stu-id="5f5a7-114">String</span></span> | <span data-ttu-id="5f5a7-115">Descrição do curso.</span><span class="sxs-lookup"><span data-stu-id="5f5a7-115">Description of the course.</span></span>                |
| <span data-ttu-id="5f5a7-116">displayName</span><span class="sxs-lookup"><span data-stu-id="5f5a7-116">displayName</span></span>  | <span data-ttu-id="5f5a7-117">String</span><span class="sxs-lookup"><span data-stu-id="5f5a7-117">String</span></span> | <span data-ttu-id="5f5a7-118">Nome do curso.</span><span class="sxs-lookup"><span data-stu-id="5f5a7-118">Name of the course.</span></span>                       |
| <span data-ttu-id="5f5a7-119">externalId</span><span class="sxs-lookup"><span data-stu-id="5f5a7-119">externalId</span></span>   | <span data-ttu-id="5f5a7-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f5a7-120">String</span></span> | <span data-ttu-id="5f5a7-121">ID do curso do sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="5f5a7-121">ID of the course from the syncing system.</span></span> |
| <span data-ttu-id="5f5a7-122">subject</span><span class="sxs-lookup"><span data-stu-id="5f5a7-122">subject</span></span>      | <span data-ttu-id="5f5a7-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f5a7-123">String</span></span> | <span data-ttu-id="5f5a7-124">Assunto do curso.</span><span class="sxs-lookup"><span data-stu-id="5f5a7-124">Subject of the course.</span></span>                    |

## <a name="json-representation"></a><span data-ttu-id="5f5a7-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f5a7-125">JSON representation</span></span>

<span data-ttu-id="5f5a7-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5f5a7-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCourse"
}-->

```json
{
  "courseNumber": "String",
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationCourse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
