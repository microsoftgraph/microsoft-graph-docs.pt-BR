---
title: tipo de recurso de privilegedAccess
description: " Por exemplo, `privilegedAccess/azureResources` representa PIM Gerenciando privilegiado acesso aos recursos do Windows Azure."
localization_priority: Normal
ms.openlocfilehash: f4166fb539d627730c68c7e039fd8d672ff4c785
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810049"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="a890a-103">tipo de recurso de privilegedAccess</span><span class="sxs-lookup"><span data-stu-id="a890a-103">privilegedAccess resource type</span></span>

> <span data-ttu-id="a890a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a890a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a890a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a890a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a890a-106">Representa um grupo de funcionalidades fornecido pelo serviço de gerenciamento de identidade privilegiado (PIM).</span><span class="sxs-lookup"><span data-stu-id="a890a-106">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="a890a-107">Diferentes instâncias do `privilegedAccess` representam os diferentes provedores gerenciados por PIM; Por exemplo, `privilegedAccess/azureResources` representa PIM Gerenciando privilegiado acesso aos recursos do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="a890a-107">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="a890a-108">`privilegedAccess`é somente leitura por enquanto.</span><span class="sxs-lookup"><span data-stu-id="a890a-108">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="a890a-109">Não `POST`, `PUT`, `PATCH`, ou `DELETE` operações são compatíveis com o `privilegedAccess` conjunto de entidade.</span><span class="sxs-lookup"><span data-stu-id="a890a-109">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="a890a-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a890a-110">Properties</span></span>
| <span data-ttu-id="a890a-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a890a-111">Property</span></span>  | <span data-ttu-id="a890a-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="a890a-112">Type</span></span>      |<span data-ttu-id="a890a-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="a890a-113">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="a890a-114">id</span><span class="sxs-lookup"><span data-stu-id="a890a-114">id</span></span>         |<span data-ttu-id="a890a-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a890a-115">String</span></span>     |<span data-ttu-id="a890a-116">A identificação do provedor gerenciado por PIM.</span><span class="sxs-lookup"><span data-stu-id="a890a-116">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="a890a-117">displayName</span><span class="sxs-lookup"><span data-stu-id="a890a-117">displayName</span></span>|<span data-ttu-id="a890a-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a890a-118">String</span></span>     |<span data-ttu-id="a890a-119">O nome de exibição do provedor gerenciado por PIM.</span><span class="sxs-lookup"><span data-stu-id="a890a-119">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="a890a-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a890a-120">Relationships</span></span>
| <span data-ttu-id="a890a-121">Relação</span><span class="sxs-lookup"><span data-stu-id="a890a-121">Relationship</span></span>   | <span data-ttu-id="a890a-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="a890a-122">Type</span></span>                                         |<span data-ttu-id="a890a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a890a-123">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="a890a-124">recursos</span><span class="sxs-lookup"><span data-stu-id="a890a-124">resources</span></span>       |<span data-ttu-id="a890a-125">coleção [governanceResource](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="a890a-125">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="a890a-126">Uma coleção de recursos para o provedor.</span><span class="sxs-lookup"><span data-stu-id="a890a-126">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="a890a-127">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="a890a-127">roleAssignments</span></span> |<span data-ttu-id="a890a-128">coleção [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a890a-128">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="a890a-129">Uma coleção de atribuições de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="a890a-129">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="a890a-130">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="a890a-130">roleDefinitions</span></span> |<span data-ttu-id="a890a-131">coleção [governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a890a-131">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="a890a-132">Uma coleção de definições de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="a890a-132">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="a890a-133">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="a890a-133">roleAssignmentRequests</span></span> |<span data-ttu-id="a890a-134">coleção [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="a890a-134">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="a890a-135">Uma coleção de solicitações de atribuição de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="a890a-135">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="a890a-136">roleSettings</span><span class="sxs-lookup"><span data-stu-id="a890a-136">roleSettings</span></span> |<span data-ttu-id="a890a-137">coleção [governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="a890a-137">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="a890a-138">Uma coleção de configurações de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="a890a-138">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a890a-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a890a-139">JSON representation</span></span>

<span data-ttu-id="a890a-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a890a-140">Here is a JSON representation of the resource.</span></span>

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
