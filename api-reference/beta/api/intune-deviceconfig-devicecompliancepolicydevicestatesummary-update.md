---
title: Atualizar deviceCompliancePolicyDeviceStateSummary
description: Atualizar as propriedades de um objeto deviceCompliancePolicyDeviceStateSummary.
ms.openlocfilehash: 045c9ac7aaecac535f3c4d04f587c74cbe84f442
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036799"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="c904b-103">Atualizar deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c904b-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="c904b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c904b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c904b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c904b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c904b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c904b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c904b-107">Atualizar as propriedades de um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c904b-107">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c904b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c904b-108">Prerequisites</span></span>
<span data-ttu-id="c904b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c904b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c904b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c904b-111">Permission type</span></span>|<span data-ttu-id="c904b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c904b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c904b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c904b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c904b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c904b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c904b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c904b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c904b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c904b-116">Not supported.</span></span>|
|<span data-ttu-id="c904b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c904b-117">Application</span></span>|<span data-ttu-id="c904b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c904b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c904b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c904b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="c904b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c904b-120">Request headers</span></span>
|<span data-ttu-id="c904b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c904b-121">Header</span></span>|<span data-ttu-id="c904b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c904b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c904b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c904b-123">Authorization</span></span>|<span data-ttu-id="c904b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c904b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c904b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c904b-125">Accept</span></span>|<span data-ttu-id="c904b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c904b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c904b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c904b-127">Request body</span></span>
<span data-ttu-id="c904b-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c904b-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="c904b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c904b-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="c904b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c904b-130">Property</span></span>|<span data-ttu-id="c904b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c904b-131">Type</span></span>|<span data-ttu-id="c904b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c904b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c904b-133">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="c904b-133">inGracePeriodCount</span></span>|<span data-ttu-id="c904b-134">Int32</span><span class="sxs-lookup"><span data-stu-id="c904b-134">Int32</span></span>|<span data-ttu-id="c904b-135">Quantidade de dispositivos que estão no período de cortesia</span><span class="sxs-lookup"><span data-stu-id="c904b-135">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="c904b-136">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="c904b-136">configManagerCount</span></span>|<span data-ttu-id="c904b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c904b-137">Int32</span></span>|<span data-ttu-id="c904b-138">Quantidade de dispositivos que estão em conformidade gerenciada pelo System Center Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="c904b-138">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="c904b-139">id</span><span class="sxs-lookup"><span data-stu-id="c904b-139">id</span></span>|<span data-ttu-id="c904b-140">String</span><span class="sxs-lookup"><span data-stu-id="c904b-140">String</span></span>|<span data-ttu-id="c904b-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c904b-141">Key of the entity.</span></span>|
|<span data-ttu-id="c904b-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c904b-142">unknownDeviceCount</span></span>|<span data-ttu-id="c904b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c904b-143">Int32</span></span>|<span data-ttu-id="c904b-144">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="c904b-144">Number of unknown devices</span></span>|
|<span data-ttu-id="c904b-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c904b-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="c904b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="c904b-146">Int32</span></span>|<span data-ttu-id="c904b-147">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="c904b-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="c904b-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c904b-148">compliantDeviceCount</span></span>|<span data-ttu-id="c904b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c904b-149">Int32</span></span>|<span data-ttu-id="c904b-150">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="c904b-150">Number of compliant devices</span></span>|
|<span data-ttu-id="c904b-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c904b-151">remediatedDeviceCount</span></span>|<span data-ttu-id="c904b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c904b-152">Int32</span></span>|<span data-ttu-id="c904b-153">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="c904b-153">Number of remediated devices</span></span>|
|<span data-ttu-id="c904b-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c904b-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="c904b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="c904b-155">Int32</span></span>|<span data-ttu-id="c904b-156">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="c904b-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="c904b-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c904b-157">errorDeviceCount</span></span>|<span data-ttu-id="c904b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c904b-158">Int32</span></span>|<span data-ttu-id="c904b-159">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="c904b-159">Number of error devices</span></span>|
|<span data-ttu-id="c904b-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c904b-160">conflictDeviceCount</span></span>|<span data-ttu-id="c904b-161">Int32</span><span class="sxs-lookup"><span data-stu-id="c904b-161">Int32</span></span>|<span data-ttu-id="c904b-162">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="c904b-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="c904b-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="c904b-163">Response</span></span>
<span data-ttu-id="c904b-164">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c904b-164">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c904b-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c904b-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="c904b-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c904b-166">Request</span></span>
<span data-ttu-id="c904b-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c904b-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicyDeviceStateSummary
Content-type: application/json
Content-length: 270

{
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

### <a name="response"></a><span data-ttu-id="c904b-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="c904b-168">Response</span></span>
<span data-ttu-id="c904b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c904b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





