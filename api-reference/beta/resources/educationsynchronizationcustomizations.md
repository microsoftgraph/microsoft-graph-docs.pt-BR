---
title: tipo de recurso educationSynchronizationCustomizations
description: Contém a lista de entidades a serem sincronizadas e suas personalizações, se houver.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d31be9bd808f411c1e208ab953784fdefd65fdda
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972436"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="b9c88-103">tipo de recurso educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="b9c88-103">educationSynchronizationCustomizations resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9c88-104">Contém a lista de entidades a serem sincronizadas [](educationsynchronizationcustomization.md)e suas personalizações, se houver.</span><span class="sxs-lookup"><span data-stu-id="b9c88-104">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="b9c88-105">**Observação:** A personalização das propriedades a serem sincronizadas não se aplica às entidades **studentEnrollment** e **teacherRoster** .</span><span class="sxs-lookup"><span data-stu-id="b9c88-105">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="b9c88-106">Este recurso é membro dos seguintes provedores de dados:</span><span class="sxs-lookup"><span data-stu-id="b9c88-106">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="b9c88-107">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="b9c88-107">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="b9c88-108">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="b9c88-108">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="b9c88-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9c88-109">Properties</span></span>

| <span data-ttu-id="b9c88-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9c88-110">Property</span></span> | <span data-ttu-id="b9c88-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9c88-111">Type</span></span> | <span data-ttu-id="b9c88-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9c88-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b9c88-113">**escola**</span><span class="sxs-lookup"><span data-stu-id="b9c88-113">**school**</span></span> | [<span data-ttu-id="b9c88-114">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="b9c88-114">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="b9c88-115">Personalização de uma entidade escolar.</span><span class="sxs-lookup"><span data-stu-id="b9c88-115">Customization for a school entity.</span></span>        |
| <span data-ttu-id="b9c88-116">**section**</span><span class="sxs-lookup"><span data-stu-id="b9c88-116">**section**</span></span> | [<span data-ttu-id="b9c88-117">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="b9c88-117">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="b9c88-118">Personalização de uma entidade de seção.</span><span class="sxs-lookup"><span data-stu-id="b9c88-118">Customization for a section entity.</span></span>         |
| <span data-ttu-id="b9c88-119">**student**</span><span class="sxs-lookup"><span data-stu-id="b9c88-119">**student**</span></span> | [<span data-ttu-id="b9c88-120">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="b9c88-120">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="b9c88-121">Personalização de uma entidade de aluno.</span><span class="sxs-lookup"><span data-stu-id="b9c88-121">Customization for a student entity.</span></span>         |
| <span data-ttu-id="b9c88-122">**teacher**</span><span class="sxs-lookup"><span data-stu-id="b9c88-122">**teacher**</span></span> | [<span data-ttu-id="b9c88-123">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="b9c88-123">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="b9c88-124">Personalização de uma entidade professor.</span><span class="sxs-lookup"><span data-stu-id="b9c88-124">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="b9c88-125">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="b9c88-125">**studentEnrollment**</span></span> | [<span data-ttu-id="b9c88-126">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="b9c88-126">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="b9c88-127">Personalização para registro de alunos.</span><span class="sxs-lookup"><span data-stu-id="b9c88-127">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="b9c88-128">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="b9c88-128">**teacherRoster**</span></span> | [<span data-ttu-id="b9c88-129">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="b9c88-129">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="b9c88-130">Personalização de uma lista de professores.</span><span class="sxs-lookup"><span data-stu-id="b9c88-130">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="b9c88-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9c88-131">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "section": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "student": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacher": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "studentEnrollment": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacherRoster": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"}
}
```
