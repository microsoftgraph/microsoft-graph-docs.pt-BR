---
title: tipo de recurso privilegedAccess
description: " por exemplo, `privilegedAccess/azureResources` representa o PIM que gerencia o acesso privilegiado aos recursos do Azure."
localization_priority: Normal
ms.openlocfilehash: 9ac8ab596906509bc0303f9a70794b6484759cc2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563640"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="74cb2-103">tipo de recurso privilegedAccess</span><span class="sxs-lookup"><span data-stu-id="74cb2-103">privilegedAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74cb2-104">Representa um grupo de funcionalidades fornecidas pelo serviço de gerenciamento de identidade privilegiado (PIM).</span><span class="sxs-lookup"><span data-stu-id="74cb2-104">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="74cb2-105">Instâncias diferentes de `privilegedAccess` representar diferentes provedores gerenciados pelo PIM; por exemplo, `privilegedAccess/azureResources` representa o PIM que gerencia o acesso privilegiado aos recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="74cb2-105">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="74cb2-106">`privilegedAccess`é somente leitura por enquanto.</span><span class="sxs-lookup"><span data-stu-id="74cb2-106">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="74cb2-107">`POST` `DELETE` Nenhuma operação é suportada no conjunto de `privilegedAccess` `PUT` `PATCH`entidades.</span><span class="sxs-lookup"><span data-stu-id="74cb2-107">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="74cb2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74cb2-108">Properties</span></span>
| <span data-ttu-id="74cb2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74cb2-109">Property</span></span>  | <span data-ttu-id="74cb2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="74cb2-110">Type</span></span>      |<span data-ttu-id="74cb2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="74cb2-111">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="74cb2-112">id</span><span class="sxs-lookup"><span data-stu-id="74cb2-112">id</span></span>         |<span data-ttu-id="74cb2-113">String</span><span class="sxs-lookup"><span data-stu-id="74cb2-113">String</span></span>     |<span data-ttu-id="74cb2-114">A ID do provedor gerenciado pelo PIM.</span><span class="sxs-lookup"><span data-stu-id="74cb2-114">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="74cb2-115">displayName</span><span class="sxs-lookup"><span data-stu-id="74cb2-115">displayName</span></span>|<span data-ttu-id="74cb2-116">String</span><span class="sxs-lookup"><span data-stu-id="74cb2-116">String</span></span>     |<span data-ttu-id="74cb2-117">O nome de exibição do provedor gerenciado pelo PIM.</span><span class="sxs-lookup"><span data-stu-id="74cb2-117">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="74cb2-118">Relações</span><span class="sxs-lookup"><span data-stu-id="74cb2-118">Relationships</span></span>
| <span data-ttu-id="74cb2-119">Relação</span><span class="sxs-lookup"><span data-stu-id="74cb2-119">Relationship</span></span>   | <span data-ttu-id="74cb2-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="74cb2-120">Type</span></span>                                         |<span data-ttu-id="74cb2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="74cb2-121">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="74cb2-122">recursos</span><span class="sxs-lookup"><span data-stu-id="74cb2-122">resources</span></span>       |<span data-ttu-id="74cb2-123">coleção [entidadegovernanceresource](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="74cb2-123">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="74cb2-124">Uma coleção de recursos para o provedor.</span><span class="sxs-lookup"><span data-stu-id="74cb2-124">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="74cb2-125">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="74cb2-125">roleAssignments</span></span> |<span data-ttu-id="74cb2-126">coleção [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="74cb2-126">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="74cb2-127">Uma coleção de atribuições de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="74cb2-127">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="74cb2-128">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="74cb2-128">roleDefinitions</span></span> |<span data-ttu-id="74cb2-129">coleção [governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="74cb2-129">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="74cb2-130">Uma coleção de defintions de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="74cb2-130">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="74cb2-131">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="74cb2-131">roleAssignmentRequests</span></span> |<span data-ttu-id="74cb2-132">coleção [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="74cb2-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="74cb2-133">Uma coleção de solicitações de atribuição de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="74cb2-133">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="74cb2-134">roleSettings</span><span class="sxs-lookup"><span data-stu-id="74cb2-134">roleSettings</span></span> |<span data-ttu-id="74cb2-135">coleção [governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="74cb2-135">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="74cb2-136">Uma coleção de configurações de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="74cb2-136">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="74cb2-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74cb2-137">JSON representation</span></span>

<span data-ttu-id="74cb2-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74cb2-138">Here is a JSON representation of the resource.</span></span>

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
