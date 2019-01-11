---
title: tipo de recurso de targetResource
description: Indica uma coleção de tipos de recursos de destino associado à atividade de auditoria. Cada tipo de recurso de destino herdará as propriedades descritas abaixo deste recurso.
localization_priority: Normal
ms.openlocfilehash: f86cfe45870292dae93327859c32d38aa2b252fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828676"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="06aa8-104">tipo de recurso de targetResource</span><span class="sxs-lookup"><span data-stu-id="06aa8-104">targetResource resource type</span></span>
<span data-ttu-id="06aa8-105">Indica uma coleção de tipos de recursos de destino associado à atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="06aa8-105">Indicates a collection of  target resource types associated with the audit activity.</span></span> <span data-ttu-id="06aa8-106">Cada tipo de recurso de destino herdará as propriedades descritas abaixo deste recurso.</span><span class="sxs-lookup"><span data-stu-id="06aa8-106">Each target resource type will inherit the properties outlined below from this resource.</span></span>


## <a name="properties"></a><span data-ttu-id="06aa8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="06aa8-107">Properties</span></span>
| <span data-ttu-id="06aa8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06aa8-108">Property</span></span>     | <span data-ttu-id="06aa8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="06aa8-109">Type</span></span>   |<span data-ttu-id="06aa8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="06aa8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06aa8-111">displayName</span><span class="sxs-lookup"><span data-stu-id="06aa8-111">displayName</span></span>|<span data-ttu-id="06aa8-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06aa8-112">String</span></span>|<span data-ttu-id="06aa8-113">Indica o nome de exibição dos recursos descritos em tipos de recursos de destino abaixo.</span><span class="sxs-lookup"><span data-stu-id="06aa8-113">Indicates the display name of the resources outlined under Target Resource Types below.</span></span>|
|<span data-ttu-id="06aa8-114">id</span><span class="sxs-lookup"><span data-stu-id="06aa8-114">id</span></span>|<span data-ttu-id="06aa8-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06aa8-115">String</span></span>|<span data-ttu-id="06aa8-116">Indica a Id exclusiva do recurso (por exemplo: UserId, AppId, RoleId.).</span><span class="sxs-lookup"><span data-stu-id="06aa8-116">Indicates the Unique Id of the resource (For example: UserId, AppId, RoleId.).</span></span>|
|<span data-ttu-id="06aa8-117">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="06aa8-117">modifiedProperties</span></span>|<span data-ttu-id="06aa8-118">coleção [modifiedProperty](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="06aa8-118">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="06aa8-119">Indica o nome, o valor antigo e o novo valor de cada atributo a ser alterado.</span><span class="sxs-lookup"><span data-stu-id="06aa8-119">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="06aa8-120">Isso é aplicável para qualquer atividades "Atualizar"</span><span class="sxs-lookup"><span data-stu-id="06aa8-120">This is applicable for any "Update" activities</span></span>|

### <a name="target-resource-types"></a><span data-ttu-id="06aa8-121">Tipos de recursos de destino</span><span class="sxs-lookup"><span data-stu-id="06aa8-121">Target Resource Types</span></span>

<span data-ttu-id="06aa8-122">O tipo de recurso de destino varia de acordo com o recurso subjacente:</span><span class="sxs-lookup"><span data-stu-id="06aa8-122">The target resource type varies according to the underlying resource:</span></span>

|<span data-ttu-id="06aa8-123">Nome do recurso</span><span class="sxs-lookup"><span data-stu-id="06aa8-123">Resource Name</span></span>| <span data-ttu-id="06aa8-124">Referência</span><span class="sxs-lookup"><span data-stu-id="06aa8-124">Reference</span></span>|
|-------------|----------|
<span data-ttu-id="06aa8-125">Device</span><span class="sxs-lookup"><span data-stu-id="06aa8-125">Device</span></span>|[<span data-ttu-id="06aa8-126">targetResourceDevice</span><span class="sxs-lookup"><span data-stu-id="06aa8-126">targetResourceDevice</span></span>](targetresourcedevice.md)
<span data-ttu-id="06aa8-127">Diretório</span><span class="sxs-lookup"><span data-stu-id="06aa8-127">Directory</span></span>|<span data-ttu-id="06aa8-128">[targetResourceDirectory] (targetresourcedirectory.md]</span><span class="sxs-lookup"><span data-stu-id="06aa8-128">[targetResourceDirectory](targetresourcedirectory.md]</span></span>
<span data-ttu-id="06aa8-129">Group</span><span class="sxs-lookup"><span data-stu-id="06aa8-129">Group</span></span>|[<span data-ttu-id="06aa8-130">targetResourceGroup</span><span class="sxs-lookup"><span data-stu-id="06aa8-130">targetResourceGroup</span></span>](targetresourcegroup.md)
<span data-ttu-id="06aa8-131">Política</span><span class="sxs-lookup"><span data-stu-id="06aa8-131">Policy</span></span>|[<span data-ttu-id="06aa8-132">targetResourcePolicy</span><span class="sxs-lookup"><span data-stu-id="06aa8-132">targetResourcePolicy</span></span>](targetresourcepolicy.md)
<span data-ttu-id="06aa8-133">Role</span><span class="sxs-lookup"><span data-stu-id="06aa8-133">Role</span></span>|[<span data-ttu-id="06aa8-134">targetResourceRole</span><span class="sxs-lookup"><span data-stu-id="06aa8-134">targetResourceRole</span></span>](targetresourcerole.md)
<span data-ttu-id="06aa8-135">Entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="06aa8-135">Service Principal</span></span>|[<span data-ttu-id="06aa8-136">targetResourceServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="06aa8-136">targetResourceServicePrincipal</span></span>](targetresourceserviceprincipal.md)
<span data-ttu-id="06aa8-137">Usuário</span><span class="sxs-lookup"><span data-stu-id="06aa8-137">User</span></span>|[<span data-ttu-id="06aa8-138">targetResourceUser</span><span class="sxs-lookup"><span data-stu-id="06aa8-138">targetResourceUser</span></span>](targetresourceuser.md)
<span data-ttu-id="06aa8-139">Outros</span><span class="sxs-lookup"><span data-stu-id="06aa8-139">Other</span></span>|[<span data-ttu-id="06aa8-140">targetResourceOther</span><span class="sxs-lookup"><span data-stu-id="06aa8-140">targetResourceOther</span></span>](targetresourceother.md)

## <a name="json-representation"></a><span data-ttu-id="06aa8-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="06aa8-141">JSON representation</span></span>

<span data-ttu-id="06aa8-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="06aa8-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
