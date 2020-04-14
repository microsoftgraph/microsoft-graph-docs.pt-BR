---
title: Criar deviceManagementIntentDeviceSettingStateSummary
description: Criar um novo objeto deviceManagementIntentDeviceSettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 187f194080922288d36f9cb5c4a91713e61bc5d2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43326924"
---
# <a name="create-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="2eb76-103">Criar deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="2eb76-103">Create deviceManagementIntentDeviceSettingStateSummary</span></span>

<span data-ttu-id="2eb76-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2eb76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2eb76-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2eb76-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2eb76-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2eb76-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2eb76-107">Criar um novo objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="2eb76-107">Create a new [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2eb76-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2eb76-108">Prerequisites</span></span>
<span data-ttu-id="2eb76-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2eb76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2eb76-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2eb76-111">Permission type</span></span>|<span data-ttu-id="2eb76-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2eb76-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2eb76-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2eb76-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2eb76-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eb76-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2eb76-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2eb76-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2eb76-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2eb76-116">Not supported.</span></span>|
|<span data-ttu-id="2eb76-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2eb76-117">Application</span></span>|<span data-ttu-id="2eb76-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eb76-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2eb76-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2eb76-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="2eb76-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2eb76-120">Request headers</span></span>
|<span data-ttu-id="2eb76-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2eb76-121">Header</span></span>|<span data-ttu-id="2eb76-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2eb76-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2eb76-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2eb76-123">Authorization</span></span>|<span data-ttu-id="2eb76-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2eb76-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2eb76-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2eb76-125">Accept</span></span>|<span data-ttu-id="2eb76-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2eb76-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2eb76-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2eb76-127">Request body</span></span>
<span data-ttu-id="2eb76-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementIntentDeviceSettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="2eb76-128">In the request body, supply a JSON representation for the deviceManagementIntentDeviceSettingStateSummary object.</span></span>

<span data-ttu-id="2eb76-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementIntentDeviceSettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="2eb76-129">The following table shows the properties that are required when you create the deviceManagementIntentDeviceSettingStateSummary.</span></span>

|<span data-ttu-id="2eb76-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2eb76-130">Property</span></span>|<span data-ttu-id="2eb76-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2eb76-131">Type</span></span>|<span data-ttu-id="2eb76-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2eb76-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2eb76-133">id</span><span class="sxs-lookup"><span data-stu-id="2eb76-133">id</span></span>|<span data-ttu-id="2eb76-134">String</span><span class="sxs-lookup"><span data-stu-id="2eb76-134">String</span></span>|<span data-ttu-id="2eb76-135">A ID</span><span class="sxs-lookup"><span data-stu-id="2eb76-135">The ID</span></span>|
|<span data-ttu-id="2eb76-136">settingName</span><span class="sxs-lookup"><span data-stu-id="2eb76-136">settingName</span></span>|<span data-ttu-id="2eb76-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2eb76-137">String</span></span>|<span data-ttu-id="2eb76-138">Nome de uma configuração</span><span class="sxs-lookup"><span data-stu-id="2eb76-138">Name of a setting</span></span>|
|<span data-ttu-id="2eb76-139">compliantCount</span><span class="sxs-lookup"><span data-stu-id="2eb76-139">compliantCount</span></span>|<span data-ttu-id="2eb76-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2eb76-140">Int32</span></span>|<span data-ttu-id="2eb76-141">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="2eb76-141">Number of compliant devices</span></span>|
|<span data-ttu-id="2eb76-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="2eb76-142">conflictCount</span></span>|<span data-ttu-id="2eb76-143">Int32</span><span class="sxs-lookup"><span data-stu-id="2eb76-143">Int32</span></span>|<span data-ttu-id="2eb76-144">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="2eb76-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="2eb76-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="2eb76-145">errorCount</span></span>|<span data-ttu-id="2eb76-146">Int32</span><span class="sxs-lookup"><span data-stu-id="2eb76-146">Int32</span></span>|<span data-ttu-id="2eb76-147">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="2eb76-147">Number of error devices</span></span>|
|<span data-ttu-id="2eb76-148">nonCompliantCount</span><span class="sxs-lookup"><span data-stu-id="2eb76-148">nonCompliantCount</span></span>|<span data-ttu-id="2eb76-149">Int32</span><span class="sxs-lookup"><span data-stu-id="2eb76-149">Int32</span></span>|<span data-ttu-id="2eb76-150">Número de dispositivos não compatíveis</span><span class="sxs-lookup"><span data-stu-id="2eb76-150">Number of non compliant devices</span></span>|
|<span data-ttu-id="2eb76-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="2eb76-151">notApplicableCount</span></span>|<span data-ttu-id="2eb76-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2eb76-152">Int32</span></span>|<span data-ttu-id="2eb76-153">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="2eb76-153">Number of not applicable devices</span></span>|
|<span data-ttu-id="2eb76-154">remediatedCount</span><span class="sxs-lookup"><span data-stu-id="2eb76-154">remediatedCount</span></span>|<span data-ttu-id="2eb76-155">Int32</span><span class="sxs-lookup"><span data-stu-id="2eb76-155">Int32</span></span>|<span data-ttu-id="2eb76-156">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="2eb76-156">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="2eb76-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="2eb76-157">Response</span></span>
<span data-ttu-id="2eb76-158">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2eb76-158">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2eb76-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2eb76-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="2eb76-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2eb76-160">Request</span></span>
<span data-ttu-id="2eb76-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2eb76-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2eb76-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="2eb76-162">Response</span></span>
<span data-ttu-id="2eb76-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2eb76-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



