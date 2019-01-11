---
title: tipo de recurso de educationSynchronizationCustomizations
description: Contém a lista de entidades de sincronização e suas personalizações, se houver alguma.
localization_priority: Normal
ms.openlocfilehash: 0c07b166c09b2bfa6bf88159533523dab869a325
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817035"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="60e39-103">tipo de recurso de educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="60e39-103">educationSynchronizationCustomizations resource type</span></span>

> <span data-ttu-id="60e39-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="60e39-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60e39-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="60e39-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="60e39-106">Contém a lista de entidades de sincronização e suas [personalizações](educationsynchronizationcustomization.md), se houver alguma.</span><span class="sxs-lookup"><span data-stu-id="60e39-106">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="60e39-107">**Observação:** Personalização das propriedades para sincronizar não se aplica às entidades **studentEnrollment** e **teacherRoster** .</span><span class="sxs-lookup"><span data-stu-id="60e39-107">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="60e39-108">Este recurso é membro dos provedores de dados a seguir:</span><span class="sxs-lookup"><span data-stu-id="60e39-108">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="60e39-109">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="60e39-109">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="60e39-110">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="60e39-110">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="60e39-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60e39-111">Properties</span></span>

| <span data-ttu-id="60e39-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60e39-112">Property</span></span> | <span data-ttu-id="60e39-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="60e39-113">Type</span></span> | <span data-ttu-id="60e39-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="60e39-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="60e39-115">**escola**</span><span class="sxs-lookup"><span data-stu-id="60e39-115">**school**</span></span> | [<span data-ttu-id="60e39-116">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="60e39-116">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="60e39-117">Personalização para uma entidade escola.</span><span class="sxs-lookup"><span data-stu-id="60e39-117">Customization for a school entity.</span></span>        |
| <span data-ttu-id="60e39-118">**section**</span><span class="sxs-lookup"><span data-stu-id="60e39-118">**section**</span></span> | [<span data-ttu-id="60e39-119">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="60e39-119">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="60e39-120">Personalização para uma entidade de seção.</span><span class="sxs-lookup"><span data-stu-id="60e39-120">Customization for a section entity.</span></span>         |
| <span data-ttu-id="60e39-121">**student**</span><span class="sxs-lookup"><span data-stu-id="60e39-121">**student**</span></span> | [<span data-ttu-id="60e39-122">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="60e39-122">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="60e39-123">Personalização para uma entidade de student.</span><span class="sxs-lookup"><span data-stu-id="60e39-123">Customization for a student entity.</span></span>         |
| <span data-ttu-id="60e39-124">**teacher**</span><span class="sxs-lookup"><span data-stu-id="60e39-124">**teacher**</span></span> | [<span data-ttu-id="60e39-125">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="60e39-125">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="60e39-126">Personalização para uma entidade de professor.</span><span class="sxs-lookup"><span data-stu-id="60e39-126">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="60e39-127">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="60e39-127">**studentEnrollment**</span></span> | [<span data-ttu-id="60e39-128">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="60e39-128">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="60e39-129">Personalização para o registro de student.</span><span class="sxs-lookup"><span data-stu-id="60e39-129">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="60e39-130">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="60e39-130">**teacherRoster**</span></span> | [<span data-ttu-id="60e39-131">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="60e39-131">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="60e39-132">Personalização para uma lista de participação do professor.</span><span class="sxs-lookup"><span data-stu-id="60e39-132">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="60e39-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60e39-133">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomizations"
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
