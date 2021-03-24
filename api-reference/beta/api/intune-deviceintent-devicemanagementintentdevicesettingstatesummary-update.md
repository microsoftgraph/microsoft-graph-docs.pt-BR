---
title: Atualizar deviceManagementIntentDeviceSettingStateSummary
description: Atualize as propriedades de um objeto deviceManagementIntentDeviceSettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: be1189953214b68196e10eefd36a9b055f5bb99d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132041"
---
# <a name="update-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="2d15f-103">Atualizar deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="2d15f-103">Update deviceManagementIntentDeviceSettingStateSummary</span></span>

<span data-ttu-id="2d15f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d15f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d15f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2d15f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d15f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d15f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d15f-107">Atualize as propriedades de [um objeto deviceManagementIntentDeviceSettingStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="2d15f-107">Update the properties of a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d15f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2d15f-108">Prerequisites</span></span>
<span data-ttu-id="2d15f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d15f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d15f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d15f-111">Permission type</span></span>|<span data-ttu-id="2d15f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2d15f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d15f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d15f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2d15f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d15f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d15f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d15f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d15f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d15f-116">Not supported.</span></span>|
|<span data-ttu-id="2d15f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d15f-117">Application</span></span>|<span data-ttu-id="2d15f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d15f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d15f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d15f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="2d15f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d15f-120">Request headers</span></span>
|<span data-ttu-id="2d15f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2d15f-121">Header</span></span>|<span data-ttu-id="2d15f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2d15f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d15f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d15f-123">Authorization</span></span>|<span data-ttu-id="2d15f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d15f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d15f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2d15f-125">Accept</span></span>|<span data-ttu-id="2d15f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2d15f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d15f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d15f-127">Request body</span></span>
<span data-ttu-id="2d15f-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementIntentDeviceSettingStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="2d15f-128">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

<span data-ttu-id="2d15f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="2d15f-129">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span></span>

|<span data-ttu-id="2d15f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d15f-130">Property</span></span>|<span data-ttu-id="2d15f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d15f-131">Type</span></span>|<span data-ttu-id="2d15f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d15f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d15f-133">id</span><span class="sxs-lookup"><span data-stu-id="2d15f-133">id</span></span>|<span data-ttu-id="2d15f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d15f-134">String</span></span>|<span data-ttu-id="2d15f-135">A ID</span><span class="sxs-lookup"><span data-stu-id="2d15f-135">The ID</span></span>|
|<span data-ttu-id="2d15f-136">settingName</span><span class="sxs-lookup"><span data-stu-id="2d15f-136">settingName</span></span>|<span data-ttu-id="2d15f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d15f-137">String</span></span>|<span data-ttu-id="2d15f-138">Nome de uma configuração</span><span class="sxs-lookup"><span data-stu-id="2d15f-138">Name of a setting</span></span>|
|<span data-ttu-id="2d15f-139">compliantCount</span><span class="sxs-lookup"><span data-stu-id="2d15f-139">compliantCount</span></span>|<span data-ttu-id="2d15f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2d15f-140">Int32</span></span>|<span data-ttu-id="2d15f-141">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="2d15f-141">Number of compliant devices</span></span>|
|<span data-ttu-id="2d15f-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="2d15f-142">conflictCount</span></span>|<span data-ttu-id="2d15f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="2d15f-143">Int32</span></span>|<span data-ttu-id="2d15f-144">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="2d15f-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="2d15f-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="2d15f-145">errorCount</span></span>|<span data-ttu-id="2d15f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="2d15f-146">Int32</span></span>|<span data-ttu-id="2d15f-147">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="2d15f-147">Number of error devices</span></span>|
|<span data-ttu-id="2d15f-148">nonCompliantCount</span><span class="sxs-lookup"><span data-stu-id="2d15f-148">nonCompliantCount</span></span>|<span data-ttu-id="2d15f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="2d15f-149">Int32</span></span>|<span data-ttu-id="2d15f-150">Número de dispositivos não compatíveis</span><span class="sxs-lookup"><span data-stu-id="2d15f-150">Number of non compliant devices</span></span>|
|<span data-ttu-id="2d15f-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="2d15f-151">notApplicableCount</span></span>|<span data-ttu-id="2d15f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2d15f-152">Int32</span></span>|<span data-ttu-id="2d15f-153">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="2d15f-153">Number of not applicable devices</span></span>|
|<span data-ttu-id="2d15f-154">remediatedCount</span><span class="sxs-lookup"><span data-stu-id="2d15f-154">remediatedCount</span></span>|<span data-ttu-id="2d15f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="2d15f-155">Int32</span></span>|<span data-ttu-id="2d15f-156">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="2d15f-156">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="2d15f-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d15f-157">Response</span></span>
<span data-ttu-id="2d15f-158">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d15f-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d15f-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d15f-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d15f-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d15f-160">Request</span></span>
<span data-ttu-id="2d15f-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d15f-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2d15f-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d15f-162">Response</span></span>
<span data-ttu-id="2d15f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d15f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




