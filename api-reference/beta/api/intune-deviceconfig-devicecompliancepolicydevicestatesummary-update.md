---
title: Atualizar deviceCompliancePolicyDeviceStateSummary
description: Atualizar as propriedades de um objeto deviceCompliancePolicyDeviceStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d4df79fcc8a532fa4fe026cffee0b21100c3963a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733067"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="4a375-103">Atualizar deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="4a375-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

<span data-ttu-id="4a375-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a375-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a375-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4a375-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a375-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a375-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a375-107">Atualizar as propriedades de um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="4a375-107">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a375-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4a375-108">Prerequisites</span></span>
<span data-ttu-id="4a375-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a375-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a375-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a375-111">Permission type</span></span>|<span data-ttu-id="4a375-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4a375-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a375-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a375-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a375-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a375-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a375-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a375-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a375-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a375-116">Not supported.</span></span>|
|<span data-ttu-id="4a375-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a375-117">Application</span></span>|<span data-ttu-id="4a375-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a375-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a375-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a375-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="4a375-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a375-120">Request headers</span></span>
|<span data-ttu-id="4a375-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4a375-121">Header</span></span>|<span data-ttu-id="4a375-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4a375-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a375-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a375-123">Authorization</span></span>|<span data-ttu-id="4a375-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a375-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a375-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4a375-125">Accept</span></span>|<span data-ttu-id="4a375-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a375-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a375-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a375-127">Request body</span></span>
<span data-ttu-id="4a375-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="4a375-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="4a375-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="4a375-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="4a375-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a375-130">Property</span></span>|<span data-ttu-id="4a375-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a375-131">Type</span></span>|<span data-ttu-id="4a375-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a375-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a375-133">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="4a375-133">inGracePeriodCount</span></span>|<span data-ttu-id="4a375-134">Int32</span><span class="sxs-lookup"><span data-stu-id="4a375-134">Int32</span></span>|<span data-ttu-id="4a375-135">Quantidade de dispositivos que estão no período de cortesia</span><span class="sxs-lookup"><span data-stu-id="4a375-135">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="4a375-136">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="4a375-136">configManagerCount</span></span>|<span data-ttu-id="4a375-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4a375-137">Int32</span></span>|<span data-ttu-id="4a375-138">Quantidade de dispositivos que estão em conformidade gerenciada pelo System Center Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="4a375-138">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="4a375-139">id</span><span class="sxs-lookup"><span data-stu-id="4a375-139">id</span></span>|<span data-ttu-id="4a375-140">String</span><span class="sxs-lookup"><span data-stu-id="4a375-140">String</span></span>|<span data-ttu-id="4a375-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4a375-141">Key of the entity.</span></span>|
|<span data-ttu-id="4a375-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4a375-142">unknownDeviceCount</span></span>|<span data-ttu-id="4a375-143">Int32</span><span class="sxs-lookup"><span data-stu-id="4a375-143">Int32</span></span>|<span data-ttu-id="4a375-144">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="4a375-144">Number of unknown devices</span></span>|
|<span data-ttu-id="4a375-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4a375-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="4a375-146">Int32</span><span class="sxs-lookup"><span data-stu-id="4a375-146">Int32</span></span>|<span data-ttu-id="4a375-147">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="4a375-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="4a375-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4a375-148">compliantDeviceCount</span></span>|<span data-ttu-id="4a375-149">Int32</span><span class="sxs-lookup"><span data-stu-id="4a375-149">Int32</span></span>|<span data-ttu-id="4a375-150">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="4a375-150">Number of compliant devices</span></span>|
|<span data-ttu-id="4a375-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4a375-151">remediatedDeviceCount</span></span>|<span data-ttu-id="4a375-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4a375-152">Int32</span></span>|<span data-ttu-id="4a375-153">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="4a375-153">Number of remediated devices</span></span>|
|<span data-ttu-id="4a375-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4a375-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="4a375-155">Int32</span><span class="sxs-lookup"><span data-stu-id="4a375-155">Int32</span></span>|<span data-ttu-id="4a375-156">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="4a375-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="4a375-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4a375-157">errorDeviceCount</span></span>|<span data-ttu-id="4a375-158">Int32</span><span class="sxs-lookup"><span data-stu-id="4a375-158">Int32</span></span>|<span data-ttu-id="4a375-159">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="4a375-159">Number of error devices</span></span>|
|<span data-ttu-id="4a375-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4a375-160">conflictDeviceCount</span></span>|<span data-ttu-id="4a375-161">Int32</span><span class="sxs-lookup"><span data-stu-id="4a375-161">Int32</span></span>|<span data-ttu-id="4a375-162">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="4a375-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="4a375-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a375-163">Response</span></span>
<span data-ttu-id="4a375-164">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a375-164">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a375-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a375-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a375-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a375-166">Request</span></span>
<span data-ttu-id="4a375-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a375-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4a375-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a375-168">Response</span></span>
<span data-ttu-id="4a375-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a375-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





