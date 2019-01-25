---
title: tipo de recurso de educationSynchronizationCustomizations
description: Contém a lista de entidades de sincronização e suas personalizações, se houver alguma.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e513e64afb1478ca7b5cc5d53f1964d16d9928b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523250"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="f71ca-103">tipo de recurso de educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="f71ca-103">educationSynchronizationCustomizations resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f71ca-104">Contém a lista de entidades de sincronização e suas [personalizações](educationsynchronizationcustomization.md), se houver alguma.</span><span class="sxs-lookup"><span data-stu-id="f71ca-104">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="f71ca-105">**Observação:** Personalização das propriedades para sincronizar não se aplica às entidades **studentEnrollment** e **teacherRoster** .</span><span class="sxs-lookup"><span data-stu-id="f71ca-105">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="f71ca-106">Este recurso é membro dos provedores de dados a seguir:</span><span class="sxs-lookup"><span data-stu-id="f71ca-106">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="f71ca-107">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="f71ca-107">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="f71ca-108">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="f71ca-108">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="f71ca-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f71ca-109">Properties</span></span>

| <span data-ttu-id="f71ca-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f71ca-110">Property</span></span> | <span data-ttu-id="f71ca-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f71ca-111">Type</span></span> | <span data-ttu-id="f71ca-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f71ca-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="f71ca-113">**escola**</span><span class="sxs-lookup"><span data-stu-id="f71ca-113">**school**</span></span> | [<span data-ttu-id="f71ca-114">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="f71ca-114">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="f71ca-115">Personalização para uma entidade escola.</span><span class="sxs-lookup"><span data-stu-id="f71ca-115">Customization for a school entity.</span></span>        |
| <span data-ttu-id="f71ca-116">**section**</span><span class="sxs-lookup"><span data-stu-id="f71ca-116">**section**</span></span> | [<span data-ttu-id="f71ca-117">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="f71ca-117">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="f71ca-118">Personalização para uma entidade de seção.</span><span class="sxs-lookup"><span data-stu-id="f71ca-118">Customization for a section entity.</span></span>         |
| <span data-ttu-id="f71ca-119">student</span><span class="sxs-lookup"><span data-stu-id="f71ca-119">**student**</span></span> | [<span data-ttu-id="f71ca-120">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="f71ca-120">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="f71ca-121">Personalização para uma entidade de student.</span><span class="sxs-lookup"><span data-stu-id="f71ca-121">Customization for a student entity.</span></span>         |
| <span data-ttu-id="f71ca-122">teacher</span><span class="sxs-lookup"><span data-stu-id="f71ca-122">**teacher**</span></span> | [<span data-ttu-id="f71ca-123">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="f71ca-123">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="f71ca-124">Personalização para uma entidade de professor.</span><span class="sxs-lookup"><span data-stu-id="f71ca-124">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="f71ca-125">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="f71ca-125">**studentEnrollment**</span></span> | [<span data-ttu-id="f71ca-126">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="f71ca-126">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="f71ca-127">Personalização para o registro de student.</span><span class="sxs-lookup"><span data-stu-id="f71ca-127">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="f71ca-128">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="f71ca-128">**teacherRoster**</span></span> | [<span data-ttu-id="f71ca-129">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="f71ca-129">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="f71ca-130">Personalização para uma lista de participação do professor.</span><span class="sxs-lookup"><span data-stu-id="f71ca-130">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="f71ca-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f71ca-131">JSON representation</span></span>
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
