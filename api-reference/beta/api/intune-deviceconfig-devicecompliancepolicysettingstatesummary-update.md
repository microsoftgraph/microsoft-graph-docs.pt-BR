---
title: Atualizar deviceCompliancePolicySettingStateSummary
description: Atualizar as propriedades de um objeto deviceCompliancePolicySettingStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0274588c0feb913838d6ab9033e306bfe9072b0f
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534166"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="c4493-103">Atualizar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="c4493-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="c4493-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4493-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4493-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4493-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4493-106">Atualizar as propriedades de um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c4493-106">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4493-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4493-107">Prerequisites</span></span>
<span data-ttu-id="c4493-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4493-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4493-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4493-110">Permission type</span></span>|<span data-ttu-id="c4493-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c4493-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4493-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4493-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c4493-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4493-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c4493-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4493-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4493-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4493-115">Not supported.</span></span>|
|<span data-ttu-id="c4493-116">Application</span><span class="sxs-lookup"><span data-stu-id="c4493-116">Application</span></span>|<span data-ttu-id="c4493-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4493-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4493-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4493-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="c4493-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4493-119">Request headers</span></span>
|<span data-ttu-id="c4493-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4493-120">Header</span></span>|<span data-ttu-id="c4493-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c4493-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4493-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4493-122">Authorization</span></span>|<span data-ttu-id="c4493-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4493-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4493-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4493-124">Accept</span></span>|<span data-ttu-id="c4493-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c4493-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4493-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4493-126">Request body</span></span>
<span data-ttu-id="c4493-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c4493-127">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="c4493-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c4493-128">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="c4493-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4493-129">Property</span></span>|<span data-ttu-id="c4493-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4493-130">Type</span></span>|<span data-ttu-id="c4493-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4493-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4493-132">id</span><span class="sxs-lookup"><span data-stu-id="c4493-132">id</span></span>|<span data-ttu-id="c4493-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4493-133">String</span></span>|<span data-ttu-id="c4493-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c4493-134">Key of the entity.</span></span>|
|<span data-ttu-id="c4493-135">configuração</span><span class="sxs-lookup"><span data-stu-id="c4493-135">setting</span></span>|<span data-ttu-id="c4493-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4493-136">String</span></span>|<span data-ttu-id="c4493-137">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="c4493-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="c4493-138">settingName</span><span class="sxs-lookup"><span data-stu-id="c4493-138">settingName</span></span>|<span data-ttu-id="c4493-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4493-139">String</span></span>|<span data-ttu-id="c4493-140">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="c4493-140">Name of the setting.</span></span>|
|<span data-ttu-id="c4493-141">platformType</span><span class="sxs-lookup"><span data-stu-id="c4493-141">platformType</span></span>|[<span data-ttu-id="c4493-142">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="c4493-142">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="c4493-143">Configuração de plataforma.</span><span class="sxs-lookup"><span data-stu-id="c4493-143">Setting platform.</span></span> <span data-ttu-id="c4493-144">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="c4493-144">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="c4493-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c4493-145">unknownDeviceCount</span></span>|<span data-ttu-id="c4493-146">Int32</span><span class="sxs-lookup"><span data-stu-id="c4493-146">Int32</span></span>|<span data-ttu-id="c4493-147">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="c4493-147">Number of unknown devices</span></span>|
|<span data-ttu-id="c4493-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c4493-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="c4493-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c4493-149">Int32</span></span>|<span data-ttu-id="c4493-150">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="c4493-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="c4493-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c4493-151">compliantDeviceCount</span></span>|<span data-ttu-id="c4493-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c4493-152">Int32</span></span>|<span data-ttu-id="c4493-153">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="c4493-153">Number of compliant devices</span></span>|
|<span data-ttu-id="c4493-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c4493-154">remediatedDeviceCount</span></span>|<span data-ttu-id="c4493-155">Int32</span><span class="sxs-lookup"><span data-stu-id="c4493-155">Int32</span></span>|<span data-ttu-id="c4493-156">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="c4493-156">Number of remediated devices</span></span>|
|<span data-ttu-id="c4493-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c4493-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="c4493-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c4493-158">Int32</span></span>|<span data-ttu-id="c4493-159">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="c4493-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="c4493-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c4493-160">errorDeviceCount</span></span>|<span data-ttu-id="c4493-161">Int32</span><span class="sxs-lookup"><span data-stu-id="c4493-161">Int32</span></span>|<span data-ttu-id="c4493-162">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="c4493-162">Number of error devices</span></span>|
|<span data-ttu-id="c4493-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c4493-163">conflictDeviceCount</span></span>|<span data-ttu-id="c4493-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c4493-164">Int32</span></span>|<span data-ttu-id="c4493-165">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="c4493-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="c4493-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4493-166">Response</span></span>
<span data-ttu-id="c4493-167">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4493-167">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4493-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4493-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4493-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4493-169">Request</span></span>
<span data-ttu-id="c4493-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4493-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c4493-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4493-171">Response</span></span>
<span data-ttu-id="c4493-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4493-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






