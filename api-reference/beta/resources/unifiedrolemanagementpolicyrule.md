---
title: Tipo de recurso unifiedRoleManagementPolicyRule
description: Um unifiedRoleManagementPolicyRule especifica a regra associada a uma política de gerenciamento de função. É abstrato.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 420ebfca11d2873ad942782fb8e7d97e893b7185
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298995"
---
# <a name="unifiedrolemanagementpolicyrule-resource-type"></a><span data-ttu-id="a2aaf-104">Tipo de recurso unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="a2aaf-104">unifiedRoleManagementPolicyRule resource type</span></span>

<span data-ttu-id="a2aaf-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2aaf-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a2aaf-106">Um unifiedRoleManagementPolicyRule especifica a regra associada a uma política de gerenciamento de função.</span><span class="sxs-lookup"><span data-stu-id="a2aaf-106">A unifiedRoleManagementPolicyRule specifies the rule associated with a role management policy.</span></span> <span data-ttu-id="a2aaf-107">É abstrato.</span><span class="sxs-lookup"><span data-stu-id="a2aaf-107">It is abstract.</span></span>

## <a name="methods"></a><span data-ttu-id="a2aaf-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="a2aaf-108">Methods</span></span>
|<span data-ttu-id="a2aaf-109">Método</span><span class="sxs-lookup"><span data-stu-id="a2aaf-109">Method</span></span>|<span data-ttu-id="a2aaf-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a2aaf-110">Return type</span></span>|<span data-ttu-id="a2aaf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2aaf-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a2aaf-112">Listar unifiedRoleManagementPolicyRules</span><span class="sxs-lookup"><span data-stu-id="a2aaf-112">List unifiedRoleManagementPolicyRules</span></span>](../api/unifiedrolemanagementpolicyrule-list.md)|<span data-ttu-id="a2aaf-113">[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="a2aaf-113">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection</span></span>|<span data-ttu-id="a2aaf-114">Obter uma lista dos [objetos unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="a2aaf-114">Get a list of the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) objects and their properties.</span></span>|
|[<span data-ttu-id="a2aaf-115">Obter unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="a2aaf-115">Get unifiedRoleManagementPolicyRule</span></span>](../api/unifiedrolemanagementpolicyrule-get.md)|[<span data-ttu-id="a2aaf-116">unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="a2aaf-116">unifiedRoleManagementPolicyRule</span></span>](../resources/unifiedrolemanagementpolicyrule.md)|<span data-ttu-id="a2aaf-117">Leia as propriedades e as relações de [um objeto unifiedRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="a2aaf-117">Read the properties and relationships of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>|
|[<span data-ttu-id="a2aaf-118">Atualizar unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="a2aaf-118">Update unifiedRoleManagementPolicyRule</span></span>](../api/unifiedrolemanagementpolicyrule-update.md)|[<span data-ttu-id="a2aaf-119">unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="a2aaf-119">unifiedRoleManagementPolicyRule</span></span>](../resources/unifiedrolemanagementpolicyrule.md)|<span data-ttu-id="a2aaf-120">Atualize as propriedades de [um objeto unifiedRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="a2aaf-120">Update the properties of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a2aaf-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2aaf-121">Properties</span></span>
|<span data-ttu-id="a2aaf-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2aaf-122">Property</span></span>|<span data-ttu-id="a2aaf-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2aaf-123">Type</span></span>|<span data-ttu-id="a2aaf-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2aaf-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2aaf-125">id</span><span class="sxs-lookup"><span data-stu-id="a2aaf-125">id</span></span>|<span data-ttu-id="a2aaf-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2aaf-126">String</span></span>|<span data-ttu-id="a2aaf-127">Identificador exclusivo da regra.</span><span class="sxs-lookup"><span data-stu-id="a2aaf-127">Unique identifier for the rule.</span></span>|
|<span data-ttu-id="a2aaf-128">destino</span><span class="sxs-lookup"><span data-stu-id="a2aaf-128">target</span></span>|[<span data-ttu-id="a2aaf-129">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="a2aaf-129">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="a2aaf-130">O destino da regra de política.</span><span class="sxs-lookup"><span data-stu-id="a2aaf-130">The target for the policy rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2aaf-131">Relações</span><span class="sxs-lookup"><span data-stu-id="a2aaf-131">Relationships</span></span>
<span data-ttu-id="a2aaf-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a2aaf-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2aaf-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2aaf-133">JSON representation</span></span>
<span data-ttu-id="a2aaf-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2aaf-134">The following is a JSON representation of the resource.</span></span>
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

