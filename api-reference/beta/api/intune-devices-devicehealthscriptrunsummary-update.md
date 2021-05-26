---
title: Atualizar deviceHealthScriptRunSummary
description: Atualize as propriedades de um objeto deviceHealthScriptRunSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d342f4703ba8dcb04b58007d26fc94ff99c8c91
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665088"
---
# <a name="update-devicehealthscriptrunsummary"></a><span data-ttu-id="83d37-103">Atualizar deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="83d37-103">Update deviceHealthScriptRunSummary</span></span>

<span data-ttu-id="83d37-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83d37-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83d37-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83d37-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83d37-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83d37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83d37-107">Atualize as propriedades de [um objeto deviceHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)</span><span class="sxs-lookup"><span data-stu-id="83d37-107">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83d37-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="83d37-108">Prerequisites</span></span>
<span data-ttu-id="83d37-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83d37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83d37-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83d37-111">Permission type</span></span>|<span data-ttu-id="83d37-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83d37-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83d37-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83d37-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83d37-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83d37-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83d37-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83d37-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83d37-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83d37-116">Not supported.</span></span>|
|<span data-ttu-id="83d37-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83d37-117">Application</span></span>|<span data-ttu-id="83d37-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83d37-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83d37-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83d37-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="83d37-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83d37-120">Request headers</span></span>
|<span data-ttu-id="83d37-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="83d37-121">Header</span></span>|<span data-ttu-id="83d37-122">Valor</span><span class="sxs-lookup"><span data-stu-id="83d37-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83d37-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="83d37-123">Authorization</span></span>|<span data-ttu-id="83d37-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83d37-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83d37-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="83d37-125">Accept</span></span>|<span data-ttu-id="83d37-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83d37-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83d37-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83d37-127">Request body</span></span>
<span data-ttu-id="83d37-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)</span><span class="sxs-lookup"><span data-stu-id="83d37-128">In the request body, supply a JSON representation for the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

<span data-ttu-id="83d37-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="83d37-129">The following table shows the properties that are required when you create the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md).</span></span>

|<span data-ttu-id="83d37-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83d37-130">Property</span></span>|<span data-ttu-id="83d37-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="83d37-131">Type</span></span>|<span data-ttu-id="83d37-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="83d37-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83d37-133">id</span><span class="sxs-lookup"><span data-stu-id="83d37-133">id</span></span>|<span data-ttu-id="83d37-134">String</span><span class="sxs-lookup"><span data-stu-id="83d37-134">String</span></span>|<span data-ttu-id="83d37-135">Chave da entidade resumo do script de saúde do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83d37-135">Key of the device health script run summary entity.</span></span> <span data-ttu-id="83d37-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="83d37-136">This property is read-only.</span></span>|
|<span data-ttu-id="83d37-137">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="83d37-137">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="83d37-138">Int32</span><span class="sxs-lookup"><span data-stu-id="83d37-138">Int32</span></span>|<span data-ttu-id="83d37-139">Número de dispositivos para os quais o script de detecção não encontrou um problema e o dispositivo está saudável</span><span class="sxs-lookup"><span data-stu-id="83d37-139">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="83d37-140">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="83d37-140">issueDetectedDeviceCount</span></span>|<span data-ttu-id="83d37-141">Int32</span><span class="sxs-lookup"><span data-stu-id="83d37-141">Int32</span></span>|<span data-ttu-id="83d37-142">Número de dispositivos para os quais o script de detecção encontrou um problema</span><span class="sxs-lookup"><span data-stu-id="83d37-142">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="83d37-143">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="83d37-143">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="83d37-144">Int32</span><span class="sxs-lookup"><span data-stu-id="83d37-144">Int32</span></span>|<span data-ttu-id="83d37-145">Número de dispositivos nos quais a execução do script de detecção encontrou um erro e não foi concluída</span><span class="sxs-lookup"><span data-stu-id="83d37-145">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="83d37-146">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="83d37-146">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="83d37-147">Int32</span><span class="sxs-lookup"><span data-stu-id="83d37-147">Int32</span></span>|<span data-ttu-id="83d37-148">Número de dispositivos que ainda não executaram a versão mais recente do script de saúde do dispositivo</span><span class="sxs-lookup"><span data-stu-id="83d37-148">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="83d37-149">detectionScriptNotApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="83d37-149">detectionScriptNotApplicableDeviceCount</span></span>|<span data-ttu-id="83d37-150">Int32</span><span class="sxs-lookup"><span data-stu-id="83d37-150">Int32</span></span>|<span data-ttu-id="83d37-151">Número de dispositivos para os quais o script de detecção não foi aplicável</span><span class="sxs-lookup"><span data-stu-id="83d37-151">Number of devices for which the detection script was not applicable</span></span>|
|<span data-ttu-id="83d37-152">issueRemediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="83d37-152">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="83d37-153">Int32</span><span class="sxs-lookup"><span data-stu-id="83d37-153">Int32</span></span>|<span data-ttu-id="83d37-154">Número de dispositivos para os quais o script de correção foi capaz de resolver o problema detectado</span><span class="sxs-lookup"><span data-stu-id="83d37-154">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="83d37-155">remediationSkippedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="83d37-155">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="83d37-156">Int32</span><span class="sxs-lookup"><span data-stu-id="83d37-156">Int32</span></span>|<span data-ttu-id="83d37-157">Número de dispositivos para os quais a correção foi ignorada</span><span class="sxs-lookup"><span data-stu-id="83d37-157">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="83d37-158">issueReoccurredDeviceCount</span><span class="sxs-lookup"><span data-stu-id="83d37-158">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="83d37-159">Int32</span><span class="sxs-lookup"><span data-stu-id="83d37-159">Int32</span></span>|<span data-ttu-id="83d37-160">Número de dispositivos para os quais o script de correção foi executado com êxito, mas não conseguiu resolver o problema detectado</span><span class="sxs-lookup"><span data-stu-id="83d37-160">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="83d37-161">remediationScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="83d37-161">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="83d37-162">Int32</span><span class="sxs-lookup"><span data-stu-id="83d37-162">Int32</span></span>|<span data-ttu-id="83d37-163">Número de dispositivos para os quais a execução do script de correção encontrou um erro e não foi concluída</span><span class="sxs-lookup"><span data-stu-id="83d37-163">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="83d37-164">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="83d37-164">lastScriptRunDateTime</span></span>|<span data-ttu-id="83d37-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83d37-165">DateTimeOffset</span></span>|<span data-ttu-id="83d37-166">Tempo de última duração do script em todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="83d37-166">Last run time for the script across all devices</span></span>|
|<span data-ttu-id="83d37-167">issueRemediatedCumulativeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="83d37-167">issueRemediatedCumulativeDeviceCount</span></span>|<span data-ttu-id="83d37-168">Int32</span><span class="sxs-lookup"><span data-stu-id="83d37-168">Int32</span></span>|<span data-ttu-id="83d37-169">Número de dispositivos que foram remediados nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="83d37-169">Number of devices that were remediated over the last 30 days</span></span>|



## <a name="response"></a><span data-ttu-id="83d37-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="83d37-170">Response</span></span>
<span data-ttu-id="83d37-171">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83d37-171">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83d37-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83d37-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="83d37-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83d37-173">Request</span></span>
<span data-ttu-id="83d37-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83d37-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
Content-type: application/json
Content-length: 543

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "detectionScriptNotApplicableDeviceCount": 7,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
  "issueRemediatedCumulativeDeviceCount": 4
}
```

### <a name="response"></a><span data-ttu-id="83d37-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="83d37-175">Response</span></span>
<span data-ttu-id="83d37-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83d37-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 592

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "8221b043-b043-8221-43b0-218243b02182",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "detectionScriptNotApplicableDeviceCount": 7,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
  "issueRemediatedCumulativeDeviceCount": 4
}
```




