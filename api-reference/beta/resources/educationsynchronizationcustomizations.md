---
title: tipo de recurso de educationSynchronizationCustomizations
description: Contém a lista de entidades de sincronização e suas personalizações, se houver alguma.
ms.openlocfilehash: d694c5ea1136d38e11ff3f1aca0ad0fde34b9d02
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037405"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="622e6-103">tipo de recurso de educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="622e6-103">educationSynchronizationCustomizations resource type</span></span>

> <span data-ttu-id="622e6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="622e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="622e6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="622e6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="622e6-106">Contém a lista de entidades de sincronização e suas [personalizações](educationsynchronizationcustomization.md), se houver alguma.</span><span class="sxs-lookup"><span data-stu-id="622e6-106">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="622e6-107">**Observação:** Personalização das propriedades para sincronizar não se aplica às entidades **studentEnrollment** e **teacherRoster** .</span><span class="sxs-lookup"><span data-stu-id="622e6-107">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="622e6-108">Este recurso é membro dos provedores de dados a seguir:</span><span class="sxs-lookup"><span data-stu-id="622e6-108">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="622e6-109">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="622e6-109">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="622e6-110">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="622e6-110">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="622e6-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="622e6-111">Properties</span></span>

| <span data-ttu-id="622e6-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="622e6-112">Property</span></span> | <span data-ttu-id="622e6-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="622e6-113">Type</span></span> | <span data-ttu-id="622e6-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="622e6-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="622e6-115">**escola**</span><span class="sxs-lookup"><span data-stu-id="622e6-115">**school**</span></span> | [<span data-ttu-id="622e6-116">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="622e6-116">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="622e6-117">Personalização para uma entidade escola.</span><span class="sxs-lookup"><span data-stu-id="622e6-117">Customization for a school entity.</span></span>        |
| <span data-ttu-id="622e6-118">**section**</span><span class="sxs-lookup"><span data-stu-id="622e6-118">**section**</span></span> | [<span data-ttu-id="622e6-119">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="622e6-119">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="622e6-120">Personalização para uma entidade de seção.</span><span class="sxs-lookup"><span data-stu-id="622e6-120">Customization for a section entity.</span></span>         |
| <span data-ttu-id="622e6-121">**student**</span><span class="sxs-lookup"><span data-stu-id="622e6-121">**student**</span></span> | [<span data-ttu-id="622e6-122">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="622e6-122">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="622e6-123">Personalização para uma entidade de student.</span><span class="sxs-lookup"><span data-stu-id="622e6-123">Customization for a student entity.</span></span>         |
| <span data-ttu-id="622e6-124">**teacher**</span><span class="sxs-lookup"><span data-stu-id="622e6-124">**teacher**</span></span> | [<span data-ttu-id="622e6-125">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="622e6-125">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="622e6-126">Personalização para uma entidade de professor.</span><span class="sxs-lookup"><span data-stu-id="622e6-126">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="622e6-127">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="622e6-127">**studentEnrollment**</span></span> | [<span data-ttu-id="622e6-128">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="622e6-128">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="622e6-129">Personalização para o registro de student.</span><span class="sxs-lookup"><span data-stu-id="622e6-129">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="622e6-130">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="622e6-130">**teacherRoster**</span></span> | [<span data-ttu-id="622e6-131">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="622e6-131">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="622e6-132">Personalização para uma lista de participação do professor.</span><span class="sxs-lookup"><span data-stu-id="622e6-132">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="622e6-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="622e6-133">JSON representation</span></span>
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
