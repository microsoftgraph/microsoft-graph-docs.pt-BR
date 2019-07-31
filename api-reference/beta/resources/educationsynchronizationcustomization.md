---
title: tipo de recurso educationSynchronizationCustomization
description: 'Fornece configurações para personalizar a sincronização do perfil de dados da escola das entidades de recurso. A personalização pode ser aplicada a todas as entidades que estão sendo sincronizadas. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 46cd20bbe016110a313d5b195a518ef81ca05afe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972450"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="1dc06-104">tipo de recurso educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="1dc06-104">educationSynchronizationCustomization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dc06-105">Fornece configurações para personalizar a sincronização do perfil de dados da escola das entidades de recurso.</span><span class="sxs-lookup"><span data-stu-id="1dc06-105">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="1dc06-106">A personalização pode ser aplicada a todas as entidades que estão sendo sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="1dc06-106">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="1dc06-107">**Observação:** A propriedade **synchronizationStartDate** só se aplica à entidade **StudentEnrollment** .</span><span class="sxs-lookup"><span data-stu-id="1dc06-107">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="1dc06-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1dc06-108">Properties</span></span>

| <span data-ttu-id="1dc06-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1dc06-109">Property</span></span> | <span data-ttu-id="1dc06-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dc06-110">Type</span></span> | <span data-ttu-id="1dc06-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dc06-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="1dc06-112">**optionalPropertiesToSync**</span><span class="sxs-lookup"><span data-stu-id="1dc06-112">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="1dc06-113">coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1dc06-113">collection of string</span></span> |  <span data-ttu-id="1dc06-114">A coleção de nomes de propriedade a serem sincronizados. Se definido como nulo, todas as propriedades serão sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="1dc06-114">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="1dc06-115">**synchronizationStartDate**</span><span class="sxs-lookup"><span data-stu-id="1dc06-115">**synchronizationStartDate**</span></span> | <span data-ttu-id="1dc06-116">DateTime</span><span class="sxs-lookup"><span data-stu-id="1dc06-116">DateTime</span></span> |  <span data-ttu-id="1dc06-117">A data em que a sincronização deve ser iniciada.</span><span class="sxs-lookup"><span data-stu-id="1dc06-117">The date that the synchronization should start.</span></span> <span data-ttu-id="1dc06-118">Esse valor deve ser definido para uma data futura.</span><span class="sxs-lookup"><span data-stu-id="1dc06-118">This value should be set to a future date.</span></span> <span data-ttu-id="1dc06-119">Se definido como nulo, o recurso será sincronizado quando a configuração do perfil for concluída.</span><span class="sxs-lookup"><span data-stu-id="1dc06-119">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="1dc06-120">**Observação:** Isso só se aplica à propriedade **StudentEnrollment** .</span><span class="sxs-lookup"><span data-stu-id="1dc06-120">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="1dc06-121">**isSyncDeferred**</span><span class="sxs-lookup"><span data-stu-id="1dc06-121">**isSyncDeferred**</span></span> |<span data-ttu-id="1dc06-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="1dc06-122">Boolean</span></span> | <span data-ttu-id="1dc06-123">Indica se a sincronização da entidade pai será adiada para uma data posterior.</span><span class="sxs-lookup"><span data-stu-id="1dc06-123">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="1dc06-124">**allowDisplayNameUpdate**</span><span class="sxs-lookup"><span data-stu-id="1dc06-124">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="1dc06-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="1dc06-125">Boolean</span></span> |  <span data-ttu-id="1dc06-126">Indica se o nome de exibição do recurso pode ser substituído pela sincronização.</span><span class="sxs-lookup"><span data-stu-id="1dc06-126">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="1dc06-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1dc06-127">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
