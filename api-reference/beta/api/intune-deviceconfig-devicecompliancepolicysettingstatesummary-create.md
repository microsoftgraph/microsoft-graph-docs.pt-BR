---
title: Criar deviceCompliancePolicySettingStateSummary
description: Crie um novo objeto deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 45f8fcc08fb9b3b260ff6446c99948124777f327
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779115"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="61ada-103">Criar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="61ada-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="61ada-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="61ada-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61ada-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61ada-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61ada-106">Crie um novo objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="61ada-106">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61ada-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61ada-107">Prerequisites</span></span>
<span data-ttu-id="61ada-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61ada-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61ada-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61ada-110">Permission type</span></span>|<span data-ttu-id="61ada-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61ada-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61ada-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61ada-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61ada-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61ada-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="61ada-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61ada-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61ada-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61ada-115">Not supported.</span></span>|
|<span data-ttu-id="61ada-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61ada-116">Application</span></span>|<span data-ttu-id="61ada-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61ada-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61ada-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61ada-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="61ada-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61ada-119">Request headers</span></span>
|<span data-ttu-id="61ada-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61ada-120">Header</span></span>|<span data-ttu-id="61ada-121">Valor</span><span class="sxs-lookup"><span data-stu-id="61ada-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61ada-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="61ada-122">Authorization</span></span>|<span data-ttu-id="61ada-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61ada-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61ada-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="61ada-124">Accept</span></span>|<span data-ttu-id="61ada-125">application/json</span><span class="sxs-lookup"><span data-stu-id="61ada-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61ada-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61ada-126">Request body</span></span>
<span data-ttu-id="61ada-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="61ada-127">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="61ada-128">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="61ada-128">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="61ada-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61ada-129">Property</span></span>|<span data-ttu-id="61ada-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="61ada-130">Type</span></span>|<span data-ttu-id="61ada-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="61ada-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61ada-132">id</span><span class="sxs-lookup"><span data-stu-id="61ada-132">id</span></span>|<span data-ttu-id="61ada-133">String</span><span class="sxs-lookup"><span data-stu-id="61ada-133">String</span></span>|<span data-ttu-id="61ada-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="61ada-134">Key of the entity.</span></span>|
|<span data-ttu-id="61ada-135">configuração</span><span class="sxs-lookup"><span data-stu-id="61ada-135">setting</span></span>|<span data-ttu-id="61ada-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61ada-136">String</span></span>|<span data-ttu-id="61ada-137">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="61ada-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="61ada-138">settingName</span><span class="sxs-lookup"><span data-stu-id="61ada-138">settingName</span></span>|<span data-ttu-id="61ada-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61ada-139">String</span></span>|<span data-ttu-id="61ada-140">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="61ada-140">Name of the setting.</span></span>|
|<span data-ttu-id="61ada-141">platformType</span><span class="sxs-lookup"><span data-stu-id="61ada-141">platformType</span></span>|[<span data-ttu-id="61ada-142">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="61ada-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="61ada-143">Configuração de plataforma.</span><span class="sxs-lookup"><span data-stu-id="61ada-143">Setting platform.</span></span> <span data-ttu-id="61ada-144">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="61ada-144">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="61ada-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="61ada-145">unknownDeviceCount</span></span>|<span data-ttu-id="61ada-146">Int32</span><span class="sxs-lookup"><span data-stu-id="61ada-146">Int32</span></span>|<span data-ttu-id="61ada-147">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="61ada-147">Number of unknown devices</span></span>|
|<span data-ttu-id="61ada-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="61ada-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="61ada-149">Int32</span><span class="sxs-lookup"><span data-stu-id="61ada-149">Int32</span></span>|<span data-ttu-id="61ada-150">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="61ada-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="61ada-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="61ada-151">compliantDeviceCount</span></span>|<span data-ttu-id="61ada-152">Int32</span><span class="sxs-lookup"><span data-stu-id="61ada-152">Int32</span></span>|<span data-ttu-id="61ada-153">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="61ada-153">Number of compliant devices</span></span>|
|<span data-ttu-id="61ada-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="61ada-154">remediatedDeviceCount</span></span>|<span data-ttu-id="61ada-155">Int32</span><span class="sxs-lookup"><span data-stu-id="61ada-155">Int32</span></span>|<span data-ttu-id="61ada-156">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="61ada-156">Number of remediated devices</span></span>|
|<span data-ttu-id="61ada-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="61ada-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="61ada-158">Int32</span><span class="sxs-lookup"><span data-stu-id="61ada-158">Int32</span></span>|<span data-ttu-id="61ada-159">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="61ada-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="61ada-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="61ada-160">errorDeviceCount</span></span>|<span data-ttu-id="61ada-161">Int32</span><span class="sxs-lookup"><span data-stu-id="61ada-161">Int32</span></span>|<span data-ttu-id="61ada-162">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="61ada-162">Number of error devices</span></span>|
|<span data-ttu-id="61ada-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="61ada-163">conflictDeviceCount</span></span>|<span data-ttu-id="61ada-164">Int32</span><span class="sxs-lookup"><span data-stu-id="61ada-164">Int32</span></span>|<span data-ttu-id="61ada-165">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="61ada-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="61ada-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="61ada-166">Response</span></span>
<span data-ttu-id="61ada-167">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61ada-167">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61ada-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61ada-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="61ada-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61ada-169">Request</span></span>
<span data-ttu-id="61ada-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61ada-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="61ada-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="61ada-171">Response</span></span>
<span data-ttu-id="61ada-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61ada-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





