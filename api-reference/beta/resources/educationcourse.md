---
title: tipo de recurso educationCourse
description: Representa as informações de curso de uma aula.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 80128524160a5f01806d36f52531383d5ab469a5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095510"
---
# <a name="educationcourse-resource-type"></a><span data-ttu-id="e3c66-103">tipo de recurso educationCourse</span><span class="sxs-lookup"><span data-stu-id="e3c66-103">educationCourse resource type</span></span>

<span data-ttu-id="e3c66-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3c66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3c66-105">Representa as informações de curso de uma aula.</span><span class="sxs-lookup"><span data-stu-id="e3c66-105">Represents the course information for a class.</span></span> <span data-ttu-id="e3c66-106">É usada dentro de [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="e3c66-106">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e3c66-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3c66-107">Properties</span></span>

| <span data-ttu-id="e3c66-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3c66-108">Property</span></span>     | <span data-ttu-id="e3c66-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3c66-109">Type</span></span>   | <span data-ttu-id="e3c66-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3c66-110">Description</span></span>                               |
| :----------- | :----- | :---------------------------------------- |
| <span data-ttu-id="e3c66-111">courseNumber</span><span class="sxs-lookup"><span data-stu-id="e3c66-111">courseNumber</span></span> | <span data-ttu-id="e3c66-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3c66-112">String</span></span> | <span data-ttu-id="e3c66-113">Identificador exclusivo do curso.</span><span class="sxs-lookup"><span data-stu-id="e3c66-113">Unique identifier for the course.</span></span>         |
| <span data-ttu-id="e3c66-114">description</span><span class="sxs-lookup"><span data-stu-id="e3c66-114">description</span></span>  | <span data-ttu-id="e3c66-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3c66-115">String</span></span> | <span data-ttu-id="e3c66-116">Descrição do curso.</span><span class="sxs-lookup"><span data-stu-id="e3c66-116">Description of the course.</span></span>                |
| <span data-ttu-id="e3c66-117">displayName</span><span class="sxs-lookup"><span data-stu-id="e3c66-117">displayName</span></span>  | <span data-ttu-id="e3c66-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3c66-118">String</span></span> | <span data-ttu-id="e3c66-119">Nome do curso.</span><span class="sxs-lookup"><span data-stu-id="e3c66-119">Name of the course.</span></span>                       |
| <span data-ttu-id="e3c66-120">externalId</span><span class="sxs-lookup"><span data-stu-id="e3c66-120">externalId</span></span>   | <span data-ttu-id="e3c66-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3c66-121">String</span></span> | <span data-ttu-id="e3c66-122">ID do curso do sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="e3c66-122">ID of the course from the syncing system.</span></span> |
| <span data-ttu-id="e3c66-123">assunto</span><span class="sxs-lookup"><span data-stu-id="e3c66-123">subject</span></span>      | <span data-ttu-id="e3c66-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3c66-124">String</span></span> | <span data-ttu-id="e3c66-125">Assunto do curso.</span><span class="sxs-lookup"><span data-stu-id="e3c66-125">Subject of the course.</span></span>                    |

## <a name="json-representation"></a><span data-ttu-id="e3c66-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3c66-126">JSON representation</span></span>

<span data-ttu-id="e3c66-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3c66-127">The following is a JSON representation of the resource.</span></span>

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


