---
title: Atualizar deviceComplianceDeviceOverview
description: Atualizar as propriedades de um objeto deviceComplianceDeviceOverview.
ms.openlocfilehash: ef95ab3b197c228ac2e7a94857ae166c44eaf003
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033916"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="57be8-103">Atualizar deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="57be8-103">Update deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="57be8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="57be8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57be8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="57be8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57be8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="57be8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57be8-107">Atualizar as propriedades de um objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="57be8-107">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="57be8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57be8-108">Prerequisites</span></span>
<span data-ttu-id="57be8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57be8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57be8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57be8-111">Permission type</span></span>|<span data-ttu-id="57be8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57be8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57be8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57be8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57be8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57be8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57be8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57be8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57be8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57be8-116">Not supported.</span></span>|
|<span data-ttu-id="57be8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57be8-117">Application</span></span>|<span data-ttu-id="57be8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57be8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57be8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57be8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="57be8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57be8-120">Request headers</span></span>
|<span data-ttu-id="57be8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57be8-121">Header</span></span>|<span data-ttu-id="57be8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="57be8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57be8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="57be8-123">Authorization</span></span>|<span data-ttu-id="57be8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57be8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57be8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="57be8-125">Accept</span></span>|<span data-ttu-id="57be8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57be8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57be8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57be8-127">Request body</span></span>
<span data-ttu-id="57be8-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="57be8-128">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="57be8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="57be8-129">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="57be8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57be8-130">Property</span></span>|<span data-ttu-id="57be8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="57be8-131">Type</span></span>|<span data-ttu-id="57be8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="57be8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57be8-133">id</span><span class="sxs-lookup"><span data-stu-id="57be8-133">id</span></span>|<span data-ttu-id="57be8-134">String</span><span class="sxs-lookup"><span data-stu-id="57be8-134">String</span></span>|<span data-ttu-id="57be8-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="57be8-135">Key of the entity.</span></span>|
|<span data-ttu-id="57be8-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="57be8-136">pendingCount</span></span>|<span data-ttu-id="57be8-137">Int32</span><span class="sxs-lookup"><span data-stu-id="57be8-137">Int32</span></span>|<span data-ttu-id="57be8-138">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="57be8-138">Number of pending devices</span></span>|
|<span data-ttu-id="57be8-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="57be8-139">notApplicableCount</span></span>|<span data-ttu-id="57be8-140">Int32</span><span class="sxs-lookup"><span data-stu-id="57be8-140">Int32</span></span>|<span data-ttu-id="57be8-141">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="57be8-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="57be8-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="57be8-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="57be8-143">Int32</span><span class="sxs-lookup"><span data-stu-id="57be8-143">Int32</span></span>|<span data-ttu-id="57be8-144">Número de dispositivos não aplicáveis devido à plataforma de incompatibilidade e política</span><span class="sxs-lookup"><span data-stu-id="57be8-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="57be8-145">successCount</span><span class="sxs-lookup"><span data-stu-id="57be8-145">successCount</span></span>|<span data-ttu-id="57be8-146">Int32</span><span class="sxs-lookup"><span data-stu-id="57be8-146">Int32</span></span>|<span data-ttu-id="57be8-147">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="57be8-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="57be8-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="57be8-148">errorCount</span></span>|<span data-ttu-id="57be8-149">Int32</span><span class="sxs-lookup"><span data-stu-id="57be8-149">Int32</span></span>|<span data-ttu-id="57be8-150">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="57be8-150">Number of error devices</span></span>|
|<span data-ttu-id="57be8-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="57be8-151">failedCount</span></span>|<span data-ttu-id="57be8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="57be8-152">Int32</span></span>|<span data-ttu-id="57be8-153">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="57be8-153">Number of failed devices</span></span>|
|<span data-ttu-id="57be8-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="57be8-154">conflictCount</span></span>|<span data-ttu-id="57be8-155">Int32</span><span class="sxs-lookup"><span data-stu-id="57be8-155">Int32</span></span>|<span data-ttu-id="57be8-156">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="57be8-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="57be8-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="57be8-157">lastUpdateDateTime</span></span>|<span data-ttu-id="57be8-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57be8-158">DateTimeOffset</span></span>|<span data-ttu-id="57be8-159">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="57be8-159">Last update time</span></span>|
|<span data-ttu-id="57be8-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="57be8-160">configurationVersion</span></span>|<span data-ttu-id="57be8-161">Int32</span><span class="sxs-lookup"><span data-stu-id="57be8-161">Int32</span></span>|<span data-ttu-id="57be8-162">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="57be8-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="57be8-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="57be8-163">Response</span></span>
<span data-ttu-id="57be8-164">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57be8-164">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57be8-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57be8-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="57be8-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57be8-166">Request</span></span>
<span data-ttu-id="57be8-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57be8-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
Content-type: application/json
Content-length: 273

{
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

### <a name="response"></a><span data-ttu-id="57be8-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="57be8-168">Response</span></span>
<span data-ttu-id="57be8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57be8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





