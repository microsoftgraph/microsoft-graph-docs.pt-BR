---
title: Tipo de recurso servicePlanInfo
description: Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade subscribedSku é uma coleção de **servicePlanInfo**.
localization_priority: Normal
ms.openlocfilehash: f0cb96a11b280fcda4e97a6dad30a9e5200c2e88
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842676"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="00339-104">Tipo de recurso servicePlanInfo</span><span class="sxs-lookup"><span data-stu-id="00339-104">servicePlanInfo resource type</span></span>

> <span data-ttu-id="00339-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="00339-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00339-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="00339-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00339-p103">Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade [subscribedSku](subscribedsku.md) é uma coleção de **servicePlanInfo**.</span><span class="sxs-lookup"><span data-stu-id="00339-p103">Contains information about a service plan associated with a subscribed SKU. The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="00339-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00339-109">Properties</span></span>
| <span data-ttu-id="00339-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00339-110">Property</span></span>     | <span data-ttu-id="00339-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="00339-111">Type</span></span>   |<span data-ttu-id="00339-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="00339-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00339-113">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="00339-113">servicePlanId</span></span>|<span data-ttu-id="00339-114">Guid</span><span class="sxs-lookup"><span data-stu-id="00339-114">Guid</span></span>|<span data-ttu-id="00339-115">O identificador exclusivo do plano de serviços.</span><span class="sxs-lookup"><span data-stu-id="00339-115">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="00339-116">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="00339-116">servicePlanName</span></span>|<span data-ttu-id="00339-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00339-117">String</span></span>|<span data-ttu-id="00339-118">O nome do plano de serviços.</span><span class="sxs-lookup"><span data-stu-id="00339-118">The name of the service plan.</span></span>|
|<span data-ttu-id="00339-119">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="00339-119">provisioningStatus</span></span>|<span data-ttu-id="00339-120">String</span><span class="sxs-lookup"><span data-stu-id="00339-120">String</span></span>|<span data-ttu-id="00339-p104">O status de provisionamento do plano de serviços. Valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="00339-p104">The provisioning status of the service plan. Possible values:</span></span><br/><span data-ttu-id="00339-123">"Success" – o serviço está totalmente provisionado.</span><span class="sxs-lookup"><span data-stu-id="00339-123">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="00339-124">“Disabled” – o serviço foi desabilitado.</span><span class="sxs-lookup"><span data-stu-id="00339-124">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="00339-125">"PendingInput" – o serviço ainda não está provisionado; aguardando confirmação do serviço.</span><span class="sxs-lookup"><span data-stu-id="00339-125">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="00339-126">"PendingActivation" - serviço é provisionado, mas requer ativação explícita pelo administrador (por exemplo, plano de serviço Intune_O365).</span><span class="sxs-lookup"><span data-stu-id="00339-126">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan).</span></span><br/><span data-ttu-id="00339-127">"PendingProvisioning" – a Microsoft adicionou um novo serviço ao SKU do produto e ele não foi ativado no locatário ainda.</span><span class="sxs-lookup"><span data-stu-id="00339-127">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="00339-128">appliesTo</span><span class="sxs-lookup"><span data-stu-id="00339-128">appliesTo</span></span>|<span data-ttu-id="00339-129">String</span><span class="sxs-lookup"><span data-stu-id="00339-129">String</span></span>|<span data-ttu-id="00339-p105">O objeto ao qual o plano de serviço pode ser atribuído. Valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="00339-p105">The object the service plan can be assigned to. Possible values:</span></span><br/><span data-ttu-id="00339-132">"Usuário" – o plano de serviço pode ser atribuído a usuários individuais.</span><span class="sxs-lookup"><span data-stu-id="00339-132">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="00339-133">"Empresa" – o plano de serviço pode ser atribuído a todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="00339-133">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00339-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00339-134">JSON representation</span></span>

<span data-ttu-id="00339-135">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="00339-135">Here is a JSON representation of the resource</span></span>

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
