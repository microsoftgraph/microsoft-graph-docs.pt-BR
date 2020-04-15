---
title: Criar deviceCompliancePolicySettingStateSummary
description: Crie um novo objeto deviceCompliancePolicySettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c63c4a0f31c2db63db0d3ef65d3516f1cea3528
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43399931"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="454b5-103">Criar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="454b5-103">Create deviceCompliancePolicySettingStateSummary</span></span>

<span data-ttu-id="454b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="454b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="454b5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="454b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="454b5-106">Crie um novo objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="454b5-106">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="454b5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="454b5-107">Prerequisites</span></span>
<span data-ttu-id="454b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="454b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="454b5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="454b5-110">Permission type</span></span>|<span data-ttu-id="454b5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="454b5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="454b5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="454b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="454b5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="454b5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="454b5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="454b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="454b5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="454b5-115">Not supported.</span></span>|
|<span data-ttu-id="454b5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="454b5-116">Application</span></span>|<span data-ttu-id="454b5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="454b5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="454b5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="454b5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="454b5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="454b5-119">Request headers</span></span>
|<span data-ttu-id="454b5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="454b5-120">Header</span></span>|<span data-ttu-id="454b5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="454b5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="454b5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="454b5-122">Authorization</span></span>|<span data-ttu-id="454b5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="454b5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="454b5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="454b5-124">Accept</span></span>|<span data-ttu-id="454b5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="454b5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="454b5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="454b5-126">Request body</span></span>
<span data-ttu-id="454b5-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="454b5-127">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="454b5-128">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="454b5-128">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="454b5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="454b5-129">Property</span></span>|<span data-ttu-id="454b5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="454b5-130">Type</span></span>|<span data-ttu-id="454b5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="454b5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="454b5-132">id</span><span class="sxs-lookup"><span data-stu-id="454b5-132">id</span></span>|<span data-ttu-id="454b5-133">String</span><span class="sxs-lookup"><span data-stu-id="454b5-133">String</span></span>|<span data-ttu-id="454b5-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="454b5-134">Key of the entity.</span></span>|
|<span data-ttu-id="454b5-135">configuração</span><span class="sxs-lookup"><span data-stu-id="454b5-135">setting</span></span>|<span data-ttu-id="454b5-136">String</span><span class="sxs-lookup"><span data-stu-id="454b5-136">String</span></span>|<span data-ttu-id="454b5-137">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="454b5-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="454b5-138">settingName</span><span class="sxs-lookup"><span data-stu-id="454b5-138">settingName</span></span>|<span data-ttu-id="454b5-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="454b5-139">String</span></span>|<span data-ttu-id="454b5-140">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="454b5-140">Name of the setting.</span></span>|
|<span data-ttu-id="454b5-141">platformType</span><span class="sxs-lookup"><span data-stu-id="454b5-141">platformType</span></span>|[<span data-ttu-id="454b5-142">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="454b5-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="454b5-143">Configuração de plataforma.</span><span class="sxs-lookup"><span data-stu-id="454b5-143">Setting platform.</span></span> <span data-ttu-id="454b5-144">Os valores possíveis são: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="454b5-144">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="454b5-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="454b5-145">unknownDeviceCount</span></span>|<span data-ttu-id="454b5-146">Int32</span><span class="sxs-lookup"><span data-stu-id="454b5-146">Int32</span></span>|<span data-ttu-id="454b5-147">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="454b5-147">Number of unknown devices</span></span>|
|<span data-ttu-id="454b5-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="454b5-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="454b5-149">Int32</span><span class="sxs-lookup"><span data-stu-id="454b5-149">Int32</span></span>|<span data-ttu-id="454b5-150">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="454b5-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="454b5-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="454b5-151">compliantDeviceCount</span></span>|<span data-ttu-id="454b5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="454b5-152">Int32</span></span>|<span data-ttu-id="454b5-153">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="454b5-153">Number of compliant devices</span></span>|
|<span data-ttu-id="454b5-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="454b5-154">remediatedDeviceCount</span></span>|<span data-ttu-id="454b5-155">Int32</span><span class="sxs-lookup"><span data-stu-id="454b5-155">Int32</span></span>|<span data-ttu-id="454b5-156">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="454b5-156">Number of remediated devices</span></span>|
|<span data-ttu-id="454b5-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="454b5-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="454b5-158">Int32</span><span class="sxs-lookup"><span data-stu-id="454b5-158">Int32</span></span>|<span data-ttu-id="454b5-159">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="454b5-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="454b5-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="454b5-160">errorDeviceCount</span></span>|<span data-ttu-id="454b5-161">Int32</span><span class="sxs-lookup"><span data-stu-id="454b5-161">Int32</span></span>|<span data-ttu-id="454b5-162">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="454b5-162">Number of error devices</span></span>|
|<span data-ttu-id="454b5-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="454b5-163">conflictDeviceCount</span></span>|<span data-ttu-id="454b5-164">Int32</span><span class="sxs-lookup"><span data-stu-id="454b5-164">Int32</span></span>|<span data-ttu-id="454b5-165">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="454b5-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="454b5-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="454b5-166">Response</span></span>
<span data-ttu-id="454b5-167">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="454b5-167">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="454b5-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="454b5-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="454b5-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="454b5-169">Request</span></span>
<span data-ttu-id="454b5-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="454b5-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries
Content-type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="454b5-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="454b5-171">Response</span></span>
<span data-ttu-id="454b5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="454b5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```






