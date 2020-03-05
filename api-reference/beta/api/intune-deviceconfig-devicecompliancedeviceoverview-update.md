---
title: Atualizar deviceComplianceDeviceOverview
description: Atualizar as propriedades de um objeto deviceComplianceDeviceOverview.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 40f4e3843f098e81f70afba440cd2aec0a474144
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443255"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="d0808-103">Atualizar deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d0808-103">Update deviceComplianceDeviceOverview</span></span>

<span data-ttu-id="d0808-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d0808-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0808-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d0808-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0808-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d0808-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0808-107">Atualizar as propriedades de um objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="d0808-107">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0808-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d0808-108">Prerequisites</span></span>
<span data-ttu-id="d0808-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0808-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0808-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0808-111">Permission type</span></span>|<span data-ttu-id="d0808-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d0808-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0808-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0808-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d0808-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0808-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d0808-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0808-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0808-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0808-116">Not supported.</span></span>|
|<span data-ttu-id="d0808-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0808-117">Application</span></span>|<span data-ttu-id="d0808-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0808-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0808-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0808-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="d0808-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0808-120">Request headers</span></span>
|<span data-ttu-id="d0808-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0808-121">Header</span></span>|<span data-ttu-id="d0808-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d0808-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0808-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0808-123">Authorization</span></span>|<span data-ttu-id="d0808-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0808-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0808-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d0808-125">Accept</span></span>|<span data-ttu-id="d0808-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d0808-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0808-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0808-127">Request body</span></span>
<span data-ttu-id="d0808-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="d0808-128">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="d0808-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="d0808-129">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="d0808-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0808-130">Property</span></span>|<span data-ttu-id="d0808-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0808-131">Type</span></span>|<span data-ttu-id="d0808-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0808-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0808-133">id</span><span class="sxs-lookup"><span data-stu-id="d0808-133">id</span></span>|<span data-ttu-id="d0808-134">String</span><span class="sxs-lookup"><span data-stu-id="d0808-134">String</span></span>|<span data-ttu-id="d0808-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d0808-135">Key of the entity.</span></span>|
|<span data-ttu-id="d0808-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="d0808-136">pendingCount</span></span>|<span data-ttu-id="d0808-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d0808-137">Int32</span></span>|<span data-ttu-id="d0808-138">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="d0808-138">Number of pending devices</span></span>|
|<span data-ttu-id="d0808-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d0808-139">notApplicableCount</span></span>|<span data-ttu-id="d0808-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d0808-140">Int32</span></span>|<span data-ttu-id="d0808-141">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="d0808-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="d0808-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="d0808-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="d0808-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d0808-143">Int32</span></span>|<span data-ttu-id="d0808-144">Número de dispositivos não aplicáveis devido à plataforma e à política incompatíveis</span><span class="sxs-lookup"><span data-stu-id="d0808-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="d0808-145">successCount</span><span class="sxs-lookup"><span data-stu-id="d0808-145">successCount</span></span>|<span data-ttu-id="d0808-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d0808-146">Int32</span></span>|<span data-ttu-id="d0808-147">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="d0808-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="d0808-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="d0808-148">errorCount</span></span>|<span data-ttu-id="d0808-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d0808-149">Int32</span></span>|<span data-ttu-id="d0808-150">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="d0808-150">Number of error devices</span></span>|
|<span data-ttu-id="d0808-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="d0808-151">failedCount</span></span>|<span data-ttu-id="d0808-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d0808-152">Int32</span></span>|<span data-ttu-id="d0808-153">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="d0808-153">Number of failed devices</span></span>|
|<span data-ttu-id="d0808-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="d0808-154">conflictCount</span></span>|<span data-ttu-id="d0808-155">Int32</span><span class="sxs-lookup"><span data-stu-id="d0808-155">Int32</span></span>|<span data-ttu-id="d0808-156">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="d0808-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="d0808-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="d0808-157">lastUpdateDateTime</span></span>|<span data-ttu-id="d0808-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0808-158">DateTimeOffset</span></span>|<span data-ttu-id="d0808-159">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="d0808-159">Last update time</span></span>|
|<span data-ttu-id="d0808-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="d0808-160">configurationVersion</span></span>|<span data-ttu-id="d0808-161">Int32</span><span class="sxs-lookup"><span data-stu-id="d0808-161">Int32</span></span>|<span data-ttu-id="d0808-162">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="d0808-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="d0808-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0808-163">Response</span></span>
<span data-ttu-id="d0808-164">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0808-164">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0808-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0808-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0808-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0808-166">Request</span></span>
<span data-ttu-id="d0808-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0808-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="d0808-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0808-168">Response</span></span>
<span data-ttu-id="d0808-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0808-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "886f167b-167b-886f-7b16-6f887b166f88",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```





