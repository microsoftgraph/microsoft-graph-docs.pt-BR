---
title: Atualizar deviceManagementIntentDeviceSettingStateSummary
description: Atualiza as propriedades de um objeto deviceManagementIntentDeviceSettingStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de67ed447a9ab3c35491c9efce03f5d22f63a129
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33916116"
---
# <a name="update-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="4c981-103">Atualizar deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="4c981-103">Update deviceManagementIntentDeviceSettingStateSummary</span></span>

> <span data-ttu-id="4c981-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4c981-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c981-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4c981-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c981-106">Atualiza as propriedades de um objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="4c981-106">Update the properties of a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c981-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4c981-107">Prerequisites</span></span>
<span data-ttu-id="4c981-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c981-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c981-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c981-110">Permission type</span></span>|<span data-ttu-id="4c981-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4c981-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c981-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c981-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c981-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c981-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c981-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c981-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c981-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c981-115">Not supported.</span></span>|
|<span data-ttu-id="4c981-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c981-116">Application</span></span>|<span data-ttu-id="4c981-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c981-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c981-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c981-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="4c981-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c981-119">Request headers</span></span>
|<span data-ttu-id="4c981-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c981-120">Header</span></span>|<span data-ttu-id="4c981-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4c981-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c981-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c981-122">Authorization</span></span>|<span data-ttu-id="4c981-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c981-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c981-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4c981-124">Accept</span></span>|<span data-ttu-id="4c981-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c981-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c981-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c981-126">Request body</span></span>
<span data-ttu-id="4c981-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="4c981-127">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

<span data-ttu-id="4c981-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="4c981-128">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span></span>

|<span data-ttu-id="4c981-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c981-129">Property</span></span>|<span data-ttu-id="4c981-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c981-130">Type</span></span>|<span data-ttu-id="4c981-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c981-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c981-132">id</span><span class="sxs-lookup"><span data-stu-id="4c981-132">id</span></span>|<span data-ttu-id="4c981-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c981-133">String</span></span>|<span data-ttu-id="4c981-134">A ID</span><span class="sxs-lookup"><span data-stu-id="4c981-134">The ID</span></span>|
|<span data-ttu-id="4c981-135">settingName</span><span class="sxs-lookup"><span data-stu-id="4c981-135">settingName</span></span>|<span data-ttu-id="4c981-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c981-136">String</span></span>|<span data-ttu-id="4c981-137">Nome de uma configuração</span><span class="sxs-lookup"><span data-stu-id="4c981-137">Name of a setting</span></span>|
|<span data-ttu-id="4c981-138">compliantCount</span><span class="sxs-lookup"><span data-stu-id="4c981-138">compliantCount</span></span>|<span data-ttu-id="4c981-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4c981-139">Int32</span></span>|<span data-ttu-id="4c981-140">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="4c981-140">Number of compliant devices</span></span>|
|<span data-ttu-id="4c981-141">conflictCount</span><span class="sxs-lookup"><span data-stu-id="4c981-141">conflictCount</span></span>|<span data-ttu-id="4c981-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4c981-142">Int32</span></span>|<span data-ttu-id="4c981-143">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="4c981-143">Number of devices in conflict</span></span>|
|<span data-ttu-id="4c981-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="4c981-144">errorCount</span></span>|<span data-ttu-id="4c981-145">Int32</span><span class="sxs-lookup"><span data-stu-id="4c981-145">Int32</span></span>|<span data-ttu-id="4c981-146">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="4c981-146">Number of error devices</span></span>|
|<span data-ttu-id="4c981-147">nonCompliantCount</span><span class="sxs-lookup"><span data-stu-id="4c981-147">nonCompliantCount</span></span>|<span data-ttu-id="4c981-148">Int32</span><span class="sxs-lookup"><span data-stu-id="4c981-148">Int32</span></span>|<span data-ttu-id="4c981-149">Número de dispositivos não compatíveis</span><span class="sxs-lookup"><span data-stu-id="4c981-149">Number of non compliant devices</span></span>|
|<span data-ttu-id="4c981-150">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="4c981-150">notApplicableCount</span></span>|<span data-ttu-id="4c981-151">Int32</span><span class="sxs-lookup"><span data-stu-id="4c981-151">Int32</span></span>|<span data-ttu-id="4c981-152">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="4c981-152">Number of not applicable devices</span></span>|
|<span data-ttu-id="4c981-153">remediatedCount</span><span class="sxs-lookup"><span data-stu-id="4c981-153">remediatedCount</span></span>|<span data-ttu-id="4c981-154">Int32</span><span class="sxs-lookup"><span data-stu-id="4c981-154">Int32</span></span>|<span data-ttu-id="4c981-155">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="4c981-155">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="4c981-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c981-156">Response</span></span>
<span data-ttu-id="4c981-157">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c981-157">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c981-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c981-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c981-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c981-159">Request</span></span>
<span data-ttu-id="4c981-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c981-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
Content-type: application/json
Content-length: 280

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "settingName": "Setting Name value",
  "compliantCount": 14,
  "conflictCount": 13,
  "errorCount": 10,
  "nonCompliantCount": 1,
  "notApplicableCount": 2,
  "remediatedCount": 15
}
```

### <a name="response"></a><span data-ttu-id="4c981-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c981-161">Response</span></span>
<span data-ttu-id="4c981-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c981-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 329

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "id": "d3d3a75f-a75f-d3d3-5fa7-d3d35fa7d3d3",
  "settingName": "Setting Name value",
  "compliantCount": 14,
  "conflictCount": 13,
  "errorCount": 10,
  "nonCompliantCount": 1,
  "notApplicableCount": 2,
  "remediatedCount": 15
}
```




