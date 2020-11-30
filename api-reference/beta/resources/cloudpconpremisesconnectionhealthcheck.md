---
title: tipo de recurso cloudPcOnPremisesConnectionHealthCheck
description: O resultado de uma verificação de integridade de conexão local do PC de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 188d9db2dbef3b3e731e0c95a48f6637e3e00101
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378224"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a><span data-ttu-id="678b0-103">tipo de recurso cloudPcOnPremisesConnectionHealthCheck</span><span class="sxs-lookup"><span data-stu-id="678b0-103">cloudPcOnPremisesConnectionHealthCheck resource type</span></span>

<span data-ttu-id="678b0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="678b0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="678b0-105">O resultado de uma verificação de integridade de conexão local do PC de nuvem.</span><span class="sxs-lookup"><span data-stu-id="678b0-105">The result of a cloud PC on-premises connection health check.</span></span>

## <a name="methods"></a><span data-ttu-id="678b0-106">Methods</span><span class="sxs-lookup"><span data-stu-id="678b0-106">Methods</span></span>

|<span data-ttu-id="678b0-107">Método</span><span class="sxs-lookup"><span data-stu-id="678b0-107">Method</span></span>|<span data-ttu-id="678b0-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="678b0-108">Return type</span></span>|<span data-ttu-id="678b0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="678b0-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="678b0-110">RunHealthChecks do cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="678b0-110">RunHealthChecks of cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-runhealthcheck.md)|<span data-ttu-id="678b0-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="678b0-111">None</span></span>|<span data-ttu-id="678b0-112">Execute as verificações de integridade de um [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="678b0-112">Run the health checks of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="678b0-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="678b0-113">Properties</span></span>

|<span data-ttu-id="678b0-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="678b0-114">Property</span></span>|<span data-ttu-id="678b0-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="678b0-115">Type</span></span>|<span data-ttu-id="678b0-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="678b0-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="678b0-117">displayName</span><span class="sxs-lookup"><span data-stu-id="678b0-117">displayName</span></span>|<span data-ttu-id="678b0-118">String</span><span class="sxs-lookup"><span data-stu-id="678b0-118">String</span></span>|<span data-ttu-id="678b0-119">O nome de exibição deste item de verificação de integridade.</span><span class="sxs-lookup"><span data-stu-id="678b0-119">The display name for this health check item.</span></span>|
|<span data-ttu-id="678b0-120">status</span><span class="sxs-lookup"><span data-stu-id="678b0-120">status</span></span>|<span data-ttu-id="678b0-121">cloudPcOnPremisesConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="678b0-121">cloudPcOnPremisesConnectionStatus</span></span>|<span data-ttu-id="678b0-122">O status do item de verificação de integridade.</span><span class="sxs-lookup"><span data-stu-id="678b0-122">The status of the health check item.</span></span> <span data-ttu-id="678b0-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="678b0-123">Read-only.</span></span> <span data-ttu-id="678b0-124">Os valores possíveis são: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="678b0-124">Possible values are: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.</span></span>|
|<span data-ttu-id="678b0-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="678b0-125">startDateTime</span></span>|<span data-ttu-id="678b0-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="678b0-126">DateTimeOffset</span></span>|<span data-ttu-id="678b0-127">A hora de início do item de verificação de integridade.</span><span class="sxs-lookup"><span data-stu-id="678b0-127">The start time of the health check item.</span></span> <span data-ttu-id="678b0-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="678b0-128">Read-only.</span></span>|
|<span data-ttu-id="678b0-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="678b0-129">endDateTime</span></span>|<span data-ttu-id="678b0-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="678b0-130">DateTimeOffset</span></span>|<span data-ttu-id="678b0-131">A hora de término do item de verificação de integridade.</span><span class="sxs-lookup"><span data-stu-id="678b0-131">The end time of the health check item.</span></span> <span data-ttu-id="678b0-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="678b0-132">Read-only.</span></span>|
|<span data-ttu-id="678b0-133">Error</span><span class="sxs-lookup"><span data-stu-id="678b0-133">errorType</span></span>|<span data-ttu-id="678b0-134">cloudPcOnPremisesConnectionHealthCheckErrorType</span><span class="sxs-lookup"><span data-stu-id="678b0-134">cloudPcOnPremisesConnectionHealthCheckErrorType</span></span>|<span data-ttu-id="678b0-135">O tipo de erro que ocorreu durante esta verificação de integridade.</span><span class="sxs-lookup"><span data-stu-id="678b0-135">The type of error that occurred during this health check.</span></span> <span data-ttu-id="678b0-136">Os valores possíveis são: `DnsCheckFqdnNotFound`, `DnsCheckUnknownError`, `AdJoinCheckFqdnNotFound`, `AdJoinCheckIncorrectCredentials`, `AdJoinCheckOrganizationalUnitNotFound`, `AdJoinCheckOrganizationalUnitIncorrectFormat`, `AdJoinCheckUnknownError`, `EndpointConnectivityCheckUrlNotWhitelisted`, `EndpointConnectivityCheckUnknownError`, `AadConnectivityCheckUnknownError`.</span><span class="sxs-lookup"><span data-stu-id="678b0-136">Possible values are: `DnsCheckFqdnNotFound`, `DnsCheckUnknownError`, `AdJoinCheckFqdnNotFound`, `AdJoinCheckIncorrectCredentials`, `AdJoinCheckOrganizationalUnitNotFound`, `AdJoinCheckOrganizationalUnitIncorrectFormat`, `AdJoinCheckUnknownError`, `EndpointConnectivityCheckUrlNotWhitelisted`, `EndpointConnectivityCheckUnknownError`, `AadConnectivityCheckUnknownError`.</span></span>|
|<span data-ttu-id="678b0-137">recomendado</span><span class="sxs-lookup"><span data-stu-id="678b0-137">recommendedAction</span></span>|<span data-ttu-id="678b0-138">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="678b0-138">String</span></span>|<span data-ttu-id="678b0-139">A ação recomendada para corrigir o erro correspondente.</span><span class="sxs-lookup"><span data-stu-id="678b0-139">The recommended action to fix the corresponding error.</span></span>|
|<span data-ttu-id="678b0-140">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="678b0-140">additionalDetails</span></span>|<span data-ttu-id="678b0-141">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="678b0-141">String</span></span>|<span data-ttu-id="678b0-142">Detalhes adicionais sobre a verificação de integridade ou a ação recomendada.</span><span class="sxs-lookup"><span data-stu-id="678b0-142">Additional details about the health check or the recommended action.</span></span>|

## <a name="relationships"></a><span data-ttu-id="678b0-143">Relações</span><span class="sxs-lookup"><span data-stu-id="678b0-143">Relationships</span></span>

<span data-ttu-id="678b0-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="678b0-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="678b0-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="678b0-145">JSON representation</span></span>

<span data-ttu-id="678b0-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="678b0-146">The following is a JSON representation of the resource.</span></span>
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
