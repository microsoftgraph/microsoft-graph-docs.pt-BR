---
title: Atualizar deviceCompliancePolicySettingStateSummary
description: Atualizar as propriedades de um objeto deviceCompliancePolicySettingStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2a69889f8f5f4a814a38424e5ffab62609262385
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36340139"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="0b91d-103">Atualizar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="0b91d-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="0b91d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0b91d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b91d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b91d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b91d-106">Atualizar as propriedades de um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="0b91d-106">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b91d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0b91d-107">Prerequisites</span></span>
<span data-ttu-id="0b91d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b91d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b91d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b91d-110">Permission type</span></span>|<span data-ttu-id="0b91d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0b91d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b91d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b91d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b91d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b91d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b91d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b91d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b91d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b91d-115">Not supported.</span></span>|
|<span data-ttu-id="0b91d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b91d-116">Application</span></span>|<span data-ttu-id="0b91d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b91d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b91d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b91d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="0b91d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b91d-119">Request headers</span></span>
|<span data-ttu-id="0b91d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b91d-120">Header</span></span>|<span data-ttu-id="0b91d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0b91d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b91d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b91d-122">Authorization</span></span>|<span data-ttu-id="0b91d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b91d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b91d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0b91d-124">Accept</span></span>|<span data-ttu-id="0b91d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0b91d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b91d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b91d-126">Request body</span></span>
<span data-ttu-id="0b91d-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="0b91d-127">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="0b91d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="0b91d-128">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="0b91d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b91d-129">Property</span></span>|<span data-ttu-id="0b91d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b91d-130">Type</span></span>|<span data-ttu-id="0b91d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b91d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b91d-132">id</span><span class="sxs-lookup"><span data-stu-id="0b91d-132">id</span></span>|<span data-ttu-id="0b91d-133">String</span><span class="sxs-lookup"><span data-stu-id="0b91d-133">String</span></span>|<span data-ttu-id="0b91d-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0b91d-134">Key of the entity.</span></span>|
|<span data-ttu-id="0b91d-135">configuração</span><span class="sxs-lookup"><span data-stu-id="0b91d-135">setting</span></span>|<span data-ttu-id="0b91d-136">String</span><span class="sxs-lookup"><span data-stu-id="0b91d-136">String</span></span>|<span data-ttu-id="0b91d-137">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="0b91d-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="0b91d-138">settingName</span><span class="sxs-lookup"><span data-stu-id="0b91d-138">settingName</span></span>|<span data-ttu-id="0b91d-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b91d-139">String</span></span>|<span data-ttu-id="0b91d-140">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="0b91d-140">Name of the setting.</span></span>|
|<span data-ttu-id="0b91d-141">platformType</span><span class="sxs-lookup"><span data-stu-id="0b91d-141">platformType</span></span>|[<span data-ttu-id="0b91d-142">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="0b91d-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="0b91d-143">Configuração de plataforma.</span><span class="sxs-lookup"><span data-stu-id="0b91d-143">Setting platform.</span></span> <span data-ttu-id="0b91d-144">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="0b91d-144">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="0b91d-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b91d-145">unknownDeviceCount</span></span>|<span data-ttu-id="0b91d-146">Int32</span><span class="sxs-lookup"><span data-stu-id="0b91d-146">Int32</span></span>|<span data-ttu-id="0b91d-147">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="0b91d-147">Number of unknown devices</span></span>|
|<span data-ttu-id="0b91d-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b91d-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="0b91d-149">Int32</span><span class="sxs-lookup"><span data-stu-id="0b91d-149">Int32</span></span>|<span data-ttu-id="0b91d-150">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="0b91d-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="0b91d-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b91d-151">compliantDeviceCount</span></span>|<span data-ttu-id="0b91d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0b91d-152">Int32</span></span>|<span data-ttu-id="0b91d-153">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="0b91d-153">Number of compliant devices</span></span>|
|<span data-ttu-id="0b91d-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b91d-154">remediatedDeviceCount</span></span>|<span data-ttu-id="0b91d-155">Int32</span><span class="sxs-lookup"><span data-stu-id="0b91d-155">Int32</span></span>|<span data-ttu-id="0b91d-156">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="0b91d-156">Number of remediated devices</span></span>|
|<span data-ttu-id="0b91d-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b91d-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="0b91d-158">Int32</span><span class="sxs-lookup"><span data-stu-id="0b91d-158">Int32</span></span>|<span data-ttu-id="0b91d-159">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="0b91d-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="0b91d-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b91d-160">errorDeviceCount</span></span>|<span data-ttu-id="0b91d-161">Int32</span><span class="sxs-lookup"><span data-stu-id="0b91d-161">Int32</span></span>|<span data-ttu-id="0b91d-162">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="0b91d-162">Number of error devices</span></span>|
|<span data-ttu-id="0b91d-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b91d-163">conflictDeviceCount</span></span>|<span data-ttu-id="0b91d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0b91d-164">Int32</span></span>|<span data-ttu-id="0b91d-165">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="0b91d-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="0b91d-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b91d-166">Response</span></span>
<span data-ttu-id="0b91d-167">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b91d-167">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b91d-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b91d-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b91d-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b91d-169">Request</span></span>
<span data-ttu-id="0b91d-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b91d-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
Content-type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "androidForWork",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="0b91d-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b91d-171">Response</span></span>
<span data-ttu-id="0b91d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b91d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 451

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "androidForWork",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```






