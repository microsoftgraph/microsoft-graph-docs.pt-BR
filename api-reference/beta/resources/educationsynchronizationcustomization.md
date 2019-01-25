---
title: tipo de recurso de educationSynchronizationCustomization
description: 'Fornece configurações para personalizar a sincronização de perfil de dados da escola das entidades que recurso. A personalização pode ser aplicada a todas as entidades que está sendo sincronizadas. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8af6c5e2173a8b04e730529123b4608fd236f959
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513603"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="d309c-104">tipo de recurso de educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="d309c-104">educationSynchronizationCustomization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d309c-105">Fornece configurações para personalizar a sincronização de perfil de dados da escola das entidades que recurso.</span><span class="sxs-lookup"><span data-stu-id="d309c-105">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="d309c-106">A personalização pode ser aplicada a todas as entidades que está sendo sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="d309c-106">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="d309c-107">**Observação:** A propriedade **synchronizationStartDate** só se aplica à entidade **StudentEnrollment** .</span><span class="sxs-lookup"><span data-stu-id="d309c-107">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="d309c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d309c-108">Properties</span></span>

| <span data-ttu-id="d309c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d309c-109">Property</span></span> | <span data-ttu-id="d309c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d309c-110">Type</span></span> | <span data-ttu-id="d309c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d309c-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="d309c-112">**optionalPropertiesToSync**</span><span class="sxs-lookup"><span data-stu-id="d309c-112">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="d309c-113">Coleção de Cadeias de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d309c-113">collection of string</span></span> |  <span data-ttu-id="d309c-114">A coleção de nomes de propriedade para sincronização. Se definido como nulo, todas as propriedades serão sincronizados.</span><span class="sxs-lookup"><span data-stu-id="d309c-114">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="d309c-115">**synchronizationStartDate**</span><span class="sxs-lookup"><span data-stu-id="d309c-115">**synchronizationStartDate**</span></span> | <span data-ttu-id="d309c-116">DateTime</span><span class="sxs-lookup"><span data-stu-id="d309c-116">DateTime</span></span> |  <span data-ttu-id="d309c-117">A data em que a sincronização deve ser iniciado.</span><span class="sxs-lookup"><span data-stu-id="d309c-117">The date that the synchronization should start.</span></span> <span data-ttu-id="d309c-118">Este valor deve ser definido como uma data futura.</span><span class="sxs-lookup"><span data-stu-id="d309c-118">This value should be set to a future date.</span></span> <span data-ttu-id="d309c-119">Se definido como null, o recurso será sincronizado após a conclusão da configuração do perfil.</span><span class="sxs-lookup"><span data-stu-id="d309c-119">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="d309c-120">**Observação:** Isso se aplica apenas à propriedade **StudentEnrollment** .</span><span class="sxs-lookup"><span data-stu-id="d309c-120">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="d309c-121">**isSyncDeferred**</span><span class="sxs-lookup"><span data-stu-id="d309c-121">**isSyncDeferred**</span></span> |<span data-ttu-id="d309c-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="d309c-122">Boolean</span></span> | <span data-ttu-id="d309c-123">Indica se a sincronização da entidade pai é adiada para uma data posterior.</span><span class="sxs-lookup"><span data-stu-id="d309c-123">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="d309c-124">**allowDisplayNameUpdate**</span><span class="sxs-lookup"><span data-stu-id="d309c-124">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="d309c-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="d309c-125">Boolean</span></span> |  <span data-ttu-id="d309c-126">Indica se o nome de exibição do recurso pode ser substituído pela sincronização.</span><span class="sxs-lookup"><span data-stu-id="d309c-126">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="d309c-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d309c-127">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
