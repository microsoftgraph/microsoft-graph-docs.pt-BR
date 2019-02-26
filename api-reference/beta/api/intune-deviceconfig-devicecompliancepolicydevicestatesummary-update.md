---
title: Atualizar deviceCompliancePolicyDeviceStateSummary
description: Atualizar as propriedades de um objeto deviceCompliancePolicyDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9bc839c96ca07f5b49dff6107058b7ca84c788e0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171971"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="e7acb-103">Atualizar deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e7acb-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="e7acb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e7acb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7acb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7acb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7acb-106">Atualizar as propriedades de um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e7acb-106">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7acb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7acb-107">Prerequisites</span></span>
<span data-ttu-id="e7acb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e7acb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e7acb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7acb-110">Permission type</span></span>|<span data-ttu-id="e7acb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7acb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7acb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7acb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7acb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7acb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7acb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7acb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7acb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7acb-115">Not supported.</span></span>|
|<span data-ttu-id="e7acb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7acb-116">Application</span></span>|<span data-ttu-id="e7acb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7acb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7acb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7acb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="e7acb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7acb-119">Request headers</span></span>
|<span data-ttu-id="e7acb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7acb-120">Header</span></span>|<span data-ttu-id="e7acb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e7acb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7acb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7acb-122">Authorization</span></span>|<span data-ttu-id="e7acb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7acb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7acb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7acb-124">Accept</span></span>|<span data-ttu-id="e7acb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7acb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7acb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7acb-126">Request body</span></span>
<span data-ttu-id="e7acb-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e7acb-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="e7acb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e7acb-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="e7acb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7acb-129">Property</span></span>|<span data-ttu-id="e7acb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7acb-130">Type</span></span>|<span data-ttu-id="e7acb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7acb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7acb-132">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="e7acb-132">inGracePeriodCount</span></span>|<span data-ttu-id="e7acb-133">Int32</span><span class="sxs-lookup"><span data-stu-id="e7acb-133">Int32</span></span>|<span data-ttu-id="e7acb-134">Quantidade de dispositivos que estão no período de cortesia</span><span class="sxs-lookup"><span data-stu-id="e7acb-134">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="e7acb-135">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="e7acb-135">configManagerCount</span></span>|<span data-ttu-id="e7acb-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e7acb-136">Int32</span></span>|<span data-ttu-id="e7acb-137">Quantidade de dispositivos que estão em conformidade gerenciada pelo System Center Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="e7acb-137">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="e7acb-138">id</span><span class="sxs-lookup"><span data-stu-id="e7acb-138">id</span></span>|<span data-ttu-id="e7acb-139">String</span><span class="sxs-lookup"><span data-stu-id="e7acb-139">String</span></span>|<span data-ttu-id="e7acb-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e7acb-140">Key of the entity.</span></span>|
|<span data-ttu-id="e7acb-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e7acb-141">unknownDeviceCount</span></span>|<span data-ttu-id="e7acb-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e7acb-142">Int32</span></span>|<span data-ttu-id="e7acb-143">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="e7acb-143">Number of unknown devices</span></span>|
|<span data-ttu-id="e7acb-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e7acb-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="e7acb-145">Int32</span><span class="sxs-lookup"><span data-stu-id="e7acb-145">Int32</span></span>|<span data-ttu-id="e7acb-146">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="e7acb-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="e7acb-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e7acb-147">compliantDeviceCount</span></span>|<span data-ttu-id="e7acb-148">Int32</span><span class="sxs-lookup"><span data-stu-id="e7acb-148">Int32</span></span>|<span data-ttu-id="e7acb-149">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="e7acb-149">Number of compliant devices</span></span>|
|<span data-ttu-id="e7acb-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e7acb-150">remediatedDeviceCount</span></span>|<span data-ttu-id="e7acb-151">Int32</span><span class="sxs-lookup"><span data-stu-id="e7acb-151">Int32</span></span>|<span data-ttu-id="e7acb-152">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="e7acb-152">Number of remediated devices</span></span>|
|<span data-ttu-id="e7acb-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e7acb-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e7acb-154">Int32</span><span class="sxs-lookup"><span data-stu-id="e7acb-154">Int32</span></span>|<span data-ttu-id="e7acb-155">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="e7acb-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="e7acb-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e7acb-156">errorDeviceCount</span></span>|<span data-ttu-id="e7acb-157">Int32</span><span class="sxs-lookup"><span data-stu-id="e7acb-157">Int32</span></span>|<span data-ttu-id="e7acb-158">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="e7acb-158">Number of error devices</span></span>|
|<span data-ttu-id="e7acb-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e7acb-159">conflictDeviceCount</span></span>|<span data-ttu-id="e7acb-160">Int32</span><span class="sxs-lookup"><span data-stu-id="e7acb-160">Int32</span></span>|<span data-ttu-id="e7acb-161">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="e7acb-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="e7acb-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7acb-162">Response</span></span>
<span data-ttu-id="e7acb-163">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7acb-163">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7acb-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7acb-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7acb-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7acb-165">Request</span></span>
<span data-ttu-id="e7acb-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7acb-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicyDeviceStateSummary
Content-type: application/json
Content-length: 349

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="e7acb-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7acb-167">Response</span></span>
<span data-ttu-id="e7acb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7acb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```




