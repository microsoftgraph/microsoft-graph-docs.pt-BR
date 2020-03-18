---
title: Atualizar deviceManagementIntentDeviceStateSummary
description: Atualiza as propriedades de um objeto deviceManagementIntentDeviceStateSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: de70cd0e2ac314dad0baaf271b57525be59b73af
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767726"
---
# <a name="update-devicemanagementintentdevicestatesummary"></a><span data-ttu-id="6b911-103">Atualizar deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="6b911-103">Update deviceManagementIntentDeviceStateSummary</span></span>

> <span data-ttu-id="6b911-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6b911-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b911-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b911-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b911-106">Atualiza as propriedades de um objeto [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="6b911-106">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b911-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6b911-107">Prerequisites</span></span>
<span data-ttu-id="6b911-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b911-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b911-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b911-110">Permission type</span></span>|<span data-ttu-id="6b911-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6b911-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b911-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b911-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b911-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b911-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b911-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b911-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b911-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b911-115">Not supported.</span></span>|
|<span data-ttu-id="6b911-116">Application</span><span class="sxs-lookup"><span data-stu-id="6b911-116">Application</span></span>|<span data-ttu-id="6b911-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b911-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b911-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b911-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="6b911-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b911-119">Request headers</span></span>
|<span data-ttu-id="6b911-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6b911-120">Header</span></span>|<span data-ttu-id="6b911-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6b911-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b911-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b911-122">Authorization</span></span>|<span data-ttu-id="6b911-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b911-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b911-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6b911-124">Accept</span></span>|<span data-ttu-id="6b911-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6b911-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b911-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b911-126">Request body</span></span>
<span data-ttu-id="6b911-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="6b911-127">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

<span data-ttu-id="6b911-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6b911-128">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md).</span></span>

|<span data-ttu-id="6b911-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b911-129">Property</span></span>|<span data-ttu-id="6b911-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b911-130">Type</span></span>|<span data-ttu-id="6b911-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b911-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b911-132">id</span><span class="sxs-lookup"><span data-stu-id="6b911-132">id</span></span>|<span data-ttu-id="6b911-133">String</span><span class="sxs-lookup"><span data-stu-id="6b911-133">String</span></span>|<span data-ttu-id="6b911-134">A ID</span><span class="sxs-lookup"><span data-stu-id="6b911-134">The ID</span></span>|
|<span data-ttu-id="6b911-135">conflictCount</span><span class="sxs-lookup"><span data-stu-id="6b911-135">conflictCount</span></span>|<span data-ttu-id="6b911-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6b911-136">Int32</span></span>|<span data-ttu-id="6b911-137">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="6b911-137">Number of devices in conflict</span></span>|
|<span data-ttu-id="6b911-138">errorCount</span><span class="sxs-lookup"><span data-stu-id="6b911-138">errorCount</span></span>|<span data-ttu-id="6b911-139">Int32</span><span class="sxs-lookup"><span data-stu-id="6b911-139">Int32</span></span>|<span data-ttu-id="6b911-140">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="6b911-140">Number of error devices</span></span>|
|<span data-ttu-id="6b911-141">failedCount</span><span class="sxs-lookup"><span data-stu-id="6b911-141">failedCount</span></span>|<span data-ttu-id="6b911-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6b911-142">Int32</span></span>|<span data-ttu-id="6b911-143">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="6b911-143">Number of failed devices</span></span>|
|<span data-ttu-id="6b911-144">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="6b911-144">notApplicableCount</span></span>|<span data-ttu-id="6b911-145">Int32</span><span class="sxs-lookup"><span data-stu-id="6b911-145">Int32</span></span>|<span data-ttu-id="6b911-146">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="6b911-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="6b911-147">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="6b911-147">notApplicablePlatformCount</span></span>|<span data-ttu-id="6b911-148">Int32</span><span class="sxs-lookup"><span data-stu-id="6b911-148">Int32</span></span>|<span data-ttu-id="6b911-149">Número de dispositivos não aplicáveis devido à plataforma e à política incompatíveis</span><span class="sxs-lookup"><span data-stu-id="6b911-149">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="6b911-150">successCount</span><span class="sxs-lookup"><span data-stu-id="6b911-150">successCount</span></span>|<span data-ttu-id="6b911-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6b911-151">Int32</span></span>|<span data-ttu-id="6b911-152">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="6b911-152">Number of succeeded devices</span></span>|



## <a name="response"></a><span data-ttu-id="6b911-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b911-153">Response</span></span>
<span data-ttu-id="6b911-154">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b911-154">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b911-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b911-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b911-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b911-156">Request</span></span>
<span data-ttu-id="6b911-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b911-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
Content-type: application/json
Content-length: 237

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12
}
```

### <a name="response"></a><span data-ttu-id="6b911-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b911-158">Response</span></span>
<span data-ttu-id="6b911-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b911-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 286

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "id": "12230bf9-0bf9-1223-f90b-2312f90b2312",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12
}
```




