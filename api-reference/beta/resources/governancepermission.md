---
title: tipo de recurso governancePermission
description: 'Representa a permissão de acesso que um governanceSubject tem a um Entidadegovernanceresource específico.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8bf32b855ed77ccdf712b1a739ef913d0a3dade0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971939"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="b76b4-103">tipo de recurso governancePermission</span><span class="sxs-lookup"><span data-stu-id="b76b4-103">governancePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b76b4-104">Representa a permissão de acesso que um [governanceSubject](../resources/governancesubject.md) tem a um [entidadegovernanceresource](../resources/governanceresource.md)específico.</span><span class="sxs-lookup"><span data-stu-id="b76b4-104">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="b76b4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b76b4-105">Properties</span></span>
| <span data-ttu-id="b76b4-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b76b4-106">Property</span></span>     | <span data-ttu-id="b76b4-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b76b4-107">Type</span></span>   |<span data-ttu-id="b76b4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b76b4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b76b4-109">accessLevel</span><span class="sxs-lookup"><span data-stu-id="b76b4-109">accessLevel</span></span>|<span data-ttu-id="b76b4-110">String</span><span class="sxs-lookup"><span data-stu-id="b76b4-110">String</span></span>|<span data-ttu-id="b76b4-111">O nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="b76b4-111">The access level.</span></span> <span data-ttu-id="b76b4-112">Valores válidos: ``None``, ``UserRead``, ``AdminRead``e ``AdminReadWrite``.</span><span class="sxs-lookup"><span data-stu-id="b76b4-112">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="b76b4-113">isActive</span><span class="sxs-lookup"><span data-stu-id="b76b4-113">isActive</span></span>|<span data-ttu-id="b76b4-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="b76b4-114">Boolean</span></span>|<span data-ttu-id="b76b4-115">Indica se o solicitante tem qualquer atribuição de função ativa para o nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="b76b4-115">Indicate if the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="b76b4-116">isqualificável</span><span class="sxs-lookup"><span data-stu-id="b76b4-116">isEligible</span></span>|<span data-ttu-id="b76b4-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="b76b4-117">Boolean</span></span>|<span data-ttu-id="b76b4-118">Indica se o solicitante tem qualquer atribuição de função qualificada para o nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="b76b4-118">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b76b4-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b76b4-119">JSON representation</span></span>

<span data-ttu-id="b76b4-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b76b4-120">Here is a JSON representation of the resource.</span></span>
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
