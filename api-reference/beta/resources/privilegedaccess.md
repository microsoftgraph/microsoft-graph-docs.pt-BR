---
title: tipo de recurso privilegedAccess
description: " por exemplo, `privilegedAccess/azureResources` representa o PIM que gerencia o acesso privilegiado aos recursos do Azure."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: c57dd911d105ba4d096a09f9262b847db5240fa1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811446"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="87199-103">tipo de recurso privilegedAccess</span><span class="sxs-lookup"><span data-stu-id="87199-103">privilegedAccess resource type</span></span>

<span data-ttu-id="87199-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87199-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87199-105">Representa um grupo de funcionalidades fornecidas pelo serviço de gerenciamento de identidade privilegiado (PIM).</span><span class="sxs-lookup"><span data-stu-id="87199-105">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="87199-106">Diferentes instâncias de `privilegedAccess` representar provedores diferentes gerenciados pelo PIM; por exemplo, `privilegedAccess/azureResources` representa o PIM que gerencia o acesso privilegiado aos recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="87199-106">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="87199-107">`privilegedAccess` é somente leitura por enquanto.</span><span class="sxs-lookup"><span data-stu-id="87199-107">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="87199-108">Nenhuma `POST` `PUT` `PATCH` `DELETE` operação é suportada no `privilegedAccess` conjunto de entidades.</span><span class="sxs-lookup"><span data-stu-id="87199-108">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="87199-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87199-109">Properties</span></span>
| <span data-ttu-id="87199-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87199-110">Property</span></span>  | <span data-ttu-id="87199-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="87199-111">Type</span></span>      |<span data-ttu-id="87199-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="87199-112">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="87199-113">id</span><span class="sxs-lookup"><span data-stu-id="87199-113">id</span></span>         |<span data-ttu-id="87199-114">String</span><span class="sxs-lookup"><span data-stu-id="87199-114">String</span></span>     |<span data-ttu-id="87199-115">A ID do provedor gerenciado pelo PIM.</span><span class="sxs-lookup"><span data-stu-id="87199-115">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="87199-116">displayName</span><span class="sxs-lookup"><span data-stu-id="87199-116">displayName</span></span>|<span data-ttu-id="87199-117">String</span><span class="sxs-lookup"><span data-stu-id="87199-117">String</span></span>     |<span data-ttu-id="87199-118">O nome de exibição do provedor gerenciado pelo PIM.</span><span class="sxs-lookup"><span data-stu-id="87199-118">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="87199-119">Relações</span><span class="sxs-lookup"><span data-stu-id="87199-119">Relationships</span></span>
| <span data-ttu-id="87199-120">Relação</span><span class="sxs-lookup"><span data-stu-id="87199-120">Relationship</span></span>   | <span data-ttu-id="87199-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="87199-121">Type</span></span>                                         |<span data-ttu-id="87199-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="87199-122">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="87199-123">recursos</span><span class="sxs-lookup"><span data-stu-id="87199-123">resources</span></span>       |<span data-ttu-id="87199-124">coleção [entidadegovernanceresource](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="87199-124">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="87199-125">Uma coleção de recursos para o provedor.</span><span class="sxs-lookup"><span data-stu-id="87199-125">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="87199-126">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="87199-126">roleAssignments</span></span> |<span data-ttu-id="87199-127">coleção [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="87199-127">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="87199-128">Uma coleção de atribuições de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="87199-128">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="87199-129">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="87199-129">roleDefinitions</span></span> |<span data-ttu-id="87199-130">coleção [governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="87199-130">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="87199-131">Uma coleção de defintions de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="87199-131">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="87199-132">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="87199-132">roleAssignmentRequests</span></span> |<span data-ttu-id="87199-133">coleção [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="87199-133">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="87199-134">Uma coleção de solicitações de atribuição de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="87199-134">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="87199-135">roleSettings</span><span class="sxs-lookup"><span data-stu-id="87199-135">roleSettings</span></span> |<span data-ttu-id="87199-136">coleção [governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="87199-136">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="87199-137">Uma coleção de configurações de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="87199-137">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="87199-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87199-138">JSON representation</span></span>

<span data-ttu-id="87199-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87199-139">Here is a JSON representation of the resource.</span></span>

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
