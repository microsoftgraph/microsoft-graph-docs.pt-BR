---
title: Tipo de recurso privilegedAccess
description: " por exemplo, representa `privilegedAccess/azureResources` o PIM gerenciando o acesso privilegiado aos recursos do Azure."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 8a144ba13974a728b4e89fc661f34f20e8157689
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136616"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="4fd45-103">Tipo de recurso privilegedAccess</span><span class="sxs-lookup"><span data-stu-id="4fd45-103">privilegedAccess resource type</span></span>

<span data-ttu-id="4fd45-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fd45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fd45-105">Representa um grupo de funcionalidades fornecidas pelo serviço privileged Identity Management (PIM).</span><span class="sxs-lookup"><span data-stu-id="4fd45-105">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="4fd45-106">Diferentes instâncias de representam diferentes provedores gerenciados por PIM; por exemplo, representa o PIM gerenciando o acesso privilegiado `privilegedAccess` `privilegedAccess/azureResources` aos recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="4fd45-106">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="4fd45-107">`privilegedAccess` é somente leitura por enquanto.</span><span class="sxs-lookup"><span data-stu-id="4fd45-107">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="4fd45-108">Não `POST` , ou operações são `PUT` `PATCH` `DELETE` suportadas no conjunto de `privilegedAccess` entidades.</span><span class="sxs-lookup"><span data-stu-id="4fd45-108">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="4fd45-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4fd45-109">Properties</span></span>
| <span data-ttu-id="4fd45-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4fd45-110">Property</span></span>  | <span data-ttu-id="4fd45-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4fd45-111">Type</span></span>      |<span data-ttu-id="4fd45-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fd45-112">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="4fd45-113">id</span><span class="sxs-lookup"><span data-stu-id="4fd45-113">id</span></span>         |<span data-ttu-id="4fd45-114">String</span><span class="sxs-lookup"><span data-stu-id="4fd45-114">String</span></span>     |<span data-ttu-id="4fd45-115">A id do provedor gerenciado pelo PIM.</span><span class="sxs-lookup"><span data-stu-id="4fd45-115">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="4fd45-116">displayName</span><span class="sxs-lookup"><span data-stu-id="4fd45-116">displayName</span></span>|<span data-ttu-id="4fd45-117">String</span><span class="sxs-lookup"><span data-stu-id="4fd45-117">String</span></span>     |<span data-ttu-id="4fd45-118">O nome de exibição do provedor gerenciado pelo PIM.</span><span class="sxs-lookup"><span data-stu-id="4fd45-118">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="4fd45-119">Relações</span><span class="sxs-lookup"><span data-stu-id="4fd45-119">Relationships</span></span>
| <span data-ttu-id="4fd45-120">Relação</span><span class="sxs-lookup"><span data-stu-id="4fd45-120">Relationship</span></span>   | <span data-ttu-id="4fd45-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4fd45-121">Type</span></span>                                         |<span data-ttu-id="4fd45-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fd45-122">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="4fd45-123">recursos</span><span class="sxs-lookup"><span data-stu-id="4fd45-123">resources</span></span>       |<span data-ttu-id="4fd45-124">[Coleção governanceResource](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="4fd45-124">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="4fd45-125">Uma coleção de recursos para o provedor.</span><span class="sxs-lookup"><span data-stu-id="4fd45-125">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="4fd45-126">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="4fd45-126">roleAssignments</span></span> |<span data-ttu-id="4fd45-127">[Coleção governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4fd45-127">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="4fd45-128">Uma coleção de atribuições de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="4fd45-128">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="4fd45-129">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="4fd45-129">roleDefinitions</span></span> |<span data-ttu-id="4fd45-130">[Coleção governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4fd45-130">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="4fd45-131">Uma coleção de definições de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="4fd45-131">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="4fd45-132">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="4fd45-132">roleAssignmentRequests</span></span> |<span data-ttu-id="4fd45-133">[Coleção governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="4fd45-133">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="4fd45-134">Uma coleção de solicitações de atribuição de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="4fd45-134">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="4fd45-135">roleSettings</span><span class="sxs-lookup"><span data-stu-id="4fd45-135">roleSettings</span></span> |<span data-ttu-id="4fd45-136">[Coleção governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="4fd45-136">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="4fd45-137">Uma coleção de configurações de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="4fd45-137">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4fd45-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4fd45-138">JSON representation</span></span>

<span data-ttu-id="4fd45-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4fd45-139">Here is a JSON representation of the resource.</span></span>

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


