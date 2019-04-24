---
title: tipo de recurso educationSynchronizationCustomization
description: 'Fornece configurações para personalizar a sincronização do perfil de dados da escola das entidades de recurso. A personalização pode ser aplicada a todas as entidades que estão sendo sincronizadas. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8af6c5e2173a8b04e730529123b4608fd236f959
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507044"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="1bdc5-104">tipo de recurso educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="1bdc5-104">educationSynchronizationCustomization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bdc5-105">Fornece configurações para personalizar a sincronização do perfil de dados da escola das entidades de recurso.</span><span class="sxs-lookup"><span data-stu-id="1bdc5-105">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="1bdc5-106">A personalização pode ser aplicada a todas as entidades que estão sendo sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="1bdc5-106">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="1bdc5-107">**Observação:** A propriedade **synchronizationStartDate** só se aplica à entidade **StudentEnrollment** .</span><span class="sxs-lookup"><span data-stu-id="1bdc5-107">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="1bdc5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1bdc5-108">Properties</span></span>

| <span data-ttu-id="1bdc5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bdc5-109">Property</span></span> | <span data-ttu-id="1bdc5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bdc5-110">Type</span></span> | <span data-ttu-id="1bdc5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bdc5-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="1bdc5-112">**optionalPropertiesToSync**</span><span class="sxs-lookup"><span data-stu-id="1bdc5-112">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="1bdc5-113">coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bdc5-113">collection of string</span></span> |  <span data-ttu-id="1bdc5-114">A coleção de nomes de propriedade a serem sincronizados. Se definido como nulo, todas as propriedades serão sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="1bdc5-114">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="1bdc5-115">**synchronizationStartDate**</span><span class="sxs-lookup"><span data-stu-id="1bdc5-115">**synchronizationStartDate**</span></span> | <span data-ttu-id="1bdc5-116">DateTime</span><span class="sxs-lookup"><span data-stu-id="1bdc5-116">DateTime</span></span> |  <span data-ttu-id="1bdc5-117">A data em que a sincronização deve ser iniciada.</span><span class="sxs-lookup"><span data-stu-id="1bdc5-117">The date that the synchronization should start.</span></span> <span data-ttu-id="1bdc5-118">Esse valor deve ser definido para uma data futura.</span><span class="sxs-lookup"><span data-stu-id="1bdc5-118">This value should be set to a future date.</span></span> <span data-ttu-id="1bdc5-119">Se definido como nulo, o recurso será sincronizado quando a configuração do perfil for concluída.</span><span class="sxs-lookup"><span data-stu-id="1bdc5-119">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="1bdc5-120">**Observação:** Isso só se aplica à propriedade **StudentEnrollment** .</span><span class="sxs-lookup"><span data-stu-id="1bdc5-120">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="1bdc5-121">**isSyncDeferred**</span><span class="sxs-lookup"><span data-stu-id="1bdc5-121">**isSyncDeferred**</span></span> |<span data-ttu-id="1bdc5-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="1bdc5-122">Boolean</span></span> | <span data-ttu-id="1bdc5-123">Indica se a sincronização da entidade pai será adiada para uma data posterior.</span><span class="sxs-lookup"><span data-stu-id="1bdc5-123">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="1bdc5-124">**allowDisplayNameUpdate**</span><span class="sxs-lookup"><span data-stu-id="1bdc5-124">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="1bdc5-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="1bdc5-125">Boolean</span></span> |  <span data-ttu-id="1bdc5-126">Indica se o nome de exibição do recurso pode ser substituído pela sincronização.</span><span class="sxs-lookup"><span data-stu-id="1bdc5-126">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="1bdc5-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1bdc5-127">JSON representation</span></span>
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
