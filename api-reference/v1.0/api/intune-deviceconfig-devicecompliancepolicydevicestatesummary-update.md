---
title: Atualizar deviceCompliancePolicyDeviceStateSummary
description: Atualizar as propriedades de um objeto deviceCompliancePolicyDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 35f55096ed9307bc4a4c29cf98418b8f36b45cbd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807431"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="a6d79-103">Atualizar deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="a6d79-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="a6d79-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a6d79-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6d79-105">Atualizar as propriedades de um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a6d79-105">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a6d79-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6d79-106">Prerequisites</span></span>
<span data-ttu-id="a6d79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6d79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6d79-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6d79-109">Permission type</span></span>|<span data-ttu-id="a6d79-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a6d79-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6d79-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6d79-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a6d79-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6d79-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6d79-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6d79-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6d79-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6d79-114">Not supported.</span></span>|
|<span data-ttu-id="a6d79-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6d79-115">Application</span></span>|<span data-ttu-id="a6d79-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6d79-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6d79-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6d79-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="a6d79-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6d79-118">Request headers</span></span>
|<span data-ttu-id="a6d79-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6d79-119">Header</span></span>|<span data-ttu-id="a6d79-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a6d79-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6d79-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6d79-121">Authorization</span></span>|<span data-ttu-id="a6d79-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6d79-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6d79-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6d79-123">Accept</span></span>|<span data-ttu-id="a6d79-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a6d79-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6d79-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6d79-125">Request body</span></span>
<span data-ttu-id="a6d79-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a6d79-126">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="a6d79-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a6d79-127">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="a6d79-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6d79-128">Property</span></span>|<span data-ttu-id="a6d79-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6d79-129">Type</span></span>|<span data-ttu-id="a6d79-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6d79-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6d79-131">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="a6d79-131">inGracePeriodCount</span></span>|<span data-ttu-id="a6d79-132">Int32</span><span class="sxs-lookup"><span data-stu-id="a6d79-132">Int32</span></span>|<span data-ttu-id="a6d79-133">Quantidade de dispositivos que estão no período de cortesia</span><span class="sxs-lookup"><span data-stu-id="a6d79-133">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="a6d79-134">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="a6d79-134">configManagerCount</span></span>|<span data-ttu-id="a6d79-135">Int32</span><span class="sxs-lookup"><span data-stu-id="a6d79-135">Int32</span></span>|<span data-ttu-id="a6d79-136">Quantidade de dispositivos que estão em conformidade gerenciada pelo System Center Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="a6d79-136">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="a6d79-137">id</span><span class="sxs-lookup"><span data-stu-id="a6d79-137">id</span></span>|<span data-ttu-id="a6d79-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6d79-138">String</span></span>|<span data-ttu-id="a6d79-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a6d79-139">Key of the entity.</span></span>|
|<span data-ttu-id="a6d79-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a6d79-140">unknownDeviceCount</span></span>|<span data-ttu-id="a6d79-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a6d79-141">Int32</span></span>|<span data-ttu-id="a6d79-142">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="a6d79-142">Number of unknown devices</span></span>|
|<span data-ttu-id="a6d79-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a6d79-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="a6d79-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a6d79-144">Int32</span></span>|<span data-ttu-id="a6d79-145">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="a6d79-145">Number of not applicable devices</span></span>|
|<span data-ttu-id="a6d79-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a6d79-146">compliantDeviceCount</span></span>|<span data-ttu-id="a6d79-147">Int32</span><span class="sxs-lookup"><span data-stu-id="a6d79-147">Int32</span></span>|<span data-ttu-id="a6d79-148">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="a6d79-148">Number of compliant devices</span></span>|
|<span data-ttu-id="a6d79-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a6d79-149">remediatedDeviceCount</span></span>|<span data-ttu-id="a6d79-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a6d79-150">Int32</span></span>|<span data-ttu-id="a6d79-151">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="a6d79-151">Number of remediated devices</span></span>|
|<span data-ttu-id="a6d79-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a6d79-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a6d79-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a6d79-153">Int32</span></span>|<span data-ttu-id="a6d79-154">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="a6d79-154">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="a6d79-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a6d79-155">errorDeviceCount</span></span>|<span data-ttu-id="a6d79-156">Int32</span><span class="sxs-lookup"><span data-stu-id="a6d79-156">Int32</span></span>|<span data-ttu-id="a6d79-157">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="a6d79-157">Number of error devices</span></span>|
|<span data-ttu-id="a6d79-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a6d79-158">conflictDeviceCount</span></span>|<span data-ttu-id="a6d79-159">Int32</span><span class="sxs-lookup"><span data-stu-id="a6d79-159">Int32</span></span>|<span data-ttu-id="a6d79-160">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="a6d79-160">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="a6d79-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6d79-161">Response</span></span>
<span data-ttu-id="a6d79-162">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6d79-162">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6d79-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6d79-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="a6d79-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6d79-164">Request</span></span>
<span data-ttu-id="a6d79-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6d79-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicyDeviceStateSummary
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

### <a name="response"></a><span data-ttu-id="a6d79-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6d79-166">Response</span></span>
<span data-ttu-id="a6d79-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6d79-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



