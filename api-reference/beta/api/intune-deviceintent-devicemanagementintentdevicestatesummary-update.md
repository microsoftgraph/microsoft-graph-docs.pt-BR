---
title: Atualizar deviceManagementIntentDeviceStateSummary
description: Atualiza as propriedades de um objeto deviceManagementIntentDeviceStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9e0773814d4b3666bf3999000db38ad3ec584fe2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48014613"
---
# <a name="update-devicemanagementintentdevicestatesummary"></a><span data-ttu-id="4dc38-103">Atualizar deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="4dc38-103">Update deviceManagementIntentDeviceStateSummary</span></span>

<span data-ttu-id="4dc38-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dc38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4dc38-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4dc38-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4dc38-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4dc38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dc38-107">Atualiza as propriedades de um objeto [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="4dc38-107">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4dc38-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4dc38-108">Prerequisites</span></span>
<span data-ttu-id="4dc38-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dc38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dc38-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4dc38-111">Permission type</span></span>|<span data-ttu-id="4dc38-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4dc38-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dc38-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4dc38-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4dc38-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dc38-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4dc38-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4dc38-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dc38-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4dc38-116">Not supported.</span></span>|
|<span data-ttu-id="4dc38-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4dc38-117">Application</span></span>|<span data-ttu-id="4dc38-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dc38-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dc38-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4dc38-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="4dc38-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4dc38-120">Request headers</span></span>
|<span data-ttu-id="4dc38-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4dc38-121">Header</span></span>|<span data-ttu-id="4dc38-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4dc38-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4dc38-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4dc38-123">Authorization</span></span>|<span data-ttu-id="4dc38-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4dc38-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4dc38-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4dc38-125">Accept</span></span>|<span data-ttu-id="4dc38-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4dc38-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dc38-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4dc38-127">Request body</span></span>
<span data-ttu-id="4dc38-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="4dc38-128">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

<span data-ttu-id="4dc38-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="4dc38-129">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md).</span></span>

|<span data-ttu-id="4dc38-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4dc38-130">Property</span></span>|<span data-ttu-id="4dc38-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4dc38-131">Type</span></span>|<span data-ttu-id="4dc38-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dc38-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dc38-133">id</span><span class="sxs-lookup"><span data-stu-id="4dc38-133">id</span></span>|<span data-ttu-id="4dc38-134">String</span><span class="sxs-lookup"><span data-stu-id="4dc38-134">String</span></span>|<span data-ttu-id="4dc38-135">A ID</span><span class="sxs-lookup"><span data-stu-id="4dc38-135">The ID</span></span>|
|<span data-ttu-id="4dc38-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="4dc38-136">conflictCount</span></span>|<span data-ttu-id="4dc38-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4dc38-137">Int32</span></span>|<span data-ttu-id="4dc38-138">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="4dc38-138">Number of devices in conflict</span></span>|
|<span data-ttu-id="4dc38-139">errorCount</span><span class="sxs-lookup"><span data-stu-id="4dc38-139">errorCount</span></span>|<span data-ttu-id="4dc38-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4dc38-140">Int32</span></span>|<span data-ttu-id="4dc38-141">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="4dc38-141">Number of error devices</span></span>|
|<span data-ttu-id="4dc38-142">failedCount</span><span class="sxs-lookup"><span data-stu-id="4dc38-142">failedCount</span></span>|<span data-ttu-id="4dc38-143">Int32</span><span class="sxs-lookup"><span data-stu-id="4dc38-143">Int32</span></span>|<span data-ttu-id="4dc38-144">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="4dc38-144">Number of failed devices</span></span>|
|<span data-ttu-id="4dc38-145">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="4dc38-145">notApplicableCount</span></span>|<span data-ttu-id="4dc38-146">Int32</span><span class="sxs-lookup"><span data-stu-id="4dc38-146">Int32</span></span>|<span data-ttu-id="4dc38-147">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="4dc38-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="4dc38-148">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="4dc38-148">notApplicablePlatformCount</span></span>|<span data-ttu-id="4dc38-149">Int32</span><span class="sxs-lookup"><span data-stu-id="4dc38-149">Int32</span></span>|<span data-ttu-id="4dc38-150">Número de dispositivos não aplicáveis devido à plataforma e à política incompatíveis</span><span class="sxs-lookup"><span data-stu-id="4dc38-150">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="4dc38-151">successCount</span><span class="sxs-lookup"><span data-stu-id="4dc38-151">successCount</span></span>|<span data-ttu-id="4dc38-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4dc38-152">Int32</span></span>|<span data-ttu-id="4dc38-153">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="4dc38-153">Number of succeeded devices</span></span>|



## <a name="response"></a><span data-ttu-id="4dc38-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dc38-154">Response</span></span>
<span data-ttu-id="4dc38-155">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4dc38-155">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dc38-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4dc38-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="4dc38-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4dc38-157">Request</span></span>
<span data-ttu-id="4dc38-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4dc38-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4dc38-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dc38-159">Response</span></span>
<span data-ttu-id="4dc38-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4dc38-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






