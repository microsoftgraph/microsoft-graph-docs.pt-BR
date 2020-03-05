---
title: tipo de recurso educationCourse
description: Representa as informações de curso de uma aula.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9ba29e98150db6ffa9938585540d9b77f8a755cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502267"
---
# <a name="educationcourse-resource-type"></a><span data-ttu-id="b4f12-103">tipo de recurso educationCourse</span><span class="sxs-lookup"><span data-stu-id="b4f12-103">educationCourse resource type</span></span>

<span data-ttu-id="b4f12-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b4f12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4f12-105">Representa as informações de curso de uma aula.</span><span class="sxs-lookup"><span data-stu-id="b4f12-105">Represents the course information for a class.</span></span> <span data-ttu-id="b4f12-106">É usada dentro de [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="b4f12-106">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b4f12-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4f12-107">Properties</span></span>

| <span data-ttu-id="b4f12-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4f12-108">Property</span></span>     | <span data-ttu-id="b4f12-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4f12-109">Type</span></span>   | <span data-ttu-id="b4f12-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4f12-110">Description</span></span>                               |
| :----------- | :----- | :---------------------------------------- |
| <span data-ttu-id="b4f12-111">courseNumber</span><span class="sxs-lookup"><span data-stu-id="b4f12-111">courseNumber</span></span> | <span data-ttu-id="b4f12-112">String</span><span class="sxs-lookup"><span data-stu-id="b4f12-112">String</span></span> | <span data-ttu-id="b4f12-113">Identificador exclusivo do curso.</span><span class="sxs-lookup"><span data-stu-id="b4f12-113">Unique identifier for the course.</span></span>         |
| <span data-ttu-id="b4f12-114">description</span><span class="sxs-lookup"><span data-stu-id="b4f12-114">description</span></span>  | <span data-ttu-id="b4f12-115">String</span><span class="sxs-lookup"><span data-stu-id="b4f12-115">String</span></span> | <span data-ttu-id="b4f12-116">Descrição do curso.</span><span class="sxs-lookup"><span data-stu-id="b4f12-116">Description of the course.</span></span>                |
| <span data-ttu-id="b4f12-117">displayName</span><span class="sxs-lookup"><span data-stu-id="b4f12-117">displayName</span></span>  | <span data-ttu-id="b4f12-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4f12-118">String</span></span> | <span data-ttu-id="b4f12-119">Nome do curso.</span><span class="sxs-lookup"><span data-stu-id="b4f12-119">Name of the course.</span></span>                       |
| <span data-ttu-id="b4f12-120">externalId</span><span class="sxs-lookup"><span data-stu-id="b4f12-120">externalId</span></span>   | <span data-ttu-id="b4f12-121">String</span><span class="sxs-lookup"><span data-stu-id="b4f12-121">String</span></span> | <span data-ttu-id="b4f12-122">ID do curso do sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="b4f12-122">ID of the course from the syncing system.</span></span> |
| <span data-ttu-id="b4f12-123">assunto</span><span class="sxs-lookup"><span data-stu-id="b4f12-123">subject</span></span>      | <span data-ttu-id="b4f12-124">String</span><span class="sxs-lookup"><span data-stu-id="b4f12-124">String</span></span> | <span data-ttu-id="b4f12-125">Assunto do curso.</span><span class="sxs-lookup"><span data-stu-id="b4f12-125">Subject of the course.</span></span>                    |

## <a name="json-representation"></a><span data-ttu-id="b4f12-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4f12-126">JSON representation</span></span>

<span data-ttu-id="b4f12-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4f12-127">The following is a JSON representation of the resource.</span></span>

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
