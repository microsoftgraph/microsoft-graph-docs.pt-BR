---
title: tipo de recurso governancePermission
description: 'Representa a permissão de acesso que um governanceSubject tem a um Entidadegovernanceresource específico.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: 14c8335cab401c246f95452dac699daa4f81ea93
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033840"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="5e2ef-103">tipo de recurso governancePermission</span><span class="sxs-lookup"><span data-stu-id="5e2ef-103">governancePermission resource type</span></span>

<span data-ttu-id="5e2ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e2ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e2ef-105">Representa a permissão de acesso que um [governanceSubject](../resources/governancesubject.md) tem a um [entidadegovernanceresource](../resources/governanceresource.md)específico.</span><span class="sxs-lookup"><span data-stu-id="5e2ef-105">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>


## <a name="properties"></a><span data-ttu-id="5e2ef-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e2ef-106">Properties</span></span>
| <span data-ttu-id="5e2ef-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e2ef-107">Property</span></span>     | <span data-ttu-id="5e2ef-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e2ef-108">Type</span></span>   |<span data-ttu-id="5e2ef-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e2ef-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e2ef-110">accessLevel</span><span class="sxs-lookup"><span data-stu-id="5e2ef-110">accessLevel</span></span>|<span data-ttu-id="5e2ef-111">String</span><span class="sxs-lookup"><span data-stu-id="5e2ef-111">String</span></span>|<span data-ttu-id="5e2ef-112">O nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="5e2ef-112">The access level.</span></span> <span data-ttu-id="5e2ef-113">Valores válidos: ``None`` , ``UserRead`` , ``AdminRead`` e ``AdminReadWrite`` .</span><span class="sxs-lookup"><span data-stu-id="5e2ef-113">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="5e2ef-114">isActive</span><span class="sxs-lookup"><span data-stu-id="5e2ef-114">isActive</span></span>|<span data-ttu-id="5e2ef-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="5e2ef-115">Boolean</span></span>|<span data-ttu-id="5e2ef-116">Indica se o solicitante tem qualquer atribuição de função ativa para o nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="5e2ef-116">Indicate if the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="5e2ef-117">isqualificável</span><span class="sxs-lookup"><span data-stu-id="5e2ef-117">isEligible</span></span>|<span data-ttu-id="5e2ef-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="5e2ef-118">Boolean</span></span>|<span data-ttu-id="5e2ef-119">Indica se o solicitante tem qualquer atribuição de função qualificada para o nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="5e2ef-119">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e2ef-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e2ef-120">JSON representation</span></span>

<span data-ttu-id="5e2ef-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5e2ef-121">Here is a JSON representation of the resource.</span></span>
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


