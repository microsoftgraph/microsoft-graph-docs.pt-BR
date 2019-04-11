---
title: Atualizar deviceCompliancePolicyDeviceStateSummary
description: Atualizar as propriedades de um objeto deviceCompliancePolicyDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e09bf9e326a0d422b1b6ff23e2927141a6f32e41
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807634"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="b7e92-103">Atualizar deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="b7e92-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="b7e92-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b7e92-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7e92-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b7e92-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7e92-106">Atualizar as propriedades de um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="b7e92-106">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7e92-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b7e92-107">Prerequisites</span></span>
<span data-ttu-id="b7e92-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7e92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7e92-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7e92-110">Permission type</span></span>|<span data-ttu-id="b7e92-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b7e92-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7e92-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7e92-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7e92-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7e92-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b7e92-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7e92-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7e92-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7e92-115">Not supported.</span></span>|
|<span data-ttu-id="b7e92-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7e92-116">Application</span></span>|<span data-ttu-id="b7e92-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7e92-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7e92-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7e92-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="b7e92-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7e92-119">Request headers</span></span>
|<span data-ttu-id="b7e92-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7e92-120">Header</span></span>|<span data-ttu-id="b7e92-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b7e92-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7e92-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7e92-122">Authorization</span></span>|<span data-ttu-id="b7e92-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7e92-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7e92-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b7e92-124">Accept</span></span>|<span data-ttu-id="b7e92-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7e92-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7e92-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7e92-126">Request body</span></span>
<span data-ttu-id="b7e92-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="b7e92-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="b7e92-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="b7e92-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="b7e92-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7e92-129">Property</span></span>|<span data-ttu-id="b7e92-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7e92-130">Type</span></span>|<span data-ttu-id="b7e92-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7e92-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7e92-132">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="b7e92-132">inGracePeriodCount</span></span>|<span data-ttu-id="b7e92-133">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e92-133">Int32</span></span>|<span data-ttu-id="b7e92-134">Quantidade de dispositivos que estão no período de cortesia</span><span class="sxs-lookup"><span data-stu-id="b7e92-134">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="b7e92-135">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="b7e92-135">configManagerCount</span></span>|<span data-ttu-id="b7e92-136">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e92-136">Int32</span></span>|<span data-ttu-id="b7e92-137">Quantidade de dispositivos que estão em conformidade gerenciada pelo System Center Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="b7e92-137">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="b7e92-138">id</span><span class="sxs-lookup"><span data-stu-id="b7e92-138">id</span></span>|<span data-ttu-id="b7e92-139">String</span><span class="sxs-lookup"><span data-stu-id="b7e92-139">String</span></span>|<span data-ttu-id="b7e92-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b7e92-140">Key of the entity.</span></span>|
|<span data-ttu-id="b7e92-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b7e92-141">unknownDeviceCount</span></span>|<span data-ttu-id="b7e92-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e92-142">Int32</span></span>|<span data-ttu-id="b7e92-143">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="b7e92-143">Number of unknown devices</span></span>|
|<span data-ttu-id="b7e92-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b7e92-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="b7e92-145">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e92-145">Int32</span></span>|<span data-ttu-id="b7e92-146">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="b7e92-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="b7e92-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b7e92-147">compliantDeviceCount</span></span>|<span data-ttu-id="b7e92-148">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e92-148">Int32</span></span>|<span data-ttu-id="b7e92-149">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="b7e92-149">Number of compliant devices</span></span>|
|<span data-ttu-id="b7e92-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b7e92-150">remediatedDeviceCount</span></span>|<span data-ttu-id="b7e92-151">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e92-151">Int32</span></span>|<span data-ttu-id="b7e92-152">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="b7e92-152">Number of remediated devices</span></span>|
|<span data-ttu-id="b7e92-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b7e92-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="b7e92-154">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e92-154">Int32</span></span>|<span data-ttu-id="b7e92-155">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="b7e92-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="b7e92-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b7e92-156">errorDeviceCount</span></span>|<span data-ttu-id="b7e92-157">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e92-157">Int32</span></span>|<span data-ttu-id="b7e92-158">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="b7e92-158">Number of error devices</span></span>|
|<span data-ttu-id="b7e92-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b7e92-159">conflictDeviceCount</span></span>|<span data-ttu-id="b7e92-160">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e92-160">Int32</span></span>|<span data-ttu-id="b7e92-161">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="b7e92-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="b7e92-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7e92-162">Response</span></span>
<span data-ttu-id="b7e92-163">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7e92-163">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7e92-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7e92-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7e92-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7e92-165">Request</span></span>
<span data-ttu-id="b7e92-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7e92-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b7e92-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7e92-167">Response</span></span>
<span data-ttu-id="b7e92-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7e92-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





