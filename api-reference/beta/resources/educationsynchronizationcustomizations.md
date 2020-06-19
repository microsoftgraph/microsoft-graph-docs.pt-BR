---
title: tipo de recurso educationSynchronizationCustomizations
description: Contém a lista de entidades a serem sincronizadas e suas personalizações, se houver.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6df720b8f0e02ba24f3972833a6a76219d327925
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790926"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="02222-103">tipo de recurso educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="02222-103">educationSynchronizationCustomizations resource type</span></span>

<span data-ttu-id="02222-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02222-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02222-105">Contém a lista de entidades a serem sincronizadas e suas personalizações, se houver.</span><span class="sxs-lookup"><span data-stu-id="02222-105">Contains the list of entities to sync and their customizations, if any.</span></span>

> [!NOTE]
> <span data-ttu-id="02222-106">A personalização das propriedades a serem sincronizadas não se aplica às registradoras ou às listas de professores do aluno.</span><span class="sxs-lookup"><span data-stu-id="02222-106">Customization of properties to sync does not apply to the Student Enrollments or  Teacher Rosters.</span></span>

<span data-ttu-id="02222-107">Este recurso é membro dos seguintes provedores de dados:</span><span class="sxs-lookup"><span data-stu-id="02222-107">This resource is member of the following data providers:</span></span>

- [<span data-ttu-id="02222-108">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="02222-108">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
- [<span data-ttu-id="02222-109">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="02222-109">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="02222-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="02222-110">Properties</span></span>

| <span data-ttu-id="02222-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02222-111">Property</span></span>          | <span data-ttu-id="02222-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="02222-112">Type</span></span>                                    | <span data-ttu-id="02222-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="02222-113">Description</span></span>                             |
| :---------------- | :-------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="02222-114">escola</span><span class="sxs-lookup"><span data-stu-id="02222-114">school</span></span>            | <span data-ttu-id="02222-115">[educationSynchronizationCustomization]</span><span class="sxs-lookup"><span data-stu-id="02222-115">[educationSynchronizationCustomization]</span></span> | <span data-ttu-id="02222-116">Personalizações para entidades escolares.</span><span class="sxs-lookup"><span data-stu-id="02222-116">Customizations for School entities.</span></span>     |
| <span data-ttu-id="02222-117">section</span><span class="sxs-lookup"><span data-stu-id="02222-117">section</span></span>           | <span data-ttu-id="02222-118">[educationSynchronizationCustomization]</span><span class="sxs-lookup"><span data-stu-id="02222-118">[educationSynchronizationCustomization]</span></span> | <span data-ttu-id="02222-119">Personalizações para entidades de seção.</span><span class="sxs-lookup"><span data-stu-id="02222-119">Customizations for Section entities.</span></span>    |
| <span data-ttu-id="02222-120">student</span><span class="sxs-lookup"><span data-stu-id="02222-120">student</span></span>           | <span data-ttu-id="02222-121">[educationSynchronizationCustomization]</span><span class="sxs-lookup"><span data-stu-id="02222-121">[educationSynchronizationCustomization]</span></span> | <span data-ttu-id="02222-122">Personalizações para entidades de alunos.</span><span class="sxs-lookup"><span data-stu-id="02222-122">Customizations for Student entities.</span></span>    |
| <span data-ttu-id="02222-123">teacher</span><span class="sxs-lookup"><span data-stu-id="02222-123">teacher</span></span>           | <span data-ttu-id="02222-124">[educationSynchronizationCustomization]</span><span class="sxs-lookup"><span data-stu-id="02222-124">[educationSynchronizationCustomization]</span></span> | <span data-ttu-id="02222-125">Personalizações para entidades de professores.</span><span class="sxs-lookup"><span data-stu-id="02222-125">Customizations for Teacher entities.</span></span>    |
| <span data-ttu-id="02222-126">studentEnrollment</span><span class="sxs-lookup"><span data-stu-id="02222-126">studentEnrollment</span></span> | <span data-ttu-id="02222-127">[educationSynchronizationCustomization]</span><span class="sxs-lookup"><span data-stu-id="02222-127">[educationSynchronizationCustomization]</span></span> | <span data-ttu-id="02222-128">Personalizações para o registro de alunos.</span><span class="sxs-lookup"><span data-stu-id="02222-128">Customizations for Student Enrollments.</span></span> |
| <span data-ttu-id="02222-129">teacherRoster</span><span class="sxs-lookup"><span data-stu-id="02222-129">teacherRoster</span></span>     | <span data-ttu-id="02222-130">[educationSynchronizationCustomization]</span><span class="sxs-lookup"><span data-stu-id="02222-130">[educationSynchronizationCustomization]</span></span> | <span data-ttu-id="02222-131">Personalizações para as listas de professores.</span><span class="sxs-lookup"><span data-stu-id="02222-131">Customizations for Teacher Rosters.</span></span>     |

[educationsynchronizationcustomization]: educationsynchronizationcustomization.md

## <a name="json-representation"></a><span data-ttu-id="02222-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="02222-133">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "section": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "studentEnrollment": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "teacherRoster": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  }
}
```
