---
title: Tipo de recurso servicePlanInfo
description: Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade subscribedSku é uma coleção de **servicePlanInfo**.
localization_priority: Normal
author: krbain
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6176174a046618176627e8bbe7b8a984c58a3c22
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991856"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="ab320-104">Tipo de recurso servicePlanInfo</span><span class="sxs-lookup"><span data-stu-id="ab320-104">servicePlanInfo resource type</span></span>

<span data-ttu-id="ab320-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab320-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab320-106">Contém informações sobre um plano de serviço associado a uma SKU inscrita.</span><span class="sxs-lookup"><span data-stu-id="ab320-106">Contains information about a service plan associated with a subscribed SKU.</span></span> <span data-ttu-id="ab320-107">A propriedade **servicePlans** da entidade [subscribedSku](subscribedsku.md) é uma coleção de **servicePlanInfo**.</span><span class="sxs-lookup"><span data-stu-id="ab320-107">The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="ab320-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab320-108">Properties</span></span>
| <span data-ttu-id="ab320-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab320-109">Property</span></span>     | <span data-ttu-id="ab320-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab320-110">Type</span></span>   |<span data-ttu-id="ab320-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab320-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab320-112">onplanid</span><span class="sxs-lookup"><span data-stu-id="ab320-112">servicePlanId</span></span>|<span data-ttu-id="ab320-113">Guid</span><span class="sxs-lookup"><span data-stu-id="ab320-113">Guid</span></span>|<span data-ttu-id="ab320-114">O identificador exclusivo do plano de serviços.</span><span class="sxs-lookup"><span data-stu-id="ab320-114">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="ab320-115">onplanname</span><span class="sxs-lookup"><span data-stu-id="ab320-115">servicePlanName</span></span>|<span data-ttu-id="ab320-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab320-116">String</span></span>|<span data-ttu-id="ab320-117">O nome do plano de serviços.</span><span class="sxs-lookup"><span data-stu-id="ab320-117">The name of the service plan.</span></span>|
|<span data-ttu-id="ab320-118">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="ab320-118">provisioningStatus</span></span>|<span data-ttu-id="ab320-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab320-119">String</span></span>|<span data-ttu-id="ab320-120">O status de provisionamento do plano de serviços.</span><span class="sxs-lookup"><span data-stu-id="ab320-120">The provisioning status of the service plan.</span></span> <span data-ttu-id="ab320-121">Valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="ab320-121">Possible values:</span></span><br/><span data-ttu-id="ab320-122">"Success"-o serviço está totalmente provisionado.</span><span class="sxs-lookup"><span data-stu-id="ab320-122">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="ab320-123">"Disabled"-o serviço foi desabilitado.</span><span class="sxs-lookup"><span data-stu-id="ab320-123">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="ab320-124">"PendingInput" – o serviço ainda não foi provisionado; aguardando confirmação do serviço.</span><span class="sxs-lookup"><span data-stu-id="ab320-124">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="ab320-125">"PendingActivation" – o serviço é provisionado, mas requer ativação explícita por administrador (por exemplo, Intune_O365 plano de serviço)</span><span class="sxs-lookup"><span data-stu-id="ab320-125">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan)</span></span><br/><span data-ttu-id="ab320-126">"PendingProvisioning"-a Microsoft adicionou um novo serviço ao SKU do produto e ainda não foi ativado no locatário.</span><span class="sxs-lookup"><span data-stu-id="ab320-126">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="ab320-127">appliesTo</span><span class="sxs-lookup"><span data-stu-id="ab320-127">appliesTo</span></span>|<span data-ttu-id="ab320-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab320-128">String</span></span>|<span data-ttu-id="ab320-129">O objeto ao qual o plano de serviço pode ser atribuído.</span><span class="sxs-lookup"><span data-stu-id="ab320-129">The object the service plan can be assigned to.</span></span> <span data-ttu-id="ab320-130">Valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="ab320-130">Possible values:</span></span><br/><span data-ttu-id="ab320-131">"User" – o plano de serviço pode ser atribuído a usuários individuais.</span><span class="sxs-lookup"><span data-stu-id="ab320-131">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="ab320-132">"Empresa"-o plano de serviço pode ser atribuído a todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="ab320-132">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab320-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab320-133">JSON representation</span></span>

<span data-ttu-id="ab320-134">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ab320-134">Here is a JSON representation of the resource</span></span>

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

