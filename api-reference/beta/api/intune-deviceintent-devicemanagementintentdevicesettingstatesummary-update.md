---
title: Atualizar deviceManagementIntentDeviceSettingStateSummary
description: Atualiza as propriedades de um objeto deviceManagementIntentDeviceSettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 11c98bfa60a1bdcc8fc24a63d3dfe48bfb797b0d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43326554"
---
# <a name="update-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="8e3e0-103">Atualizar deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="8e3e0-103">Update deviceManagementIntentDeviceSettingStateSummary</span></span>

<span data-ttu-id="8e3e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e3e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e3e0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e3e0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e3e0-107">Atualiza as propriedades de um objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="8e3e0-107">Update the properties of a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e3e0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e3e0-108">Prerequisites</span></span>
<span data-ttu-id="8e3e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e3e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e3e0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e3e0-111">Permission type</span></span>|<span data-ttu-id="8e3e0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8e3e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e3e0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e3e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e3e0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e3e0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e3e0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e3e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e3e0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-116">Not supported.</span></span>|
|<span data-ttu-id="8e3e0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e3e0-117">Application</span></span>|<span data-ttu-id="8e3e0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e3e0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e3e0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e3e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="8e3e0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e3e0-120">Request headers</span></span>
|<span data-ttu-id="8e3e0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e3e0-121">Header</span></span>|<span data-ttu-id="8e3e0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8e3e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e3e0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e3e0-123">Authorization</span></span>|<span data-ttu-id="8e3e0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e3e0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8e3e0-125">Accept</span></span>|<span data-ttu-id="8e3e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e3e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e3e0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e3e0-127">Request body</span></span>
<span data-ttu-id="8e3e0-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="8e3e0-128">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

<span data-ttu-id="8e3e0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="8e3e0-129">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span></span>

|<span data-ttu-id="8e3e0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e3e0-130">Property</span></span>|<span data-ttu-id="8e3e0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e3e0-131">Type</span></span>|<span data-ttu-id="8e3e0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e3e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e3e0-133">id</span><span class="sxs-lookup"><span data-stu-id="8e3e0-133">id</span></span>|<span data-ttu-id="8e3e0-134">String</span><span class="sxs-lookup"><span data-stu-id="8e3e0-134">String</span></span>|<span data-ttu-id="8e3e0-135">A ID</span><span class="sxs-lookup"><span data-stu-id="8e3e0-135">The ID</span></span>|
|<span data-ttu-id="8e3e0-136">settingName</span><span class="sxs-lookup"><span data-stu-id="8e3e0-136">settingName</span></span>|<span data-ttu-id="8e3e0-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e3e0-137">String</span></span>|<span data-ttu-id="8e3e0-138">Nome de uma configuração</span><span class="sxs-lookup"><span data-stu-id="8e3e0-138">Name of a setting</span></span>|
|<span data-ttu-id="8e3e0-139">compliantCount</span><span class="sxs-lookup"><span data-stu-id="8e3e0-139">compliantCount</span></span>|<span data-ttu-id="8e3e0-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8e3e0-140">Int32</span></span>|<span data-ttu-id="8e3e0-141">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="8e3e0-141">Number of compliant devices</span></span>|
|<span data-ttu-id="8e3e0-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="8e3e0-142">conflictCount</span></span>|<span data-ttu-id="8e3e0-143">Int32</span><span class="sxs-lookup"><span data-stu-id="8e3e0-143">Int32</span></span>|<span data-ttu-id="8e3e0-144">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="8e3e0-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="8e3e0-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="8e3e0-145">errorCount</span></span>|<span data-ttu-id="8e3e0-146">Int32</span><span class="sxs-lookup"><span data-stu-id="8e3e0-146">Int32</span></span>|<span data-ttu-id="8e3e0-147">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="8e3e0-147">Number of error devices</span></span>|
|<span data-ttu-id="8e3e0-148">nonCompliantCount</span><span class="sxs-lookup"><span data-stu-id="8e3e0-148">nonCompliantCount</span></span>|<span data-ttu-id="8e3e0-149">Int32</span><span class="sxs-lookup"><span data-stu-id="8e3e0-149">Int32</span></span>|<span data-ttu-id="8e3e0-150">Número de dispositivos não compatíveis</span><span class="sxs-lookup"><span data-stu-id="8e3e0-150">Number of non compliant devices</span></span>|
|<span data-ttu-id="8e3e0-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="8e3e0-151">notApplicableCount</span></span>|<span data-ttu-id="8e3e0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8e3e0-152">Int32</span></span>|<span data-ttu-id="8e3e0-153">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="8e3e0-153">Number of not applicable devices</span></span>|
|<span data-ttu-id="8e3e0-154">remediatedCount</span><span class="sxs-lookup"><span data-stu-id="8e3e0-154">remediatedCount</span></span>|<span data-ttu-id="8e3e0-155">Int32</span><span class="sxs-lookup"><span data-stu-id="8e3e0-155">Int32</span></span>|<span data-ttu-id="8e3e0-156">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="8e3e0-156">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="8e3e0-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e3e0-157">Response</span></span>
<span data-ttu-id="8e3e0-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e3e0-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e3e0-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e3e0-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e3e0-160">Request</span></span>
<span data-ttu-id="8e3e0-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8e3e0-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e3e0-162">Response</span></span>
<span data-ttu-id="8e3e0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



