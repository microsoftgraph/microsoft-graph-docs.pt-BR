---
title: Tipo de recurso educationCourse
description: Representa as informações do curso para uma classe.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 347eb92cd0b36789cc7ecce1dea72af6985ea330
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232121"
---
# <a name="educationcourse-resource-type"></a><span data-ttu-id="9ddfa-103">Tipo de recurso educationCourse</span><span class="sxs-lookup"><span data-stu-id="9ddfa-103">educationCourse resource type</span></span>

<span data-ttu-id="9ddfa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ddfa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9ddfa-105">Representa as informações do curso para uma classe.</span><span class="sxs-lookup"><span data-stu-id="9ddfa-105">Represents the course information for a class.</span></span> <span data-ttu-id="9ddfa-106">É usada dentro de [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="9ddfa-106">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9ddfa-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ddfa-107">Properties</span></span>

| <span data-ttu-id="9ddfa-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ddfa-108">Property</span></span>     | <span data-ttu-id="9ddfa-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ddfa-109">Type</span></span>   | <span data-ttu-id="9ddfa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ddfa-110">Description</span></span>                               |
| :----------- | :----- | :---------------------------------------- |
| <span data-ttu-id="9ddfa-111">courseNumber</span><span class="sxs-lookup"><span data-stu-id="9ddfa-111">courseNumber</span></span> | <span data-ttu-id="9ddfa-112">String</span><span class="sxs-lookup"><span data-stu-id="9ddfa-112">String</span></span> | <span data-ttu-id="9ddfa-113">Identificador exclusivo do curso.</span><span class="sxs-lookup"><span data-stu-id="9ddfa-113">Unique identifier for the course.</span></span>         |
| <span data-ttu-id="9ddfa-114">descrição</span><span class="sxs-lookup"><span data-stu-id="9ddfa-114">description</span></span>  | <span data-ttu-id="9ddfa-115">String</span><span class="sxs-lookup"><span data-stu-id="9ddfa-115">String</span></span> | <span data-ttu-id="9ddfa-116">Descrição do curso.</span><span class="sxs-lookup"><span data-stu-id="9ddfa-116">Description of the course.</span></span>                |
| <span data-ttu-id="9ddfa-117">displayName</span><span class="sxs-lookup"><span data-stu-id="9ddfa-117">displayName</span></span>  | <span data-ttu-id="9ddfa-118">String</span><span class="sxs-lookup"><span data-stu-id="9ddfa-118">String</span></span> | <span data-ttu-id="9ddfa-119">Nome do curso.</span><span class="sxs-lookup"><span data-stu-id="9ddfa-119">Name of the course.</span></span>                       |
| <span data-ttu-id="9ddfa-120">externalId</span><span class="sxs-lookup"><span data-stu-id="9ddfa-120">externalId</span></span>   | <span data-ttu-id="9ddfa-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ddfa-121">String</span></span> | <span data-ttu-id="9ddfa-122">ID do curso do sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="9ddfa-122">ID of the course from the syncing system.</span></span> |
| <span data-ttu-id="9ddfa-123">Assunto</span><span class="sxs-lookup"><span data-stu-id="9ddfa-123">subject</span></span>      | <span data-ttu-id="9ddfa-124">String</span><span class="sxs-lookup"><span data-stu-id="9ddfa-124">String</span></span> | <span data-ttu-id="9ddfa-125">Assunto do curso.</span><span class="sxs-lookup"><span data-stu-id="9ddfa-125">Subject of the course.</span></span>                    |

## <a name="relationships"></a><span data-ttu-id="9ddfa-126">Relações</span><span class="sxs-lookup"><span data-stu-id="9ddfa-126">Relationships</span></span>

<span data-ttu-id="9ddfa-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ddfa-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ddfa-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ddfa-128">JSON representation</span></span>

<span data-ttu-id="9ddfa-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ddfa-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationCourse"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationCourse",
  "subject": "String",
  "courseNumber": "String",
  "description": "String",
  "displayName": "String",
  "externalId": "String"
}
```
