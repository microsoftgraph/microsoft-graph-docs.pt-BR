---
title: Atualizar deviceCompliancePolicyDeviceStateSummary
description: Atualizar as propriedades de um objeto deviceCompliancePolicyDeviceStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2236e5bfb666e51294993d66267baf0a65905859
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082914"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="63874-103">Atualizar deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="63874-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

<span data-ttu-id="63874-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63874-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63874-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63874-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63874-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63874-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63874-107">Atualizar as propriedades de um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="63874-107">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63874-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63874-108">Prerequisites</span></span>
<span data-ttu-id="63874-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63874-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63874-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63874-111">Permission type</span></span>|<span data-ttu-id="63874-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63874-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63874-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63874-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63874-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63874-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="63874-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63874-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63874-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63874-116">Not supported.</span></span>|
|<span data-ttu-id="63874-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63874-117">Application</span></span>|<span data-ttu-id="63874-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63874-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63874-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63874-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="63874-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63874-120">Request headers</span></span>
|<span data-ttu-id="63874-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63874-121">Header</span></span>|<span data-ttu-id="63874-122">Valor</span><span class="sxs-lookup"><span data-stu-id="63874-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63874-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="63874-123">Authorization</span></span>|<span data-ttu-id="63874-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63874-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63874-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63874-125">Accept</span></span>|<span data-ttu-id="63874-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63874-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63874-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63874-127">Request body</span></span>
<span data-ttu-id="63874-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="63874-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="63874-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="63874-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="63874-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63874-130">Property</span></span>|<span data-ttu-id="63874-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="63874-131">Type</span></span>|<span data-ttu-id="63874-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="63874-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63874-133">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="63874-133">inGracePeriodCount</span></span>|<span data-ttu-id="63874-134">Int32</span><span class="sxs-lookup"><span data-stu-id="63874-134">Int32</span></span>|<span data-ttu-id="63874-135">Quantidade de dispositivos que estão no período de cortesia</span><span class="sxs-lookup"><span data-stu-id="63874-135">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="63874-136">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="63874-136">configManagerCount</span></span>|<span data-ttu-id="63874-137">Int32</span><span class="sxs-lookup"><span data-stu-id="63874-137">Int32</span></span>|<span data-ttu-id="63874-138">Quantidade de dispositivos que estão em conformidade gerenciada pelo System Center Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="63874-138">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="63874-139">id</span><span class="sxs-lookup"><span data-stu-id="63874-139">id</span></span>|<span data-ttu-id="63874-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63874-140">String</span></span>|<span data-ttu-id="63874-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="63874-141">Key of the entity.</span></span>|
|<span data-ttu-id="63874-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63874-142">unknownDeviceCount</span></span>|<span data-ttu-id="63874-143">Int32</span><span class="sxs-lookup"><span data-stu-id="63874-143">Int32</span></span>|<span data-ttu-id="63874-144">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="63874-144">Number of unknown devices</span></span>|
|<span data-ttu-id="63874-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63874-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="63874-146">Int32</span><span class="sxs-lookup"><span data-stu-id="63874-146">Int32</span></span>|<span data-ttu-id="63874-147">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="63874-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="63874-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63874-148">compliantDeviceCount</span></span>|<span data-ttu-id="63874-149">Int32</span><span class="sxs-lookup"><span data-stu-id="63874-149">Int32</span></span>|<span data-ttu-id="63874-150">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="63874-150">Number of compliant devices</span></span>|
|<span data-ttu-id="63874-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63874-151">remediatedDeviceCount</span></span>|<span data-ttu-id="63874-152">Int32</span><span class="sxs-lookup"><span data-stu-id="63874-152">Int32</span></span>|<span data-ttu-id="63874-153">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="63874-153">Number of remediated devices</span></span>|
|<span data-ttu-id="63874-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63874-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="63874-155">Int32</span><span class="sxs-lookup"><span data-stu-id="63874-155">Int32</span></span>|<span data-ttu-id="63874-156">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="63874-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="63874-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63874-157">errorDeviceCount</span></span>|<span data-ttu-id="63874-158">Int32</span><span class="sxs-lookup"><span data-stu-id="63874-158">Int32</span></span>|<span data-ttu-id="63874-159">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="63874-159">Number of error devices</span></span>|
|<span data-ttu-id="63874-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63874-160">conflictDeviceCount</span></span>|<span data-ttu-id="63874-161">Int32</span><span class="sxs-lookup"><span data-stu-id="63874-161">Int32</span></span>|<span data-ttu-id="63874-162">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="63874-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="63874-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="63874-163">Response</span></span>
<span data-ttu-id="63874-164">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63874-164">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63874-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63874-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="63874-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63874-166">Request</span></span>
<span data-ttu-id="63874-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63874-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="63874-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="63874-168">Response</span></span>
<span data-ttu-id="63874-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63874-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






