---
title: Atualizar deviceCompliancePolicyDeviceStateSummary
description: Atualizar as propriedades de um objeto deviceCompliancePolicyDeviceStateSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5da4941a6f37f67e320aca647332cadfdffaa483
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42755683"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="628be-103">Atualizar deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="628be-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="628be-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="628be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="628be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="628be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="628be-106">Atualizar as propriedades de um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="628be-106">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="628be-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="628be-107">Prerequisites</span></span>
<span data-ttu-id="628be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="628be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="628be-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="628be-110">Permission type</span></span>|<span data-ttu-id="628be-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="628be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="628be-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="628be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="628be-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="628be-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="628be-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="628be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="628be-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="628be-115">Not supported.</span></span>|
|<span data-ttu-id="628be-116">Application</span><span class="sxs-lookup"><span data-stu-id="628be-116">Application</span></span>|<span data-ttu-id="628be-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="628be-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="628be-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="628be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="628be-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="628be-119">Request headers</span></span>
|<span data-ttu-id="628be-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="628be-120">Header</span></span>|<span data-ttu-id="628be-121">Valor</span><span class="sxs-lookup"><span data-stu-id="628be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="628be-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="628be-122">Authorization</span></span>|<span data-ttu-id="628be-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="628be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="628be-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="628be-124">Accept</span></span>|<span data-ttu-id="628be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="628be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="628be-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="628be-126">Request body</span></span>
<span data-ttu-id="628be-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="628be-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="628be-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="628be-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="628be-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="628be-129">Property</span></span>|<span data-ttu-id="628be-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="628be-130">Type</span></span>|<span data-ttu-id="628be-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="628be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="628be-132">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="628be-132">inGracePeriodCount</span></span>|<span data-ttu-id="628be-133">Int32</span><span class="sxs-lookup"><span data-stu-id="628be-133">Int32</span></span>|<span data-ttu-id="628be-134">Quantidade de dispositivos que estão no período de cortesia</span><span class="sxs-lookup"><span data-stu-id="628be-134">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="628be-135">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="628be-135">configManagerCount</span></span>|<span data-ttu-id="628be-136">Int32</span><span class="sxs-lookup"><span data-stu-id="628be-136">Int32</span></span>|<span data-ttu-id="628be-137">Quantidade de dispositivos que estão em conformidade gerenciada pelo System Center Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="628be-137">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="628be-138">id</span><span class="sxs-lookup"><span data-stu-id="628be-138">id</span></span>|<span data-ttu-id="628be-139">String</span><span class="sxs-lookup"><span data-stu-id="628be-139">String</span></span>|<span data-ttu-id="628be-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="628be-140">Key of the entity.</span></span>|
|<span data-ttu-id="628be-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="628be-141">unknownDeviceCount</span></span>|<span data-ttu-id="628be-142">Int32</span><span class="sxs-lookup"><span data-stu-id="628be-142">Int32</span></span>|<span data-ttu-id="628be-143">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="628be-143">Number of unknown devices</span></span>|
|<span data-ttu-id="628be-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="628be-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="628be-145">Int32</span><span class="sxs-lookup"><span data-stu-id="628be-145">Int32</span></span>|<span data-ttu-id="628be-146">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="628be-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="628be-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="628be-147">compliantDeviceCount</span></span>|<span data-ttu-id="628be-148">Int32</span><span class="sxs-lookup"><span data-stu-id="628be-148">Int32</span></span>|<span data-ttu-id="628be-149">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="628be-149">Number of compliant devices</span></span>|
|<span data-ttu-id="628be-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="628be-150">remediatedDeviceCount</span></span>|<span data-ttu-id="628be-151">Int32</span><span class="sxs-lookup"><span data-stu-id="628be-151">Int32</span></span>|<span data-ttu-id="628be-152">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="628be-152">Number of remediated devices</span></span>|
|<span data-ttu-id="628be-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="628be-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="628be-154">Int32</span><span class="sxs-lookup"><span data-stu-id="628be-154">Int32</span></span>|<span data-ttu-id="628be-155">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="628be-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="628be-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="628be-156">errorDeviceCount</span></span>|<span data-ttu-id="628be-157">Int32</span><span class="sxs-lookup"><span data-stu-id="628be-157">Int32</span></span>|<span data-ttu-id="628be-158">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="628be-158">Number of error devices</span></span>|
|<span data-ttu-id="628be-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="628be-159">conflictDeviceCount</span></span>|<span data-ttu-id="628be-160">Int32</span><span class="sxs-lookup"><span data-stu-id="628be-160">Int32</span></span>|<span data-ttu-id="628be-161">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="628be-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="628be-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="628be-162">Response</span></span>
<span data-ttu-id="628be-163">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="628be-163">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="628be-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="628be-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="628be-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="628be-165">Request</span></span>
<span data-ttu-id="628be-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="628be-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="628be-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="628be-167">Response</span></span>
<span data-ttu-id="628be-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="628be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




