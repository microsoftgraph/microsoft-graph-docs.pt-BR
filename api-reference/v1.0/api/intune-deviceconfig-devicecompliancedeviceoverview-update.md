---
title: Atualizar deviceComplianceDeviceOverview
description: Atualizar as propriedades de um objeto deviceComplianceDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 48a0722c48e384570a1e5c87c3bbf93d0147b218
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052121"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="2376b-103">Atualizar deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="2376b-103">Update deviceComplianceDeviceOverview</span></span>

<span data-ttu-id="2376b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2376b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2376b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2376b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2376b-106">Atualizar as propriedades de um objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="2376b-106">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2376b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2376b-107">Prerequisites</span></span>
<span data-ttu-id="2376b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2376b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2376b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2376b-110">Permission type</span></span>|<span data-ttu-id="2376b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2376b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2376b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2376b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2376b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2376b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2376b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2376b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2376b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2376b-115">Not supported.</span></span>|
|<span data-ttu-id="2376b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2376b-116">Application</span></span>|<span data-ttu-id="2376b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2376b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2376b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2376b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="2376b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2376b-119">Request headers</span></span>
|<span data-ttu-id="2376b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2376b-120">Header</span></span>|<span data-ttu-id="2376b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2376b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2376b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2376b-122">Authorization</span></span>|<span data-ttu-id="2376b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2376b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2376b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2376b-124">Accept</span></span>|<span data-ttu-id="2376b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2376b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2376b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2376b-126">Request body</span></span>
<span data-ttu-id="2376b-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="2376b-127">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="2376b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="2376b-128">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="2376b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2376b-129">Property</span></span>|<span data-ttu-id="2376b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2376b-130">Type</span></span>|<span data-ttu-id="2376b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2376b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2376b-132">id</span><span class="sxs-lookup"><span data-stu-id="2376b-132">id</span></span>|<span data-ttu-id="2376b-133">String</span><span class="sxs-lookup"><span data-stu-id="2376b-133">String</span></span>|<span data-ttu-id="2376b-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2376b-134">Key of the entity.</span></span>|
|<span data-ttu-id="2376b-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="2376b-135">pendingCount</span></span>|<span data-ttu-id="2376b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="2376b-136">Int32</span></span>|<span data-ttu-id="2376b-137">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="2376b-137">Number of pending devices</span></span>|
|<span data-ttu-id="2376b-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="2376b-138">notApplicableCount</span></span>|<span data-ttu-id="2376b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2376b-139">Int32</span></span>|<span data-ttu-id="2376b-140">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="2376b-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="2376b-141">successCount</span><span class="sxs-lookup"><span data-stu-id="2376b-141">successCount</span></span>|<span data-ttu-id="2376b-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2376b-142">Int32</span></span>|<span data-ttu-id="2376b-143">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="2376b-143">Number of succeeded devices</span></span>|
|<span data-ttu-id="2376b-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="2376b-144">errorCount</span></span>|<span data-ttu-id="2376b-145">Int32</span><span class="sxs-lookup"><span data-stu-id="2376b-145">Int32</span></span>|<span data-ttu-id="2376b-146">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="2376b-146">Number of error devices</span></span>|
|<span data-ttu-id="2376b-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="2376b-147">failedCount</span></span>|<span data-ttu-id="2376b-148">Int32</span><span class="sxs-lookup"><span data-stu-id="2376b-148">Int32</span></span>|<span data-ttu-id="2376b-149">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="2376b-149">Number of failed devices</span></span>|
|<span data-ttu-id="2376b-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="2376b-150">lastUpdateDateTime</span></span>|<span data-ttu-id="2376b-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2376b-151">DateTimeOffset</span></span>|<span data-ttu-id="2376b-152">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="2376b-152">Last update time</span></span>|
|<span data-ttu-id="2376b-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="2376b-153">configurationVersion</span></span>|<span data-ttu-id="2376b-154">Int32</span><span class="sxs-lookup"><span data-stu-id="2376b-154">Int32</span></span>|<span data-ttu-id="2376b-155">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="2376b-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="2376b-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="2376b-156">Response</span></span>
<span data-ttu-id="2376b-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2376b-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2376b-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2376b-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="2376b-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2376b-159">Request</span></span>
<span data-ttu-id="2376b-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2376b-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="2376b-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="2376b-161">Response</span></span>
<span data-ttu-id="2376b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2376b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "886f167b-167b-886f-7b16-6f887b166f88",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```









