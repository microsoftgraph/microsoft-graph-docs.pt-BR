---
title: tipo de recurso de privilegedAccess
description: " Por exemplo, `privilegedAccess/azureResources` representa PIM Gerenciando privilegiado acesso aos recursos do Windows Azure."
ms.openlocfilehash: af109c0cc355bfb282630d21cd02bb463b944f38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040767"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="3bb70-103">tipo de recurso de privilegedAccess</span><span class="sxs-lookup"><span data-stu-id="3bb70-103">privilegedAccess resource type</span></span>

> <span data-ttu-id="3bb70-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3bb70-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3bb70-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3bb70-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3bb70-106">Representa um grupo de funcionalidades fornecido pelo serviço de gerenciamento de identidade privilegiado (PIM).</span><span class="sxs-lookup"><span data-stu-id="3bb70-106">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="3bb70-107">Diferentes instâncias do `privilegedAccess` representam os diferentes provedores gerenciados por PIM; Por exemplo, `privilegedAccess/azureResources` representa PIM Gerenciando privilegiado acesso aos recursos do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="3bb70-107">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="3bb70-108">`privilegedAccess`é somente leitura por enquanto.</span><span class="sxs-lookup"><span data-stu-id="3bb70-108">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="3bb70-109">Não `POST`, `PUT`, `PATCH`, ou `DELETE` operações são compatíveis com o `privilegedAccess` conjunto de entidade.</span><span class="sxs-lookup"><span data-stu-id="3bb70-109">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="3bb70-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3bb70-110">Properties</span></span>
| <span data-ttu-id="3bb70-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3bb70-111">Property</span></span>  | <span data-ttu-id="3bb70-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bb70-112">Type</span></span>      |<span data-ttu-id="3bb70-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bb70-113">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="3bb70-114">id</span><span class="sxs-lookup"><span data-stu-id="3bb70-114">id</span></span>         |<span data-ttu-id="3bb70-115">String</span><span class="sxs-lookup"><span data-stu-id="3bb70-115">String</span></span>     |<span data-ttu-id="3bb70-116">A identificação do provedor gerenciado por PIM.</span><span class="sxs-lookup"><span data-stu-id="3bb70-116">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="3bb70-117">displayName</span><span class="sxs-lookup"><span data-stu-id="3bb70-117">displayName</span></span>|<span data-ttu-id="3bb70-118">String</span><span class="sxs-lookup"><span data-stu-id="3bb70-118">String</span></span>     |<span data-ttu-id="3bb70-119">O nome de exibição do provedor gerenciado por PIM.</span><span class="sxs-lookup"><span data-stu-id="3bb70-119">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="3bb70-120">Relações</span><span class="sxs-lookup"><span data-stu-id="3bb70-120">Relationships</span></span>
| <span data-ttu-id="3bb70-121">Relação</span><span class="sxs-lookup"><span data-stu-id="3bb70-121">Relationship</span></span>   | <span data-ttu-id="3bb70-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bb70-122">Type</span></span>                                         |<span data-ttu-id="3bb70-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bb70-123">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="3bb70-124">recursos</span><span class="sxs-lookup"><span data-stu-id="3bb70-124">resources</span></span>       |<span data-ttu-id="3bb70-125">coleção [governanceResource](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="3bb70-125">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="3bb70-126">Uma coleção de recursos para o provedor.</span><span class="sxs-lookup"><span data-stu-id="3bb70-126">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="3bb70-127">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="3bb70-127">roleAssignments</span></span> |<span data-ttu-id="3bb70-128">coleção [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3bb70-128">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="3bb70-129">Uma coleção de atribuições de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="3bb70-129">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="3bb70-130">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="3bb70-130">roleDefinitions</span></span> |<span data-ttu-id="3bb70-131">coleção [governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3bb70-131">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="3bb70-132">Uma coleção de definições de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="3bb70-132">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="3bb70-133">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="3bb70-133">roleAssignmentRequests</span></span> |<span data-ttu-id="3bb70-134">coleção [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="3bb70-134">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="3bb70-135">Uma coleção de solicitações de atribuição de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="3bb70-135">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="3bb70-136">roleSettings</span><span class="sxs-lookup"><span data-stu-id="3bb70-136">roleSettings</span></span> |<span data-ttu-id="3bb70-137">coleção [governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="3bb70-137">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="3bb70-138">Uma coleção de configurações de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="3bb70-138">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="3bb70-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3bb70-139">JSON representation</span></span>

<span data-ttu-id="3bb70-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3bb70-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
