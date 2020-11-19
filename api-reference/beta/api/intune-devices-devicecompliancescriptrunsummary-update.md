---
title: Atualizar deviceComplianceScriptRunSummary
description: Atualiza as propriedades de um objeto deviceComplianceScriptRunSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b9f723b924028a73facdee32073508f1743511a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49310864"
---
# <a name="update-devicecompliancescriptrunsummary"></a><span data-ttu-id="40cc6-103">Atualizar deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="40cc6-103">Update deviceComplianceScriptRunSummary</span></span>

<span data-ttu-id="40cc6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40cc6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40cc6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="40cc6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40cc6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40cc6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40cc6-107">Atualiza as propriedades de um objeto [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="40cc6-107">Update the properties of a [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40cc6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="40cc6-108">Prerequisites</span></span>
<span data-ttu-id="40cc6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40cc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40cc6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40cc6-111">Permission type</span></span>|<span data-ttu-id="40cc6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="40cc6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40cc6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40cc6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40cc6-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40cc6-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="40cc6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40cc6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40cc6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40cc6-116">Not supported.</span></span>|
|<span data-ttu-id="40cc6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40cc6-117">Application</span></span>|<span data-ttu-id="40cc6-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40cc6-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40cc6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40cc6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="40cc6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40cc6-120">Request headers</span></span>
|<span data-ttu-id="40cc6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40cc6-121">Header</span></span>|<span data-ttu-id="40cc6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="40cc6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40cc6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="40cc6-123">Authorization</span></span>|<span data-ttu-id="40cc6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40cc6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40cc6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="40cc6-125">Accept</span></span>|<span data-ttu-id="40cc6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40cc6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40cc6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40cc6-127">Request body</span></span>
<span data-ttu-id="40cc6-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="40cc6-128">In the request body, supply a JSON representation for the [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>

<span data-ttu-id="40cc6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="40cc6-129">The following table shows the properties that are required when you create the [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md).</span></span>

|<span data-ttu-id="40cc6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40cc6-130">Property</span></span>|<span data-ttu-id="40cc6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="40cc6-131">Type</span></span>|<span data-ttu-id="40cc6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="40cc6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40cc6-133">id</span><span class="sxs-lookup"><span data-stu-id="40cc6-133">id</span></span>|<span data-ttu-id="40cc6-134">String</span><span class="sxs-lookup"><span data-stu-id="40cc6-134">String</span></span>|<span data-ttu-id="40cc6-135">Chave da entidade de Resumo de execução de script de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40cc6-135">Key of the device compliance script run summary entity.</span></span> <span data-ttu-id="40cc6-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40cc6-136">This property is read-only.</span></span>|
|<span data-ttu-id="40cc6-137">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="40cc6-137">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="40cc6-138">Int32</span><span class="sxs-lookup"><span data-stu-id="40cc6-138">Int32</span></span>|<span data-ttu-id="40cc6-139">Número de dispositivos para os quais o script de detecção não encontrou um problema e o dispositivo está íntegro.</span><span class="sxs-lookup"><span data-stu-id="40cc6-139">Number of devices for which the detection script did not find an issue and the device is healthy.</span></span> <span data-ttu-id="40cc6-140">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="40cc6-140">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="40cc6-141">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="40cc6-141">issueDetectedDeviceCount</span></span>|<span data-ttu-id="40cc6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="40cc6-142">Int32</span></span>|<span data-ttu-id="40cc6-143">Número de dispositivos para os quais o script de detecção encontrou um problema.</span><span class="sxs-lookup"><span data-stu-id="40cc6-143">Number of devices for which the detection script found an issue.</span></span> <span data-ttu-id="40cc6-144">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="40cc6-144">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="40cc6-145">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="40cc6-145">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="40cc6-146">Int32</span><span class="sxs-lookup"><span data-stu-id="40cc6-146">Int32</span></span>|<span data-ttu-id="40cc6-147">Número de dispositivos nos quais a execução do script de detecção encontrou um erro e não foi concluída.</span><span class="sxs-lookup"><span data-stu-id="40cc6-147">Number of devices on which the detection script execution encountered an error and did not complete.</span></span> <span data-ttu-id="40cc6-148">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="40cc6-148">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="40cc6-149">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="40cc6-149">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="40cc6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="40cc6-150">Int32</span></span>|<span data-ttu-id="40cc6-151">Número de dispositivos que ainda não executaram a versão mais recente do script de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40cc6-151">Number of devices which have not yet run the latest version of the device compliance script.</span></span> <span data-ttu-id="40cc6-152">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="40cc6-152">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="40cc6-153">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="40cc6-153">lastScriptRunDateTime</span></span>|<span data-ttu-id="40cc6-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40cc6-154">DateTimeOffset</span></span>|<span data-ttu-id="40cc6-155">Hora da última execução para o script em todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="40cc6-155">Last run time for the script across all devices</span></span>|



## <a name="response"></a><span data-ttu-id="40cc6-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="40cc6-156">Response</span></span>
<span data-ttu-id="40cc6-157">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40cc6-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40cc6-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40cc6-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="40cc6-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40cc6-159">Request</span></span>
<span data-ttu-id="40cc6-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40cc6-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/runSummary
Content-type: application/json
Content-length: 295

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00"
}
```

### <a name="response"></a><span data-ttu-id="40cc6-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="40cc6-161">Response</span></span>
<span data-ttu-id="40cc6-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40cc6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "id": "dad42f14-2f14-dad4-142f-d4da142fd4da",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00"
}
```




