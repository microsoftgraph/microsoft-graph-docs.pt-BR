---
title: tipo de recurso privilegedAccess
description: " por exemplo, `privilegedAccess/azureResources` representa o PIM que gerencia o acesso privilegiado aos recursos do Azure."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: f815228157721f6100af79f53f84abf43763f632
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070629"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="d3aac-103">tipo de recurso privilegedAccess</span><span class="sxs-lookup"><span data-stu-id="d3aac-103">privilegedAccess resource type</span></span>

<span data-ttu-id="d3aac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3aac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3aac-105">Representa um grupo de funcionalidades fornecidas pelo serviço de gerenciamento de identidade privilegiado (PIM).</span><span class="sxs-lookup"><span data-stu-id="d3aac-105">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="d3aac-106">Diferentes instâncias de `privilegedAccess` representar provedores diferentes gerenciados pelo PIM; por exemplo, `privilegedAccess/azureResources` representa o PIM que gerencia o acesso privilegiado aos recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="d3aac-106">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="d3aac-107">`privilegedAccess` é somente leitura por enquanto.</span><span class="sxs-lookup"><span data-stu-id="d3aac-107">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="d3aac-108">Nenhuma `POST` `PUT` `PATCH` `DELETE` operação é suportada no `privilegedAccess` conjunto de entidades.</span><span class="sxs-lookup"><span data-stu-id="d3aac-108">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="d3aac-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3aac-109">Properties</span></span>
| <span data-ttu-id="d3aac-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3aac-110">Property</span></span>  | <span data-ttu-id="d3aac-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3aac-111">Type</span></span>      |<span data-ttu-id="d3aac-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3aac-112">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="d3aac-113">id</span><span class="sxs-lookup"><span data-stu-id="d3aac-113">id</span></span>         |<span data-ttu-id="d3aac-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3aac-114">String</span></span>     |<span data-ttu-id="d3aac-115">A ID do provedor gerenciado pelo PIM.</span><span class="sxs-lookup"><span data-stu-id="d3aac-115">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="d3aac-116">displayName</span><span class="sxs-lookup"><span data-stu-id="d3aac-116">displayName</span></span>|<span data-ttu-id="d3aac-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3aac-117">String</span></span>     |<span data-ttu-id="d3aac-118">O nome de exibição do provedor gerenciado pelo PIM.</span><span class="sxs-lookup"><span data-stu-id="d3aac-118">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="d3aac-119">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="d3aac-119">Relationships</span></span>
| <span data-ttu-id="d3aac-120">Relação</span><span class="sxs-lookup"><span data-stu-id="d3aac-120">Relationship</span></span>   | <span data-ttu-id="d3aac-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3aac-121">Type</span></span>                                         |<span data-ttu-id="d3aac-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3aac-122">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="d3aac-123">recursos</span><span class="sxs-lookup"><span data-stu-id="d3aac-123">resources</span></span>       |<span data-ttu-id="d3aac-124">coleção [entidadegovernanceresource](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="d3aac-124">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="d3aac-125">Uma coleção de recursos para o provedor.</span><span class="sxs-lookup"><span data-stu-id="d3aac-125">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="d3aac-126">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="d3aac-126">roleAssignments</span></span> |<span data-ttu-id="d3aac-127">coleção [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d3aac-127">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="d3aac-128">Uma coleção de atribuições de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="d3aac-128">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="d3aac-129">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="d3aac-129">roleDefinitions</span></span> |<span data-ttu-id="d3aac-130">coleção [governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d3aac-130">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="d3aac-131">Uma coleção de defintions de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="d3aac-131">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="d3aac-132">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="d3aac-132">roleAssignmentRequests</span></span> |<span data-ttu-id="d3aac-133">coleção [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="d3aac-133">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="d3aac-134">Uma coleção de solicitações de atribuição de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="d3aac-134">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="d3aac-135">roleSettings</span><span class="sxs-lookup"><span data-stu-id="d3aac-135">roleSettings</span></span> |<span data-ttu-id="d3aac-136">coleção [governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="d3aac-136">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="d3aac-137">Uma coleção de configurações de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="d3aac-137">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d3aac-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3aac-138">JSON representation</span></span>

<span data-ttu-id="d3aac-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d3aac-139">Here is a JSON representation of the resource.</span></span>

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


