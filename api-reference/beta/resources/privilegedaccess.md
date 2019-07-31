---
title: tipo de recurso privilegedAccess
description: " por exemplo, `privilegedAccess/azureResources` representa o PIM que gerencia o acesso privilegiado aos recursos do Azure."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7f59f8420be6ff97511415e944d154cb5d59950f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965786"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="bc67f-103">tipo de recurso privilegedAccess</span><span class="sxs-lookup"><span data-stu-id="bc67f-103">privilegedAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc67f-104">Representa um grupo de funcionalidades fornecidas pelo serviço de gerenciamento de identidade privilegiado (PIM).</span><span class="sxs-lookup"><span data-stu-id="bc67f-104">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="bc67f-105">Instâncias diferentes de `privilegedAccess` representar diferentes provedores gerenciados pelo PIM; por exemplo, `privilegedAccess/azureResources` representa o PIM que gerencia o acesso privilegiado aos recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="bc67f-105">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="bc67f-106">`privilegedAccess`é somente leitura por enquanto.</span><span class="sxs-lookup"><span data-stu-id="bc67f-106">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="bc67f-107">`POST` `DELETE` Nenhuma operação é suportada no conjunto de `privilegedAccess` `PUT` `PATCH`entidades.</span><span class="sxs-lookup"><span data-stu-id="bc67f-107">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="bc67f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc67f-108">Properties</span></span>
| <span data-ttu-id="bc67f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc67f-109">Property</span></span>  | <span data-ttu-id="bc67f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc67f-110">Type</span></span>      |<span data-ttu-id="bc67f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc67f-111">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="bc67f-112">id</span><span class="sxs-lookup"><span data-stu-id="bc67f-112">id</span></span>         |<span data-ttu-id="bc67f-113">String</span><span class="sxs-lookup"><span data-stu-id="bc67f-113">String</span></span>     |<span data-ttu-id="bc67f-114">A ID do provedor gerenciado pelo PIM.</span><span class="sxs-lookup"><span data-stu-id="bc67f-114">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="bc67f-115">displayName</span><span class="sxs-lookup"><span data-stu-id="bc67f-115">displayName</span></span>|<span data-ttu-id="bc67f-116">String</span><span class="sxs-lookup"><span data-stu-id="bc67f-116">String</span></span>     |<span data-ttu-id="bc67f-117">O nome de exibição do provedor gerenciado pelo PIM.</span><span class="sxs-lookup"><span data-stu-id="bc67f-117">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="bc67f-118">Relações</span><span class="sxs-lookup"><span data-stu-id="bc67f-118">Relationships</span></span>
| <span data-ttu-id="bc67f-119">Relação</span><span class="sxs-lookup"><span data-stu-id="bc67f-119">Relationship</span></span>   | <span data-ttu-id="bc67f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc67f-120">Type</span></span>                                         |<span data-ttu-id="bc67f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc67f-121">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="bc67f-122">recursos</span><span class="sxs-lookup"><span data-stu-id="bc67f-122">resources</span></span>       |<span data-ttu-id="bc67f-123">coleção [entidadegovernanceresource](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="bc67f-123">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="bc67f-124">Uma coleção de recursos para o provedor.</span><span class="sxs-lookup"><span data-stu-id="bc67f-124">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="bc67f-125">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="bc67f-125">roleAssignments</span></span> |<span data-ttu-id="bc67f-126">coleção [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="bc67f-126">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="bc67f-127">Uma coleção de atribuições de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="bc67f-127">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="bc67f-128">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="bc67f-128">roleDefinitions</span></span> |<span data-ttu-id="bc67f-129">coleção [governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bc67f-129">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="bc67f-130">Uma coleção de defintions de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="bc67f-130">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="bc67f-131">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="bc67f-131">roleAssignmentRequests</span></span> |<span data-ttu-id="bc67f-132">coleção [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="bc67f-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="bc67f-133">Uma coleção de solicitações de atribuição de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="bc67f-133">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="bc67f-134">roleSettings</span><span class="sxs-lookup"><span data-stu-id="bc67f-134">roleSettings</span></span> |<span data-ttu-id="bc67f-135">coleção [governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="bc67f-135">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="bc67f-136">Uma coleção de configurações de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="bc67f-136">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="bc67f-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc67f-137">JSON representation</span></span>

<span data-ttu-id="bc67f-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc67f-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedAccess"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
