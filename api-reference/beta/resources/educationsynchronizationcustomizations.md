---
title: tipo de recurso educationSynchronizationCustomizations
description: Contém a lista de entidades a serem sincronizadas e suas personalizações, se houver.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e513e64afb1478ca7b5cc5d53f1964d16d9928b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543188"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="bacf4-103">tipo de recurso educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="bacf4-103">educationSynchronizationCustomizations resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bacf4-104">Contém a lista de entidades a serem sincronizadas [](educationsynchronizationcustomization.md)e suas personalizações, se houver.</span><span class="sxs-lookup"><span data-stu-id="bacf4-104">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="bacf4-105">**Observação:** A personalização das propriedades a serem sincronizadas não se aplica às entidades **studentEnrollment** e **teacherRoster** .</span><span class="sxs-lookup"><span data-stu-id="bacf4-105">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="bacf4-106">Este recurso é membro dos seguintes provedores de dados:</span><span class="sxs-lookup"><span data-stu-id="bacf4-106">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="bacf4-107">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="bacf4-107">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="bacf4-108">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="bacf4-108">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="bacf4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bacf4-109">Properties</span></span>

| <span data-ttu-id="bacf4-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bacf4-110">Property</span></span> | <span data-ttu-id="bacf4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="bacf4-111">Type</span></span> | <span data-ttu-id="bacf4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="bacf4-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="bacf4-113">**escola**</span><span class="sxs-lookup"><span data-stu-id="bacf4-113">**school**</span></span> | [<span data-ttu-id="bacf4-114">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="bacf4-114">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="bacf4-115">Personalização de uma entidade escolar.</span><span class="sxs-lookup"><span data-stu-id="bacf4-115">Customization for a school entity.</span></span>        |
| <span data-ttu-id="bacf4-116">**section**</span><span class="sxs-lookup"><span data-stu-id="bacf4-116">**section**</span></span> | [<span data-ttu-id="bacf4-117">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="bacf4-117">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="bacf4-118">Personalização de uma entidade de seção.</span><span class="sxs-lookup"><span data-stu-id="bacf4-118">Customization for a section entity.</span></span>         |
| <span data-ttu-id="bacf4-119">**student**</span><span class="sxs-lookup"><span data-stu-id="bacf4-119">**student**</span></span> | [<span data-ttu-id="bacf4-120">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="bacf4-120">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="bacf4-121">Personalização de uma entidade de aluno.</span><span class="sxs-lookup"><span data-stu-id="bacf4-121">Customization for a student entity.</span></span>         |
| <span data-ttu-id="bacf4-122">**teacher**</span><span class="sxs-lookup"><span data-stu-id="bacf4-122">**teacher**</span></span> | [<span data-ttu-id="bacf4-123">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="bacf4-123">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="bacf4-124">Personalização de uma entidade professor.</span><span class="sxs-lookup"><span data-stu-id="bacf4-124">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="bacf4-125">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="bacf4-125">**studentEnrollment**</span></span> | [<span data-ttu-id="bacf4-126">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="bacf4-126">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="bacf4-127">Personalização para registro de alunos.</span><span class="sxs-lookup"><span data-stu-id="bacf4-127">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="bacf4-128">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="bacf4-128">**teacherRoster**</span></span> | [<span data-ttu-id="bacf4-129">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="bacf4-129">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="bacf4-130">Personalização de uma lista de professores.</span><span class="sxs-lookup"><span data-stu-id="bacf4-130">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="bacf4-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bacf4-131">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomizations.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
