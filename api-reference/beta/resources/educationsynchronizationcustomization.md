---
title: tipo de recurso educationSynchronizationCustomization
description: 'Fornece configurações para personalizar a sincronização do perfil de dados da escola das entidades de recurso. A personalização pode ser aplicada a todas as entidades que estão sendo sincronizadas. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 368117a5293f4ede59282fa1ced12d024976de52
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500461"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="80728-104">tipo de recurso educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="80728-104">educationSynchronizationCustomization resource type</span></span>

<span data-ttu-id="80728-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="80728-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80728-106">Fornece configurações para personalizar a sincronização do perfil de dados da escola das entidades de recurso.</span><span class="sxs-lookup"><span data-stu-id="80728-106">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="80728-107">A personalização pode ser aplicada a todas as entidades que estão sendo sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="80728-107">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="80728-108">**Observação:** A propriedade **synchronizationStartDate** só se aplica à entidade **StudentEnrollment** .</span><span class="sxs-lookup"><span data-stu-id="80728-108">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="80728-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80728-109">Properties</span></span>

| <span data-ttu-id="80728-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80728-110">Property</span></span> | <span data-ttu-id="80728-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="80728-111">Type</span></span> | <span data-ttu-id="80728-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="80728-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="80728-113">**optionalPropertiesToSync**</span><span class="sxs-lookup"><span data-stu-id="80728-113">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="80728-114">coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80728-114">collection of string</span></span> |  <span data-ttu-id="80728-115">A coleção de nomes de propriedade a serem sincronizados. Se definido como nulo, todas as propriedades serão sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="80728-115">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="80728-116">**synchronizationStartDate**</span><span class="sxs-lookup"><span data-stu-id="80728-116">**synchronizationStartDate**</span></span> | <span data-ttu-id="80728-117">DateTime</span><span class="sxs-lookup"><span data-stu-id="80728-117">DateTime</span></span> |  <span data-ttu-id="80728-118">A data em que a sincronização deve ser iniciada.</span><span class="sxs-lookup"><span data-stu-id="80728-118">The date that the synchronization should start.</span></span> <span data-ttu-id="80728-119">Esse valor deve ser definido para uma data futura.</span><span class="sxs-lookup"><span data-stu-id="80728-119">This value should be set to a future date.</span></span> <span data-ttu-id="80728-120">Se definido como nulo, o recurso será sincronizado quando a configuração do perfil for concluída.</span><span class="sxs-lookup"><span data-stu-id="80728-120">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="80728-121">**Observação:** Isso só se aplica à propriedade **StudentEnrollment** .</span><span class="sxs-lookup"><span data-stu-id="80728-121">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="80728-122">**isSyncDeferred**</span><span class="sxs-lookup"><span data-stu-id="80728-122">**isSyncDeferred**</span></span> |<span data-ttu-id="80728-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="80728-123">Boolean</span></span> | <span data-ttu-id="80728-124">Indica se a sincronização da entidade pai será adiada para uma data posterior.</span><span class="sxs-lookup"><span data-stu-id="80728-124">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="80728-125">**allowDisplayNameUpdate**</span><span class="sxs-lookup"><span data-stu-id="80728-125">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="80728-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="80728-126">Boolean</span></span> |  <span data-ttu-id="80728-127">Indica se o nome de exibição do recurso pode ser substituído pela sincronização.</span><span class="sxs-lookup"><span data-stu-id="80728-127">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="80728-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80728-128">JSON representation</span></span>
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
