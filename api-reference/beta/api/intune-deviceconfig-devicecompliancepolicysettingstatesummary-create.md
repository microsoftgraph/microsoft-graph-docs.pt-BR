---
title: Criar deviceCompliancePolicySettingStateSummary
description: Crie um novo objeto deviceCompliancePolicySettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c1c962b2827fbf7ea8d784fc191f9320bb8eceda
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49292181"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="2e95a-103">Criar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="2e95a-103">Create deviceCompliancePolicySettingStateSummary</span></span>

<span data-ttu-id="2e95a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e95a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e95a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2e95a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e95a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2e95a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e95a-107">Crie um novo objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="2e95a-107">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e95a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2e95a-108">Prerequisites</span></span>
<span data-ttu-id="2e95a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e95a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e95a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e95a-111">Permission type</span></span>|<span data-ttu-id="2e95a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2e95a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e95a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e95a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e95a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e95a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2e95a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e95a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e95a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e95a-116">Not supported.</span></span>|
|<span data-ttu-id="2e95a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e95a-117">Application</span></span>|<span data-ttu-id="2e95a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e95a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e95a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e95a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="2e95a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e95a-120">Request headers</span></span>
|<span data-ttu-id="2e95a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2e95a-121">Header</span></span>|<span data-ttu-id="2e95a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2e95a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e95a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e95a-123">Authorization</span></span>|<span data-ttu-id="2e95a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e95a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e95a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2e95a-125">Accept</span></span>|<span data-ttu-id="2e95a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2e95a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e95a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e95a-127">Request body</span></span>
<span data-ttu-id="2e95a-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="2e95a-128">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="2e95a-129">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="2e95a-129">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="2e95a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e95a-130">Property</span></span>|<span data-ttu-id="2e95a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e95a-131">Type</span></span>|<span data-ttu-id="2e95a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e95a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e95a-133">id</span><span class="sxs-lookup"><span data-stu-id="2e95a-133">id</span></span>|<span data-ttu-id="2e95a-134">String</span><span class="sxs-lookup"><span data-stu-id="2e95a-134">String</span></span>|<span data-ttu-id="2e95a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2e95a-135">Key of the entity.</span></span>|
|<span data-ttu-id="2e95a-136">configuração</span><span class="sxs-lookup"><span data-stu-id="2e95a-136">setting</span></span>|<span data-ttu-id="2e95a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e95a-137">String</span></span>|<span data-ttu-id="2e95a-138">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="2e95a-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="2e95a-139">settingName</span><span class="sxs-lookup"><span data-stu-id="2e95a-139">settingName</span></span>|<span data-ttu-id="2e95a-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e95a-140">String</span></span>|<span data-ttu-id="2e95a-141">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="2e95a-141">Name of the setting.</span></span>|
|<span data-ttu-id="2e95a-142">platformType</span><span class="sxs-lookup"><span data-stu-id="2e95a-142">platformType</span></span>|[<span data-ttu-id="2e95a-143">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="2e95a-143">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="2e95a-144">Configuração de plataforma.</span><span class="sxs-lookup"><span data-stu-id="2e95a-144">Setting platform.</span></span> <span data-ttu-id="2e95a-145">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="2e95a-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="2e95a-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2e95a-146">unknownDeviceCount</span></span>|<span data-ttu-id="2e95a-147">Int32</span><span class="sxs-lookup"><span data-stu-id="2e95a-147">Int32</span></span>|<span data-ttu-id="2e95a-148">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="2e95a-148">Number of unknown devices</span></span>|
|<span data-ttu-id="2e95a-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2e95a-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="2e95a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="2e95a-150">Int32</span></span>|<span data-ttu-id="2e95a-151">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="2e95a-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="2e95a-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2e95a-152">compliantDeviceCount</span></span>|<span data-ttu-id="2e95a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="2e95a-153">Int32</span></span>|<span data-ttu-id="2e95a-154">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="2e95a-154">Number of compliant devices</span></span>|
|<span data-ttu-id="2e95a-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2e95a-155">remediatedDeviceCount</span></span>|<span data-ttu-id="2e95a-156">Int32</span><span class="sxs-lookup"><span data-stu-id="2e95a-156">Int32</span></span>|<span data-ttu-id="2e95a-157">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="2e95a-157">Number of remediated devices</span></span>|
|<span data-ttu-id="2e95a-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2e95a-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="2e95a-159">Int32</span><span class="sxs-lookup"><span data-stu-id="2e95a-159">Int32</span></span>|<span data-ttu-id="2e95a-160">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="2e95a-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="2e95a-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2e95a-161">errorDeviceCount</span></span>|<span data-ttu-id="2e95a-162">Int32</span><span class="sxs-lookup"><span data-stu-id="2e95a-162">Int32</span></span>|<span data-ttu-id="2e95a-163">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="2e95a-163">Number of error devices</span></span>|
|<span data-ttu-id="2e95a-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2e95a-164">conflictDeviceCount</span></span>|<span data-ttu-id="2e95a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2e95a-165">Int32</span></span>|<span data-ttu-id="2e95a-166">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="2e95a-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="2e95a-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e95a-167">Response</span></span>
<span data-ttu-id="2e95a-168">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e95a-168">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e95a-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e95a-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e95a-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e95a-170">Request</span></span>
<span data-ttu-id="2e95a-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e95a-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries
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

### <a name="response"></a><span data-ttu-id="2e95a-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e95a-172">Response</span></span>
<span data-ttu-id="2e95a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e95a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




