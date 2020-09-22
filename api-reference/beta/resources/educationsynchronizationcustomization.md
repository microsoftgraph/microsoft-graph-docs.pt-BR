---
title: tipo de recurso educationSynchronizationCustomization
description: 'Fornece configurações para personalizar a sincronização do perfil de dados da escola das entidades de recurso. A personalização pode ser aplicada a todas as entidades que estão sendo sincronizadas. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c3f704339dbf2acbe7cb78e1899c5f209f50f21e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055587"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="c4715-104">tipo de recurso educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c4715-104">educationSynchronizationCustomization resource type</span></span>

<span data-ttu-id="c4715-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4715-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4715-106">Fornece configurações para personalizar a sincronização do perfil de dados da escola das entidades de recurso.</span><span class="sxs-lookup"><span data-stu-id="c4715-106">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="c4715-107">A personalização pode ser aplicada a todas as entidades que estão sendo sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="c4715-107">The customization can be applied to all the entities being synchronized.</span></span>

## <a name="properties"></a><span data-ttu-id="c4715-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c4715-108">Properties</span></span>

| <span data-ttu-id="c4715-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4715-109">Property</span></span>                 | <span data-ttu-id="c4715-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4715-110">Type</span></span>              | <span data-ttu-id="c4715-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4715-111">Description</span></span>                                                                                                                                                                                                            |
| :----------------------- | :---------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="c4715-112">optionalPropertiesToSync</span><span class="sxs-lookup"><span data-stu-id="c4715-112">optionalPropertiesToSync</span></span> | <span data-ttu-id="c4715-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4715-113">String collection</span></span> | <span data-ttu-id="c4715-114">A coleção de nomes de propriedade a serem sincronizados. Se definido como nulo, todas as propriedades serão sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="c4715-114">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span> <span data-ttu-id="c4715-115">**Não se aplica a registradoras ou listas de professores do aluno**</span><span class="sxs-lookup"><span data-stu-id="c4715-115">**Does not apply to Student Enrollments or Teacher Rosters**</span></span>                                                            |
| <span data-ttu-id="c4715-116">synchronizationStartDate</span><span class="sxs-lookup"><span data-stu-id="c4715-116">synchronizationStartDate</span></span> | <span data-ttu-id="c4715-117">DateTime</span><span class="sxs-lookup"><span data-stu-id="c4715-117">DateTime</span></span>          | <span data-ttu-id="c4715-118">A data em que a sincronização deve ser iniciada.</span><span class="sxs-lookup"><span data-stu-id="c4715-118">The date that the synchronization should start.</span></span> <span data-ttu-id="c4715-119">Esse valor deve ser definido para uma data futura.</span><span class="sxs-lookup"><span data-stu-id="c4715-119">This value should be set to a future date.</span></span> <span data-ttu-id="c4715-120">Se definido como nulo, o recurso será sincronizado quando a configuração do perfil for concluída.</span><span class="sxs-lookup"><span data-stu-id="c4715-120">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="c4715-121">**Aplica-se apenas às registradoras de alunos**</span><span class="sxs-lookup"><span data-stu-id="c4715-121">**Only applies to Student Enrollments**</span></span> |
| <span data-ttu-id="c4715-122">isSyncDeferred</span><span class="sxs-lookup"><span data-stu-id="c4715-122">isSyncDeferred</span></span>           | <span data-ttu-id="c4715-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="c4715-123">Boolean</span></span>           | <span data-ttu-id="c4715-124">Indica se a sincronização da entidade pai será adiada para uma data posterior.</span><span class="sxs-lookup"><span data-stu-id="c4715-124">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span>                                                                                                                                    |
| <span data-ttu-id="c4715-125">allowDisplayNameUpdate</span><span class="sxs-lookup"><span data-stu-id="c4715-125">allowDisplayNameUpdate</span></span>   | <span data-ttu-id="c4715-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="c4715-126">Boolean</span></span>           | <span data-ttu-id="c4715-127">Indica se o nome de exibição do recurso pode ser substituído pela sincronização.</span><span class="sxs-lookup"><span data-stu-id="c4715-127">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>                                                                                                                                     |

## <a name="json-representation"></a><span data-ttu-id="c4715-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c4715-128">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{
  "optionalPropertiesToSync": ["String"],
  "synchronizationStartDate": "DateTimeOffset",
  "isSyncDeferred": "Boolean",
  "allowDisplayNameUpdate": "Boolean"
}
```


