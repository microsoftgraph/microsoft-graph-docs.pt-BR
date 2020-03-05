---
title: tipo de recurso governancePermission
description: 'Representa a permissão de acesso que um governanceSubject tem a um Entidadegovernanceresource específico.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3efdebea07bb824b2314af516810ca36ad43adc9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497619"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="e3535-103">tipo de recurso governancePermission</span><span class="sxs-lookup"><span data-stu-id="e3535-103">governancePermission resource type</span></span>

<span data-ttu-id="e3535-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e3535-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3535-105">Representa a permissão de acesso que um [governanceSubject](../resources/governancesubject.md) tem a um [entidadegovernanceresource](../resources/governanceresource.md)específico.</span><span class="sxs-lookup"><span data-stu-id="e3535-105">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="e3535-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3535-106">Properties</span></span>
| <span data-ttu-id="e3535-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3535-107">Property</span></span>     | <span data-ttu-id="e3535-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3535-108">Type</span></span>   |<span data-ttu-id="e3535-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3535-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3535-110">accessLevel</span><span class="sxs-lookup"><span data-stu-id="e3535-110">accessLevel</span></span>|<span data-ttu-id="e3535-111">String</span><span class="sxs-lookup"><span data-stu-id="e3535-111">String</span></span>|<span data-ttu-id="e3535-112">O nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="e3535-112">The access level.</span></span> <span data-ttu-id="e3535-113">Valores válidos: ``None``, ``UserRead``, ``AdminRead``e ``AdminReadWrite``.</span><span class="sxs-lookup"><span data-stu-id="e3535-113">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="e3535-114">isActive</span><span class="sxs-lookup"><span data-stu-id="e3535-114">isActive</span></span>|<span data-ttu-id="e3535-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3535-115">Boolean</span></span>|<span data-ttu-id="e3535-116">Indica se o solicitante tem qualquer atribuição de função ativa para o nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="e3535-116">Indicate if the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="e3535-117">isqualificável</span><span class="sxs-lookup"><span data-stu-id="e3535-117">isEligible</span></span>|<span data-ttu-id="e3535-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3535-118">Boolean</span></span>|<span data-ttu-id="e3535-119">Indica se o solicitante tem qualquer atribuição de função qualificada para o nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="e3535-119">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3535-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3535-120">JSON representation</span></span>

<span data-ttu-id="e3535-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3535-121">Here is a JSON representation of the resource.</span></span>
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
