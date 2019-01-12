---
title: tipo de recurso de educationSynchronizationCustomization
description: 'Fornece configurações para personalizar a sincronização de perfil de dados da escola das entidades que recurso. A personalização pode ser aplicada a todas as entidades que está sendo sincronizadas. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c4e8810202dbae5fdc3d978bd27e0463f0424d2e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962867"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="5bb62-104">tipo de recurso de educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="5bb62-104">educationSynchronizationCustomization resource type</span></span>

> <span data-ttu-id="5bb62-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5bb62-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5bb62-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5bb62-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5bb62-107">Fornece configurações para personalizar a sincronização de perfil de dados da escola das entidades que recurso.</span><span class="sxs-lookup"><span data-stu-id="5bb62-107">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="5bb62-108">A personalização pode ser aplicada a todas as entidades que está sendo sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="5bb62-108">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="5bb62-109">**Observação:** A propriedade **synchronizationStartDate** só se aplica à entidade **StudentEnrollment** .</span><span class="sxs-lookup"><span data-stu-id="5bb62-109">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="5bb62-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5bb62-110">Properties</span></span>

| <span data-ttu-id="5bb62-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5bb62-111">Property</span></span> | <span data-ttu-id="5bb62-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="5bb62-112">Type</span></span> | <span data-ttu-id="5bb62-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bb62-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="5bb62-114">**optionalPropertiesToSync**</span><span class="sxs-lookup"><span data-stu-id="5bb62-114">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="5bb62-115">coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bb62-115">collection of string</span></span> |  <span data-ttu-id="5bb62-116">A coleção de nomes de propriedade para sincronização. Se definido como nulo, todas as propriedades serão sincronizados.</span><span class="sxs-lookup"><span data-stu-id="5bb62-116">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="5bb62-117">**synchronizationStartDate**</span><span class="sxs-lookup"><span data-stu-id="5bb62-117">**synchronizationStartDate**</span></span> | <span data-ttu-id="5bb62-118">DateTime</span><span class="sxs-lookup"><span data-stu-id="5bb62-118">DateTime</span></span> |  <span data-ttu-id="5bb62-119">A data em que a sincronização deve ser iniciado.</span><span class="sxs-lookup"><span data-stu-id="5bb62-119">The date that the synchronization should start.</span></span> <span data-ttu-id="5bb62-120">Este valor deve ser definido como uma data futura.</span><span class="sxs-lookup"><span data-stu-id="5bb62-120">This value should be set to a future date.</span></span> <span data-ttu-id="5bb62-121">Se definido como null, o recurso será sincronizado após a conclusão da configuração do perfil.</span><span class="sxs-lookup"><span data-stu-id="5bb62-121">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="5bb62-122">**Observação:** Isso se aplica apenas à propriedade **StudentEnrollment** .</span><span class="sxs-lookup"><span data-stu-id="5bb62-122">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="5bb62-123">**isSyncDeferred**</span><span class="sxs-lookup"><span data-stu-id="5bb62-123">**isSyncDeferred**</span></span> |<span data-ttu-id="5bb62-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="5bb62-124">Boolean</span></span> | <span data-ttu-id="5bb62-125">Indica se a sincronização da entidade pai é adiada para uma data posterior.</span><span class="sxs-lookup"><span data-stu-id="5bb62-125">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="5bb62-126">**allowDisplayNameUpdate**</span><span class="sxs-lookup"><span data-stu-id="5bb62-126">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="5bb62-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="5bb62-127">Boolean</span></span> |  <span data-ttu-id="5bb62-128">Indica se o nome de exibição do recurso pode ser substituído pela sincronização.</span><span class="sxs-lookup"><span data-stu-id="5bb62-128">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="5bb62-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5bb62-129">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
