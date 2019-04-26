---
title: tipo de recurso governancePermission
description: 'Representa a permissão de acesso que um governanceSubject tem a um Entidadegovernanceresource específico.  '
localization_priority: Normal
ms.openlocfilehash: 2f6be4bdc502f829b1dcfd991d1c2ae6130dea8a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340176"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="8ad3e-103">tipo de recurso governancePermission</span><span class="sxs-lookup"><span data-stu-id="8ad3e-103">governancePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ad3e-104">Representa a permissão de acesso que um [governanceSubject](../resources/governancesubject.md) tem a um [entidadegovernanceresource](../resources/governanceresource.md)específico.</span><span class="sxs-lookup"><span data-stu-id="8ad3e-104">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="8ad3e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ad3e-105">Properties</span></span>
| <span data-ttu-id="8ad3e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ad3e-106">Property</span></span>     | <span data-ttu-id="8ad3e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ad3e-107">Type</span></span>   |<span data-ttu-id="8ad3e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ad3e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ad3e-109">accessLevel</span><span class="sxs-lookup"><span data-stu-id="8ad3e-109">accessLevel</span></span>|<span data-ttu-id="8ad3e-110">String</span><span class="sxs-lookup"><span data-stu-id="8ad3e-110">String</span></span>|<span data-ttu-id="8ad3e-111">O nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="8ad3e-111">The access level.</span></span> <span data-ttu-id="8ad3e-112">Valores válidos: ``None``, ``UserRead``, ``AdminRead``e ``AdminReadWrite``.</span><span class="sxs-lookup"><span data-stu-id="8ad3e-112">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="8ad3e-113">isActive</span><span class="sxs-lookup"><span data-stu-id="8ad3e-113">isActive</span></span>|<span data-ttu-id="8ad3e-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ad3e-114">Boolean</span></span>|<span data-ttu-id="8ad3e-115">Indica se o solicitante tem qualquer atribuição de função ativa para o nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="8ad3e-115">Indicate if the the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="8ad3e-116">isQualificável</span><span class="sxs-lookup"><span data-stu-id="8ad3e-116">isEligible</span></span>|<span data-ttu-id="8ad3e-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ad3e-117">Boolean</span></span>|<span data-ttu-id="8ad3e-118">Indica se o solicitante tem qualquer atribuição de função qualificada para o nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="8ad3e-118">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ad3e-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ad3e-119">JSON representation</span></span>

<span data-ttu-id="8ad3e-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ad3e-120">Here is a JSON representation of the resource.</span></span>
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
