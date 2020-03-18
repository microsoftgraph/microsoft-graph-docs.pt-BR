---
title: Atualizar deviceManagementIntentDeviceSettingStateSummary
description: Atualiza as propriedades de um objeto deviceManagementIntentDeviceSettingStateSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 875fef3c6dcf6b14725896949f5b19a0a9e8698b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815272"
---
# <a name="update-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="3e181-103">Atualizar deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="3e181-103">Update deviceManagementIntentDeviceSettingStateSummary</span></span>

> <span data-ttu-id="3e181-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3e181-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e181-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3e181-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e181-106">Atualiza as propriedades de um objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="3e181-106">Update the properties of a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e181-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3e181-107">Prerequisites</span></span>
<span data-ttu-id="3e181-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e181-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e181-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e181-110">Permission type</span></span>|<span data-ttu-id="3e181-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3e181-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e181-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e181-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3e181-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e181-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3e181-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e181-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e181-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e181-115">Not supported.</span></span>|
|<span data-ttu-id="3e181-116">Application</span><span class="sxs-lookup"><span data-stu-id="3e181-116">Application</span></span>|<span data-ttu-id="3e181-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e181-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e181-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e181-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="3e181-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e181-119">Request headers</span></span>
|<span data-ttu-id="3e181-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3e181-120">Header</span></span>|<span data-ttu-id="3e181-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3e181-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e181-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e181-122">Authorization</span></span>|<span data-ttu-id="3e181-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e181-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e181-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3e181-124">Accept</span></span>|<span data-ttu-id="3e181-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3e181-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e181-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e181-126">Request body</span></span>
<span data-ttu-id="3e181-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="3e181-127">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

<span data-ttu-id="3e181-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3e181-128">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span></span>

|<span data-ttu-id="3e181-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e181-129">Property</span></span>|<span data-ttu-id="3e181-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e181-130">Type</span></span>|<span data-ttu-id="3e181-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e181-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e181-132">id</span><span class="sxs-lookup"><span data-stu-id="3e181-132">id</span></span>|<span data-ttu-id="3e181-133">String</span><span class="sxs-lookup"><span data-stu-id="3e181-133">String</span></span>|<span data-ttu-id="3e181-134">A ID</span><span class="sxs-lookup"><span data-stu-id="3e181-134">The ID</span></span>|
|<span data-ttu-id="3e181-135">settingName</span><span class="sxs-lookup"><span data-stu-id="3e181-135">settingName</span></span>|<span data-ttu-id="3e181-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e181-136">String</span></span>|<span data-ttu-id="3e181-137">Nome de uma configuração</span><span class="sxs-lookup"><span data-stu-id="3e181-137">Name of a setting</span></span>|
|<span data-ttu-id="3e181-138">compliantCount</span><span class="sxs-lookup"><span data-stu-id="3e181-138">compliantCount</span></span>|<span data-ttu-id="3e181-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3e181-139">Int32</span></span>|<span data-ttu-id="3e181-140">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="3e181-140">Number of compliant devices</span></span>|
|<span data-ttu-id="3e181-141">conflictCount</span><span class="sxs-lookup"><span data-stu-id="3e181-141">conflictCount</span></span>|<span data-ttu-id="3e181-142">Int32</span><span class="sxs-lookup"><span data-stu-id="3e181-142">Int32</span></span>|<span data-ttu-id="3e181-143">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="3e181-143">Number of devices in conflict</span></span>|
|<span data-ttu-id="3e181-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="3e181-144">errorCount</span></span>|<span data-ttu-id="3e181-145">Int32</span><span class="sxs-lookup"><span data-stu-id="3e181-145">Int32</span></span>|<span data-ttu-id="3e181-146">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="3e181-146">Number of error devices</span></span>|
|<span data-ttu-id="3e181-147">nonCompliantCount</span><span class="sxs-lookup"><span data-stu-id="3e181-147">nonCompliantCount</span></span>|<span data-ttu-id="3e181-148">Int32</span><span class="sxs-lookup"><span data-stu-id="3e181-148">Int32</span></span>|<span data-ttu-id="3e181-149">Número de dispositivos não compatíveis</span><span class="sxs-lookup"><span data-stu-id="3e181-149">Number of non compliant devices</span></span>|
|<span data-ttu-id="3e181-150">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="3e181-150">notApplicableCount</span></span>|<span data-ttu-id="3e181-151">Int32</span><span class="sxs-lookup"><span data-stu-id="3e181-151">Int32</span></span>|<span data-ttu-id="3e181-152">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="3e181-152">Number of not applicable devices</span></span>|
|<span data-ttu-id="3e181-153">remediatedCount</span><span class="sxs-lookup"><span data-stu-id="3e181-153">remediatedCount</span></span>|<span data-ttu-id="3e181-154">Int32</span><span class="sxs-lookup"><span data-stu-id="3e181-154">Int32</span></span>|<span data-ttu-id="3e181-155">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="3e181-155">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="3e181-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e181-156">Response</span></span>
<span data-ttu-id="3e181-157">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e181-157">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e181-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e181-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e181-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e181-159">Request</span></span>
<span data-ttu-id="3e181-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e181-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3e181-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e181-161">Response</span></span>
<span data-ttu-id="3e181-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e181-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




