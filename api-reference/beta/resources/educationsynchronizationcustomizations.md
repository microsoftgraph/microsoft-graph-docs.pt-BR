---
title: tipo de recurso de educationSynchronizationCustomizations
description: Contém a lista de entidades de sincronização e suas personalizações, se houver alguma.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 3254915887afc1e6b0da0b3b6c44b59689219ab1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918186"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="69904-103">tipo de recurso de educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="69904-103">educationSynchronizationCustomizations resource type</span></span>

> <span data-ttu-id="69904-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="69904-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69904-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="69904-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="69904-106">Contém a lista de entidades de sincronização e suas [personalizações](educationsynchronizationcustomization.md), se houver alguma.</span><span class="sxs-lookup"><span data-stu-id="69904-106">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="69904-107">**Observação:** Personalização das propriedades para sincronizar não se aplica às entidades **studentEnrollment** e **teacherRoster** .</span><span class="sxs-lookup"><span data-stu-id="69904-107">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="69904-108">Este recurso é membro dos provedores de dados a seguir:</span><span class="sxs-lookup"><span data-stu-id="69904-108">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="69904-109">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="69904-109">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="69904-110">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="69904-110">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="69904-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69904-111">Properties</span></span>

| <span data-ttu-id="69904-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69904-112">Property</span></span> | <span data-ttu-id="69904-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="69904-113">Type</span></span> | <span data-ttu-id="69904-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="69904-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="69904-115">**escola**</span><span class="sxs-lookup"><span data-stu-id="69904-115">**school**</span></span> | [<span data-ttu-id="69904-116">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="69904-116">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="69904-117">Personalização para uma entidade escola.</span><span class="sxs-lookup"><span data-stu-id="69904-117">Customization for a school entity.</span></span>        |
| <span data-ttu-id="69904-118">**section**</span><span class="sxs-lookup"><span data-stu-id="69904-118">**section**</span></span> | [<span data-ttu-id="69904-119">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="69904-119">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="69904-120">Personalização para uma entidade de seção.</span><span class="sxs-lookup"><span data-stu-id="69904-120">Customization for a section entity.</span></span>         |
| <span data-ttu-id="69904-121">**student**</span><span class="sxs-lookup"><span data-stu-id="69904-121">**student**</span></span> | [<span data-ttu-id="69904-122">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="69904-122">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="69904-123">Personalização para uma entidade de student.</span><span class="sxs-lookup"><span data-stu-id="69904-123">Customization for a student entity.</span></span>         |
| <span data-ttu-id="69904-124">**teacher**</span><span class="sxs-lookup"><span data-stu-id="69904-124">**teacher**</span></span> | [<span data-ttu-id="69904-125">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="69904-125">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="69904-126">Personalização para uma entidade de professor.</span><span class="sxs-lookup"><span data-stu-id="69904-126">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="69904-127">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="69904-127">**studentEnrollment**</span></span> | [<span data-ttu-id="69904-128">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="69904-128">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="69904-129">Personalização para o registro de student.</span><span class="sxs-lookup"><span data-stu-id="69904-129">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="69904-130">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="69904-130">**teacherRoster**</span></span> | [<span data-ttu-id="69904-131">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="69904-131">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="69904-132">Personalização para uma lista de participação do professor.</span><span class="sxs-lookup"><span data-stu-id="69904-132">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="69904-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69904-133">JSON representation</span></span>
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
