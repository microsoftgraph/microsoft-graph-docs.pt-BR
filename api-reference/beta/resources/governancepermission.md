---
title: Tipo de recurso governancePermission
description: 'Representa a permissão de acesso que um governanceSubject tem para uma governanceResource específica.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: f316a863ecba9ed546b9ba4045e57ada87e97ab9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128831"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="e6cc5-103">Tipo de recurso governancePermission</span><span class="sxs-lookup"><span data-stu-id="e6cc5-103">governancePermission resource type</span></span>

<span data-ttu-id="e6cc5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6cc5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6cc5-105">Representa a permissão de acesso que um [governanceSubject](../resources/governancesubject.md) tem para uma [governança EspecíficaResource](../resources/governanceresource.md).</span><span class="sxs-lookup"><span data-stu-id="e6cc5-105">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>


## <a name="properties"></a><span data-ttu-id="e6cc5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6cc5-106">Properties</span></span>
| <span data-ttu-id="e6cc5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6cc5-107">Property</span></span>     | <span data-ttu-id="e6cc5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6cc5-108">Type</span></span>   |<span data-ttu-id="e6cc5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6cc5-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6cc5-110">accessLevel</span><span class="sxs-lookup"><span data-stu-id="e6cc5-110">accessLevel</span></span>|<span data-ttu-id="e6cc5-111">String</span><span class="sxs-lookup"><span data-stu-id="e6cc5-111">String</span></span>|<span data-ttu-id="e6cc5-112">O nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="e6cc5-112">The access level.</span></span> <span data-ttu-id="e6cc5-113">Valores válidos: ``None`` ``UserRead`` , , e ``AdminRead`` ``AdminReadWrite`` .</span><span class="sxs-lookup"><span data-stu-id="e6cc5-113">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="e6cc5-114">isActive</span><span class="sxs-lookup"><span data-stu-id="e6cc5-114">isActive</span></span>|<span data-ttu-id="e6cc5-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6cc5-115">Boolean</span></span>|<span data-ttu-id="e6cc5-116">Indica se o solicitante tem qualquer atribuição de função ativa para o nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="e6cc5-116">Indicate if the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="e6cc5-117">isEligible</span><span class="sxs-lookup"><span data-stu-id="e6cc5-117">isEligible</span></span>|<span data-ttu-id="e6cc5-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6cc5-118">Boolean</span></span>|<span data-ttu-id="e6cc5-119">Indica se o solicitante tem qualquer atribuição de função qualificada para o nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="e6cc5-119">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e6cc5-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6cc5-120">JSON representation</span></span>

<span data-ttu-id="e6cc5-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6cc5-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governancePermission"
}-->
```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```


