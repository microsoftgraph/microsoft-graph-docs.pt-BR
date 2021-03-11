---
title: Tipo de recurso servicePlanInfo
description: Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade subscribedSku é uma coleção de **servicePlanInfo**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: jpettere
ms.openlocfilehash: 7188c38c8114008ed124440512646ecd53a9705a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718448"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="0bc2a-104">Tipo de recurso servicePlanInfo</span><span class="sxs-lookup"><span data-stu-id="0bc2a-104">servicePlanInfo resource type</span></span>

<span data-ttu-id="0bc2a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bc2a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bc2a-106">Contém informações sobre um plano de serviço associado a uma SKU inscrita.</span><span class="sxs-lookup"><span data-stu-id="0bc2a-106">Contains information about a service plan associated with a subscribed SKU.</span></span> <span data-ttu-id="0bc2a-107">A propriedade **servicePlans** da entidade [subscribedSku](subscribedsku.md) é uma coleção de **servicePlanInfo**.</span><span class="sxs-lookup"><span data-stu-id="0bc2a-107">The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="0bc2a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0bc2a-108">Properties</span></span>
| <span data-ttu-id="0bc2a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bc2a-109">Property</span></span>     | <span data-ttu-id="0bc2a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bc2a-110">Type</span></span>   |<span data-ttu-id="0bc2a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bc2a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0bc2a-112">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="0bc2a-112">servicePlanId</span></span>|<span data-ttu-id="0bc2a-113">Guid</span><span class="sxs-lookup"><span data-stu-id="0bc2a-113">Guid</span></span>|<span data-ttu-id="0bc2a-114">O identificador exclusivo do plano de serviços.</span><span class="sxs-lookup"><span data-stu-id="0bc2a-114">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="0bc2a-115">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="0bc2a-115">servicePlanName</span></span>|<span data-ttu-id="0bc2a-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bc2a-116">String</span></span>|<span data-ttu-id="0bc2a-117">O nome do plano de serviços.</span><span class="sxs-lookup"><span data-stu-id="0bc2a-117">The name of the service plan.</span></span>|
|<span data-ttu-id="0bc2a-118">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="0bc2a-118">provisioningStatus</span></span>|<span data-ttu-id="0bc2a-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bc2a-119">String</span></span>|<span data-ttu-id="0bc2a-120">O status de provisionamento do plano de serviços.</span><span class="sxs-lookup"><span data-stu-id="0bc2a-120">The provisioning status of the service plan.</span></span> <span data-ttu-id="0bc2a-121">Valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="0bc2a-121">Possible values:</span></span><br/><span data-ttu-id="0bc2a-122">"Sucesso" - O serviço está totalmente provisionado.</span><span class="sxs-lookup"><span data-stu-id="0bc2a-122">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="0bc2a-123">"Desabilitado" - O serviço foi desabilitado.</span><span class="sxs-lookup"><span data-stu-id="0bc2a-123">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="0bc2a-124">"PendingInput" - O serviço ainda não foi provisionado; aguardando confirmação do serviço.</span><span class="sxs-lookup"><span data-stu-id="0bc2a-124">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="0bc2a-125">"PendingActivation" - O serviço é provisionado, mas exige ativação explícita pelo administrador (por exemplo, Intune_O365 plano de serviço).</span><span class="sxs-lookup"><span data-stu-id="0bc2a-125">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan).</span></span><br/><span data-ttu-id="0bc2a-126">"PendingProvisioning" - A Microsoft adicionou um novo serviço à SKU do produto e ainda não foi ativado no locatário.</span><span class="sxs-lookup"><span data-stu-id="0bc2a-126">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="0bc2a-127">appliesTo</span><span class="sxs-lookup"><span data-stu-id="0bc2a-127">appliesTo</span></span>|<span data-ttu-id="0bc2a-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bc2a-128">String</span></span>|<span data-ttu-id="0bc2a-129">O objeto ao que o plano de serviço pode ser atribuído.</span><span class="sxs-lookup"><span data-stu-id="0bc2a-129">The object the service plan can be assigned to.</span></span> <span data-ttu-id="0bc2a-130">Valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="0bc2a-130">Possible values:</span></span><br/><span data-ttu-id="0bc2a-131">"Usuário" - o plano de serviço pode ser atribuído a usuários individuais.</span><span class="sxs-lookup"><span data-stu-id="0bc2a-131">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="0bc2a-132">"Empresa" - o plano de serviço pode ser atribuído a todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="0bc2a-132">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0bc2a-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0bc2a-133">JSON representation</span></span>

<span data-ttu-id="0bc2a-134">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0bc2a-134">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


