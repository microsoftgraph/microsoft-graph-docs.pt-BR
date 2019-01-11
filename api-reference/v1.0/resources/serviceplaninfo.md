---
title: Tipo de recurso servicePlanInfo
description: Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade subscribedSku é uma coleção de **servicePlanInfo**.
localization_priority: Normal
ms.openlocfilehash: 837170881c7c093d26c5b59662e20e87b399a029
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845448"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="e1cbf-104">Tipo de recurso servicePlanInfo</span><span class="sxs-lookup"><span data-stu-id="e1cbf-104">servicePlanInfo resource type</span></span>

<span data-ttu-id="e1cbf-p102">Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade [subscribedSku](subscribedsku.md) é uma coleção de **servicePlanInfo**.</span><span class="sxs-lookup"><span data-stu-id="e1cbf-p102">Contains information about a service plan associated with a subscribed SKU. The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="e1cbf-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1cbf-107">Properties</span></span>
| <span data-ttu-id="e1cbf-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1cbf-108">Property</span></span>     | <span data-ttu-id="e1cbf-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1cbf-109">Type</span></span>   |<span data-ttu-id="e1cbf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1cbf-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1cbf-111">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="e1cbf-111">servicePlanId</span></span>|<span data-ttu-id="e1cbf-112">Guid</span><span class="sxs-lookup"><span data-stu-id="e1cbf-112">Guid</span></span>|<span data-ttu-id="e1cbf-113">O identificador exclusivo do plano de serviços.</span><span class="sxs-lookup"><span data-stu-id="e1cbf-113">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="e1cbf-114">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="e1cbf-114">servicePlanName</span></span>|<span data-ttu-id="e1cbf-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1cbf-115">String</span></span>|<span data-ttu-id="e1cbf-116">O nome do plano de serviços.</span><span class="sxs-lookup"><span data-stu-id="e1cbf-116">The name of the service plan.</span></span>|
|<span data-ttu-id="e1cbf-117">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="e1cbf-117">provisioningStatus</span></span>|<span data-ttu-id="e1cbf-118">String</span><span class="sxs-lookup"><span data-stu-id="e1cbf-118">String</span></span>|<span data-ttu-id="e1cbf-p103">O status de provisionamento do plano de serviços. Valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="e1cbf-p103">The provisioning status of the service plan. Possible values:</span></span><br/><span data-ttu-id="e1cbf-121">"Success" – o serviço está totalmente provisionado.</span><span class="sxs-lookup"><span data-stu-id="e1cbf-121">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="e1cbf-122">“Disabled” – o serviço foi desabilitado.</span><span class="sxs-lookup"><span data-stu-id="e1cbf-122">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="e1cbf-123">"PendingInput" – o serviço ainda não está provisionado; aguardando confirmação do serviço.</span><span class="sxs-lookup"><span data-stu-id="e1cbf-123">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="e1cbf-124">"PendingActivation" – o serviço está provisionado, mas requer ativação explícita pelo administrador (por exemplo, plano de serviço do Intune_O365)</span><span class="sxs-lookup"><span data-stu-id="e1cbf-124">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan)</span></span><br/><span data-ttu-id="e1cbf-125">"PendingProvisioning" – a Microsoft adicionou um novo serviço ao SKU do produto e ele não foi ativado no locatário ainda.</span><span class="sxs-lookup"><span data-stu-id="e1cbf-125">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="e1cbf-126">appliesTo</span><span class="sxs-lookup"><span data-stu-id="e1cbf-126">appliesTo</span></span>|<span data-ttu-id="e1cbf-127">String</span><span class="sxs-lookup"><span data-stu-id="e1cbf-127">String</span></span>|<span data-ttu-id="e1cbf-p104">O objeto ao qual o plano de serviço pode ser atribuído. Valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="e1cbf-p104">The object the service plan can be assigned to. Possible values:</span></span><br/><span data-ttu-id="e1cbf-130">"Usuário" – o plano de serviço pode ser atribuído a usuários individuais.</span><span class="sxs-lookup"><span data-stu-id="e1cbf-130">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="e1cbf-131">"Empresa" – o plano de serviço pode ser atribuído a todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="e1cbf-131">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1cbf-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1cbf-132">JSON representation</span></span>

<span data-ttu-id="e1cbf-133">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e1cbf-133">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
