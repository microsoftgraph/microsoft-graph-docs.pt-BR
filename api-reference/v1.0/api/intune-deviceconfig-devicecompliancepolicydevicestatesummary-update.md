---
title: Atualizar deviceCompliancePolicyDeviceStateSummary
description: Atualizar as propriedades de um objeto deviceCompliancePolicyDeviceStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 65193c1bfd77a947f707a19b976a62700a35d2f4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43399946"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="c48dd-103">Atualizar deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c48dd-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

<span data-ttu-id="c48dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c48dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c48dd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c48dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c48dd-106">Atualizar as propriedades de um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c48dd-106">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c48dd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c48dd-107">Prerequisites</span></span>
<span data-ttu-id="c48dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c48dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c48dd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c48dd-110">Permission type</span></span>|<span data-ttu-id="c48dd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c48dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c48dd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c48dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c48dd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c48dd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c48dd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c48dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c48dd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c48dd-115">Not supported.</span></span>|
|<span data-ttu-id="c48dd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c48dd-116">Application</span></span>|<span data-ttu-id="c48dd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c48dd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c48dd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c48dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="c48dd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c48dd-119">Request headers</span></span>
|<span data-ttu-id="c48dd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c48dd-120">Header</span></span>|<span data-ttu-id="c48dd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c48dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c48dd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c48dd-122">Authorization</span></span>|<span data-ttu-id="c48dd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c48dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c48dd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c48dd-124">Accept</span></span>|<span data-ttu-id="c48dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c48dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c48dd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c48dd-126">Request body</span></span>
<span data-ttu-id="c48dd-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c48dd-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="c48dd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c48dd-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="c48dd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c48dd-129">Property</span></span>|<span data-ttu-id="c48dd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c48dd-130">Type</span></span>|<span data-ttu-id="c48dd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c48dd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c48dd-132">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="c48dd-132">inGracePeriodCount</span></span>|<span data-ttu-id="c48dd-133">Int32</span><span class="sxs-lookup"><span data-stu-id="c48dd-133">Int32</span></span>|<span data-ttu-id="c48dd-134">Quantidade de dispositivos que estão no período de cortesia</span><span class="sxs-lookup"><span data-stu-id="c48dd-134">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="c48dd-135">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="c48dd-135">configManagerCount</span></span>|<span data-ttu-id="c48dd-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c48dd-136">Int32</span></span>|<span data-ttu-id="c48dd-137">Quantidade de dispositivos que estão em conformidade gerenciada pelo System Center Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="c48dd-137">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="c48dd-138">id</span><span class="sxs-lookup"><span data-stu-id="c48dd-138">id</span></span>|<span data-ttu-id="c48dd-139">String</span><span class="sxs-lookup"><span data-stu-id="c48dd-139">String</span></span>|<span data-ttu-id="c48dd-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c48dd-140">Key of the entity.</span></span>|
|<span data-ttu-id="c48dd-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c48dd-141">unknownDeviceCount</span></span>|<span data-ttu-id="c48dd-142">Int32</span><span class="sxs-lookup"><span data-stu-id="c48dd-142">Int32</span></span>|<span data-ttu-id="c48dd-143">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="c48dd-143">Number of unknown devices</span></span>|
|<span data-ttu-id="c48dd-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c48dd-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="c48dd-145">Int32</span><span class="sxs-lookup"><span data-stu-id="c48dd-145">Int32</span></span>|<span data-ttu-id="c48dd-146">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="c48dd-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="c48dd-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c48dd-147">compliantDeviceCount</span></span>|<span data-ttu-id="c48dd-148">Int32</span><span class="sxs-lookup"><span data-stu-id="c48dd-148">Int32</span></span>|<span data-ttu-id="c48dd-149">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="c48dd-149">Number of compliant devices</span></span>|
|<span data-ttu-id="c48dd-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c48dd-150">remediatedDeviceCount</span></span>|<span data-ttu-id="c48dd-151">Int32</span><span class="sxs-lookup"><span data-stu-id="c48dd-151">Int32</span></span>|<span data-ttu-id="c48dd-152">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="c48dd-152">Number of remediated devices</span></span>|
|<span data-ttu-id="c48dd-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c48dd-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="c48dd-154">Int32</span><span class="sxs-lookup"><span data-stu-id="c48dd-154">Int32</span></span>|<span data-ttu-id="c48dd-155">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="c48dd-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="c48dd-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c48dd-156">errorDeviceCount</span></span>|<span data-ttu-id="c48dd-157">Int32</span><span class="sxs-lookup"><span data-stu-id="c48dd-157">Int32</span></span>|<span data-ttu-id="c48dd-158">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="c48dd-158">Number of error devices</span></span>|
|<span data-ttu-id="c48dd-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c48dd-159">conflictDeviceCount</span></span>|<span data-ttu-id="c48dd-160">Int32</span><span class="sxs-lookup"><span data-stu-id="c48dd-160">Int32</span></span>|<span data-ttu-id="c48dd-161">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="c48dd-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="c48dd-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="c48dd-162">Response</span></span>
<span data-ttu-id="c48dd-163">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c48dd-163">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c48dd-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c48dd-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="c48dd-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c48dd-165">Request</span></span>
<span data-ttu-id="c48dd-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c48dd-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c48dd-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="c48dd-167">Response</span></span>
<span data-ttu-id="c48dd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c48dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






