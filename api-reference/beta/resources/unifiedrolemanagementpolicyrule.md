---
title: Tipo de recurso unifiedRoleManagementPolicyRule
description: Um unifiedRoleManagementPolicyRule especifica a regra associada a uma política de gerenciamento de função. É abstrato.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: aa0bc719fe4722692b1ff42861cccede7150780d
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682240"
---
# <a name="unifiedrolemanagementpolicyrule-resource-type"></a><span data-ttu-id="da974-104">Tipo de recurso unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="da974-104">unifiedRoleManagementPolicyRule resource type</span></span>

<span data-ttu-id="da974-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da974-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da974-106">Um unifiedRoleManagementPolicyRule especifica a regra associada a uma política de gerenciamento de função.</span><span class="sxs-lookup"><span data-stu-id="da974-106">A unifiedRoleManagementPolicyRule specifies the rule associated with a role management policy.</span></span> <span data-ttu-id="da974-107">É abstrato.</span><span class="sxs-lookup"><span data-stu-id="da974-107">It is abstract.</span></span>

## <a name="methods"></a><span data-ttu-id="da974-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="da974-108">Methods</span></span>
|<span data-ttu-id="da974-109">Método</span><span class="sxs-lookup"><span data-stu-id="da974-109">Method</span></span>|<span data-ttu-id="da974-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="da974-110">Return type</span></span>|<span data-ttu-id="da974-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="da974-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="da974-112">Listar unifiedRoleManagementPolicyRules</span><span class="sxs-lookup"><span data-stu-id="da974-112">List unifiedRoleManagementPolicyRules</span></span>](../api/unifiedrolemanagementpolicyrule-list.md)|<span data-ttu-id="da974-113">[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="da974-113">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection</span></span>|<span data-ttu-id="da974-114">Obter uma lista dos [objetos unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="da974-114">Get a list of the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) objects and their properties.</span></span>|
|[<span data-ttu-id="da974-115">Obter unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="da974-115">Get unifiedRoleManagementPolicyRule</span></span>](../api/unifiedrolemanagementpolicyrule-get.md)|[<span data-ttu-id="da974-116">unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="da974-116">unifiedRoleManagementPolicyRule</span></span>](../resources/unifiedrolemanagementpolicyrule.md)|<span data-ttu-id="da974-117">Leia as propriedades e as relações de [um objeto unifiedRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="da974-117">Read the properties and relationships of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>|
|[<span data-ttu-id="da974-118">Atualizar unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="da974-118">Update unifiedRoleManagementPolicyRule</span></span>](../api/unifiedrolemanagementpolicyrule-update.md)|[<span data-ttu-id="da974-119">unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="da974-119">unifiedRoleManagementPolicyRule</span></span>](../resources/unifiedrolemanagementpolicyrule.md)|<span data-ttu-id="da974-120">Atualize as propriedades de [um objeto unifiedRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="da974-120">Update the properties of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="da974-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da974-121">Properties</span></span>
|<span data-ttu-id="da974-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da974-122">Property</span></span>|<span data-ttu-id="da974-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="da974-123">Type</span></span>|<span data-ttu-id="da974-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="da974-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da974-125">id</span><span class="sxs-lookup"><span data-stu-id="da974-125">id</span></span>|<span data-ttu-id="da974-126">String</span><span class="sxs-lookup"><span data-stu-id="da974-126">String</span></span>|<span data-ttu-id="da974-127">Identificador exclusivo da regra.</span><span class="sxs-lookup"><span data-stu-id="da974-127">Unique identifier for the rule.</span></span>|
|<span data-ttu-id="da974-128">destino</span><span class="sxs-lookup"><span data-stu-id="da974-128">target</span></span>|[<span data-ttu-id="da974-129">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="da974-129">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="da974-130">O destino da regra de política.</span><span class="sxs-lookup"><span data-stu-id="da974-130">The target for the policy rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da974-131">Relações</span><span class="sxs-lookup"><span data-stu-id="da974-131">Relationships</span></span>
<span data-ttu-id="da974-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="da974-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="da974-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da974-133">JSON representation</span></span>
<span data-ttu-id="da974-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da974-134">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  }
}
```

