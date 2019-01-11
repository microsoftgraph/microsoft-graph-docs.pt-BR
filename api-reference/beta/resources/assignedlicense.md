---
title: Tipo de recurso assignedLicense
description: Representa uma licença atribuída a um usuário. A propriedade **assignedLicenses** da entidade user é uma coleção de **assignedLicense**.
localization_priority: Normal
ms.openlocfilehash: dfb93075fe62a0cfb479e12554e9078e876c4529
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853779"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="e9c84-104">Tipo de recurso assignedLicense</span><span class="sxs-lookup"><span data-stu-id="e9c84-104">assignedLicense resource type</span></span>

> <span data-ttu-id="e9c84-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e9c84-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9c84-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e9c84-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e9c84-p103">Representa uma licença atribuída a um usuário. A propriedade **assignedLicenses** da entidade [user](user.md) é uma coleção de **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="e9c84-p103">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="e9c84-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e9c84-109">Properties</span></span>
| <span data-ttu-id="e9c84-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9c84-110">Property</span></span>     | <span data-ttu-id="e9c84-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9c84-111">Type</span></span>   |<span data-ttu-id="e9c84-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9c84-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9c84-113">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="e9c84-113">disabledPlans</span></span>|<span data-ttu-id="e9c84-114">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="e9c84-114">Guid collection</span></span>|<span data-ttu-id="e9c84-115">Uma coleção dos identificadores exclusivos de planos que foram desabilitados.</span><span class="sxs-lookup"><span data-stu-id="e9c84-115">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="e9c84-116">skuId</span><span class="sxs-lookup"><span data-stu-id="e9c84-116">skuId</span></span>|<span data-ttu-id="e9c84-117">Guid</span><span class="sxs-lookup"><span data-stu-id="e9c84-117">Guid</span></span>|<span data-ttu-id="e9c84-118">O identificador exclusivo da SKU.</span><span class="sxs-lookup"><span data-stu-id="e9c84-118">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9c84-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e9c84-119">JSON representation</span></span>

<span data-ttu-id="e9c84-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e9c84-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
