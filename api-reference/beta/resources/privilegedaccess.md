---
title: tipo de recurso de privilegedAccess
description: " Por exemplo, `privilegedAccess/azureResources` representa PIM Gerenciando privilegiado acesso aos recursos do Windows Azure."
localization_priority: Normal
ms.openlocfilehash: 9ac8ab596906509bc0303f9a70794b6484759cc2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512924"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="3a67d-103">tipo de recurso de privilegedAccess</span><span class="sxs-lookup"><span data-stu-id="3a67d-103">privilegedAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a67d-104">Representa um grupo de funcionalidades fornecido pelo serviço de gerenciamento de identidade privilegiado (PIM).</span><span class="sxs-lookup"><span data-stu-id="3a67d-104">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="3a67d-105">Diferentes instâncias do `privilegedAccess` representam os diferentes provedores gerenciados por PIM; Por exemplo, `privilegedAccess/azureResources` representa PIM Gerenciando privilegiado acesso aos recursos do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="3a67d-105">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="3a67d-106">`privilegedAccess`é somente leitura por enquanto.</span><span class="sxs-lookup"><span data-stu-id="3a67d-106">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="3a67d-107">Não `POST`, `PUT`, `PATCH`, ou `DELETE` operações são compatíveis com o `privilegedAccess` conjunto de entidade.</span><span class="sxs-lookup"><span data-stu-id="3a67d-107">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="3a67d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a67d-108">Properties</span></span>
| <span data-ttu-id="3a67d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a67d-109">Property</span></span>  | <span data-ttu-id="3a67d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a67d-110">Type</span></span>      |<span data-ttu-id="3a67d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a67d-111">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="3a67d-112">id</span><span class="sxs-lookup"><span data-stu-id="3a67d-112">id</span></span>         |<span data-ttu-id="3a67d-113">String</span><span class="sxs-lookup"><span data-stu-id="3a67d-113">String</span></span>     |<span data-ttu-id="3a67d-114">A identificação do provedor gerenciado por PIM.</span><span class="sxs-lookup"><span data-stu-id="3a67d-114">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="3a67d-115">displayName</span><span class="sxs-lookup"><span data-stu-id="3a67d-115">displayName</span></span>|<span data-ttu-id="3a67d-116">String</span><span class="sxs-lookup"><span data-stu-id="3a67d-116">String</span></span>     |<span data-ttu-id="3a67d-117">O nome de exibição do provedor gerenciado por PIM.</span><span class="sxs-lookup"><span data-stu-id="3a67d-117">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="3a67d-118">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="3a67d-118">Relationships</span></span>
| <span data-ttu-id="3a67d-119">Relação</span><span class="sxs-lookup"><span data-stu-id="3a67d-119">Relationship</span></span>   | <span data-ttu-id="3a67d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a67d-120">Type</span></span>                                         |<span data-ttu-id="3a67d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a67d-121">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="3a67d-122">recursos</span><span class="sxs-lookup"><span data-stu-id="3a67d-122">resources</span></span>       |<span data-ttu-id="3a67d-123">coleção [governanceResource](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="3a67d-123">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="3a67d-124">Uma coleção de recursos para o provedor.</span><span class="sxs-lookup"><span data-stu-id="3a67d-124">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="3a67d-125">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="3a67d-125">roleAssignments</span></span> |<span data-ttu-id="3a67d-126">coleção [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3a67d-126">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="3a67d-127">Uma coleção de atribuições de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="3a67d-127">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="3a67d-128">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="3a67d-128">roleDefinitions</span></span> |<span data-ttu-id="3a67d-129">coleção [governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3a67d-129">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="3a67d-130">Uma coleção de definições de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="3a67d-130">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="3a67d-131">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="3a67d-131">roleAssignmentRequests</span></span> |<span data-ttu-id="3a67d-132">coleção [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="3a67d-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="3a67d-133">Uma coleção de solicitações de atribuição de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="3a67d-133">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="3a67d-134">roleSettings</span><span class="sxs-lookup"><span data-stu-id="3a67d-134">roleSettings</span></span> |<span data-ttu-id="3a67d-135">coleção [governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="3a67d-135">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="3a67d-136">Uma coleção de configurações de função para o provedor.</span><span class="sxs-lookup"><span data-stu-id="3a67d-136">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="3a67d-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a67d-137">JSON representation</span></span>

<span data-ttu-id="3a67d-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a67d-138">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
