---
title: Tipo de recurso cloudPcOnPremisesConnectionHealthCheck
description: O resultado de uma verificação de saúde de conexão local do computador na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: e79f73bbe1a493e581a35db5fec396d752ff08d1
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844603"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a><span data-ttu-id="0ecf5-103">Tipo de recurso cloudPcOnPremisesConnectionHealthCheck</span><span class="sxs-lookup"><span data-stu-id="0ecf5-103">cloudPcOnPremisesConnectionHealthCheck resource type</span></span>

<span data-ttu-id="0ecf5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ecf5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ecf5-105">O resultado de uma verificação de saúde de conexão local do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="0ecf5-105">The result of a cloud PC on-premises connection health check.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="0ecf5-106">Methods</span><span class="sxs-lookup"><span data-stu-id="0ecf5-106">Methods</span></span>

|<span data-ttu-id="0ecf5-107">Método</span><span class="sxs-lookup"><span data-stu-id="0ecf5-107">Method</span></span>|<span data-ttu-id="0ecf5-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0ecf5-108">Return type</span></span>|<span data-ttu-id="0ecf5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ecf5-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0ecf5-110">RunHealthChecks of cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="0ecf5-110">RunHealthChecks of cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-runhealthcheck.md)|<span data-ttu-id="0ecf5-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0ecf5-111">None</span></span>|<span data-ttu-id="0ecf5-112">Execute as verificações de saúde de [uma cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecf5-112">Run the health checks of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="0ecf5-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ecf5-113">Properties</span></span>

|<span data-ttu-id="0ecf5-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ecf5-114">Property</span></span>|<span data-ttu-id="0ecf5-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ecf5-115">Type</span></span>|<span data-ttu-id="0ecf5-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ecf5-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ecf5-117">displayName</span><span class="sxs-lookup"><span data-stu-id="0ecf5-117">displayName</span></span>|<span data-ttu-id="0ecf5-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ecf5-118">String</span></span>|<span data-ttu-id="0ecf5-119">O nome de exibição deste item de verificação de saúde.</span><span class="sxs-lookup"><span data-stu-id="0ecf5-119">The display name for this health check item.</span></span>|
|<span data-ttu-id="0ecf5-120">status</span><span class="sxs-lookup"><span data-stu-id="0ecf5-120">status</span></span>|<span data-ttu-id="0ecf5-121">cloudPcOnPremisesConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="0ecf5-121">cloudPcOnPremisesConnectionStatus</span></span>|<span data-ttu-id="0ecf5-122">O status do item de verificação de saúde.</span><span class="sxs-lookup"><span data-stu-id="0ecf5-122">The status of the health check item.</span></span> <span data-ttu-id="0ecf5-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ecf5-123">Read-only.</span></span> <span data-ttu-id="0ecf5-124">Os valores possíveis são: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0ecf5-124">Possible values are: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.</span></span>|
|<span data-ttu-id="0ecf5-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0ecf5-125">startDateTime</span></span>|<span data-ttu-id="0ecf5-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ecf5-126">DateTimeOffset</span></span>|<span data-ttu-id="0ecf5-127">A hora de início do item de verificação de saúde.</span><span class="sxs-lookup"><span data-stu-id="0ecf5-127">The start time of the health check item.</span></span> <span data-ttu-id="0ecf5-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ecf5-128">Read-only.</span></span>|
|<span data-ttu-id="0ecf5-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0ecf5-129">endDateTime</span></span>|<span data-ttu-id="0ecf5-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ecf5-130">DateTimeOffset</span></span>|<span data-ttu-id="0ecf5-131">A hora de término do item de verificação de saúde.</span><span class="sxs-lookup"><span data-stu-id="0ecf5-131">The end time of the health check item.</span></span> <span data-ttu-id="0ecf5-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ecf5-132">Read-only.</span></span>|
|<span data-ttu-id="0ecf5-133">errorType</span><span class="sxs-lookup"><span data-stu-id="0ecf5-133">errorType</span></span>|<span data-ttu-id="0ecf5-134">cloudPcOnPremisesConnectionHealthCheckErrorType</span><span class="sxs-lookup"><span data-stu-id="0ecf5-134">cloudPcOnPremisesConnectionHealthCheckErrorType</span></span>|<span data-ttu-id="0ecf5-135">O tipo de erro que ocorreu durante a verificação de saúde.</span><span class="sxs-lookup"><span data-stu-id="0ecf5-135">The type of error that occurred during this health check.</span></span> <span data-ttu-id="0ecf5-136">Os valores possíveis `DnsCheckFqdnNotFound` são: `DnsCheckUnknownError` , , , , `AdJoinCheckFqdnNotFound` , `AdJoinCheckIncorrectCredentials` `AdJoinCheckOrganizationalUnitNotFound` `AdJoinCheckOrganizationalUnitIncorrectFormat` `AdJoinCheckUnknownError` `EndpointConnectivityCheckUrlNotWhitelisted` , `EndpointConnectivityCheckUnknownError` `AadConnectivityCheckUnknownError` `ResourceAvailabilityCheckNoSubnetIP` `resourceAvailabilityCheckSubscriptionDisabled` `resourceAvailabilityCheckUnknownError` `permissionCheckNoSubscriptionReaderRole` `permissionCheckNoResourceGroupOwnerRole` `permissionCheckNoVNetContributorRole` `permissionCheckUnknownError` `internalServerUnknownError` .</span><span class="sxs-lookup"><span data-stu-id="0ecf5-136">Possible values are: `DnsCheckFqdnNotFound`, `DnsCheckUnknownError`, `AdJoinCheckFqdnNotFound`, `AdJoinCheckIncorrectCredentials`, `AdJoinCheckOrganizationalUnitNotFound`, `AdJoinCheckOrganizationalUnitIncorrectFormat`, `AdJoinCheckUnknownError`, `EndpointConnectivityCheckUrlNotWhitelisted`, `EndpointConnectivityCheckUnknownError`, `AadConnectivityCheckUnknownError`, `ResourceAvailabilityCheckNoSubnetIP`, `resourceAvailabilityCheckSubscriptionDisabled`, `resourceAvailabilityCheckUnknownError`,`permissionCheckNoSubscriptionReaderRole`, `permissionCheckNoResourceGroupOwnerRole`, `permissionCheckNoVNetContributorRole`, `permissionCheckUnknownError`, `internalServerUnknownError`.</span></span>|
|<span data-ttu-id="0ecf5-137">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="0ecf5-137">recommendedAction</span></span>|<span data-ttu-id="0ecf5-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ecf5-138">String</span></span>|<span data-ttu-id="0ecf5-139">A ação recomendada para corrigir o erro correspondente.</span><span class="sxs-lookup"><span data-stu-id="0ecf5-139">The recommended action to fix the corresponding error.</span></span>|
|<span data-ttu-id="0ecf5-140">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="0ecf5-140">additionalDetails</span></span>|<span data-ttu-id="0ecf5-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ecf5-141">String</span></span>|<span data-ttu-id="0ecf5-142">Detalhes adicionais sobre a verificação de saúde ou a ação recomendada.</span><span class="sxs-lookup"><span data-stu-id="0ecf5-142">Additional details about the health check or the recommended action.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ecf5-143">Relações</span><span class="sxs-lookup"><span data-stu-id="0ecf5-143">Relationships</span></span>

<span data-ttu-id="0ecf5-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0ecf5-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ecf5-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ecf5-145">JSON representation</span></span>

<span data-ttu-id="0ecf5-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ecf5-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
  "displayName": "String",
  "status": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "errorType": "String",
  "recommendedAction": "String",
  "additionalDetails": "String"
}
```
