---
title: Criar deviceManagementIntentDeviceSettingStateSummary
description: Criar um novo objeto deviceManagementIntentDeviceSettingStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ed53831d0f8cb04a440f46a721d62ff8883cfba6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343661"
---
# <a name="create-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="58c86-103">Criar deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="58c86-103">Create deviceManagementIntentDeviceSettingStateSummary</span></span>

> <span data-ttu-id="58c86-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="58c86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58c86-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58c86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58c86-106">Criar um novo objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="58c86-106">Create a new [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58c86-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58c86-107">Prerequisites</span></span>
<span data-ttu-id="58c86-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58c86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58c86-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58c86-110">Permission type</span></span>|<span data-ttu-id="58c86-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="58c86-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58c86-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58c86-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58c86-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58c86-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="58c86-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58c86-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58c86-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58c86-115">Not supported.</span></span>|
|<span data-ttu-id="58c86-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58c86-116">Application</span></span>|<span data-ttu-id="58c86-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58c86-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58c86-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58c86-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="58c86-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58c86-119">Request headers</span></span>
|<span data-ttu-id="58c86-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58c86-120">Header</span></span>|<span data-ttu-id="58c86-121">Valor</span><span class="sxs-lookup"><span data-stu-id="58c86-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58c86-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="58c86-122">Authorization</span></span>|<span data-ttu-id="58c86-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58c86-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58c86-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="58c86-124">Accept</span></span>|<span data-ttu-id="58c86-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58c86-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58c86-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58c86-126">Request body</span></span>
<span data-ttu-id="58c86-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementIntentDeviceSettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="58c86-127">In the request body, supply a JSON representation for the deviceManagementIntentDeviceSettingStateSummary object.</span></span>

<span data-ttu-id="58c86-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementIntentDeviceSettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="58c86-128">The following table shows the properties that are required when you create the deviceManagementIntentDeviceSettingStateSummary.</span></span>

|<span data-ttu-id="58c86-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58c86-129">Property</span></span>|<span data-ttu-id="58c86-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="58c86-130">Type</span></span>|<span data-ttu-id="58c86-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="58c86-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58c86-132">id</span><span class="sxs-lookup"><span data-stu-id="58c86-132">id</span></span>|<span data-ttu-id="58c86-133">String</span><span class="sxs-lookup"><span data-stu-id="58c86-133">String</span></span>|<span data-ttu-id="58c86-134">A ID</span><span class="sxs-lookup"><span data-stu-id="58c86-134">The ID</span></span>|
|<span data-ttu-id="58c86-135">settingName</span><span class="sxs-lookup"><span data-stu-id="58c86-135">settingName</span></span>|<span data-ttu-id="58c86-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58c86-136">String</span></span>|<span data-ttu-id="58c86-137">Nome de uma configuração</span><span class="sxs-lookup"><span data-stu-id="58c86-137">Name of a setting</span></span>|
|<span data-ttu-id="58c86-138">compliantCount</span><span class="sxs-lookup"><span data-stu-id="58c86-138">compliantCount</span></span>|<span data-ttu-id="58c86-139">Int32</span><span class="sxs-lookup"><span data-stu-id="58c86-139">Int32</span></span>|<span data-ttu-id="58c86-140">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="58c86-140">Number of compliant devices</span></span>|
|<span data-ttu-id="58c86-141">conflictCount</span><span class="sxs-lookup"><span data-stu-id="58c86-141">conflictCount</span></span>|<span data-ttu-id="58c86-142">Int32</span><span class="sxs-lookup"><span data-stu-id="58c86-142">Int32</span></span>|<span data-ttu-id="58c86-143">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="58c86-143">Number of devices in conflict</span></span>|
|<span data-ttu-id="58c86-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="58c86-144">errorCount</span></span>|<span data-ttu-id="58c86-145">Int32</span><span class="sxs-lookup"><span data-stu-id="58c86-145">Int32</span></span>|<span data-ttu-id="58c86-146">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="58c86-146">Number of error devices</span></span>|
|<span data-ttu-id="58c86-147">nonCompliantCount</span><span class="sxs-lookup"><span data-stu-id="58c86-147">nonCompliantCount</span></span>|<span data-ttu-id="58c86-148">Int32</span><span class="sxs-lookup"><span data-stu-id="58c86-148">Int32</span></span>|<span data-ttu-id="58c86-149">Número de dispositivos não compatíveis</span><span class="sxs-lookup"><span data-stu-id="58c86-149">Number of non compliant devices</span></span>|
|<span data-ttu-id="58c86-150">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="58c86-150">notApplicableCount</span></span>|<span data-ttu-id="58c86-151">Int32</span><span class="sxs-lookup"><span data-stu-id="58c86-151">Int32</span></span>|<span data-ttu-id="58c86-152">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="58c86-152">Number of not applicable devices</span></span>|
|<span data-ttu-id="58c86-153">remediatedCount</span><span class="sxs-lookup"><span data-stu-id="58c86-153">remediatedCount</span></span>|<span data-ttu-id="58c86-154">Int32</span><span class="sxs-lookup"><span data-stu-id="58c86-154">Int32</span></span>|<span data-ttu-id="58c86-155">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="58c86-155">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="58c86-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="58c86-156">Response</span></span>
<span data-ttu-id="58c86-157">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58c86-157">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58c86-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58c86-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="58c86-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58c86-159">Request</span></span>
<span data-ttu-id="58c86-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58c86-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
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

### <a name="response"></a><span data-ttu-id="58c86-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="58c86-161">Response</span></span>
<span data-ttu-id="58c86-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58c86-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






