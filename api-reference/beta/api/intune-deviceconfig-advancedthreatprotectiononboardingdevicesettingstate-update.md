---
title: Atualizar advancedThreatProtectionOnboardingDeviceSettingState
description: Atualize as propriedades de um objeto advancedThreatProtectionOnboardingDeviceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1db888112e3cea22cdf154662618474694a60b6e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126861"
---
# <a name="update-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="e6f3e-103">Atualizar advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="e6f3e-103">Update advancedThreatProtectionOnboardingDeviceSettingState</span></span>

<span data-ttu-id="e6f3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6f3e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6f3e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e6f3e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6f3e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6f3e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6f3e-107">Atualize as propriedades de [um objeto advancedThreatProtectionOnboardingDeviceSettingState.](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)</span><span class="sxs-lookup"><span data-stu-id="e6f3e-107">Update the properties of a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6f3e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e6f3e-108">Prerequisites</span></span>
<span data-ttu-id="e6f3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6f3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6f3e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6f3e-111">Permission type</span></span>|<span data-ttu-id="e6f3e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6f3e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6f3e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6f3e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6f3e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6f3e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e6f3e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6f3e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6f3e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6f3e-116">Not supported.</span></span>|
|<span data-ttu-id="e6f3e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6f3e-117">Application</span></span>|<span data-ttu-id="e6f3e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6f3e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6f3e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6f3e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="e6f3e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6f3e-120">Request headers</span></span>
|<span data-ttu-id="e6f3e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e6f3e-121">Header</span></span>|<span data-ttu-id="e6f3e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e6f3e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6f3e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6f3e-123">Authorization</span></span>|<span data-ttu-id="e6f3e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6f3e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6f3e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e6f3e-125">Accept</span></span>|<span data-ttu-id="e6f3e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6f3e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6f3e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6f3e-127">Request body</span></span>
<span data-ttu-id="e6f3e-128">No corpo da solicitação, fornece uma representação JSON para [o objeto advancedThreatProtectionOnboardingDeviceSettingState.](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)</span><span class="sxs-lookup"><span data-stu-id="e6f3e-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

<span data-ttu-id="e6f3e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="e6f3e-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).</span></span>

|<span data-ttu-id="e6f3e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6f3e-130">Property</span></span>|<span data-ttu-id="e6f3e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6f3e-131">Type</span></span>|<span data-ttu-id="e6f3e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6f3e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6f3e-133">id</span><span class="sxs-lookup"><span data-stu-id="e6f3e-133">id</span></span>|<span data-ttu-id="e6f3e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6f3e-134">String</span></span>|<span data-ttu-id="e6f3e-135">Chave da entidade</span><span class="sxs-lookup"><span data-stu-id="e6f3e-135">Key of the entity</span></span>|
|<span data-ttu-id="e6f3e-136">platformType</span><span class="sxs-lookup"><span data-stu-id="e6f3e-136">platformType</span></span>|[<span data-ttu-id="e6f3e-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="e6f3e-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="e6f3e-138">Tipo de plataforma de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e6f3e-138">Device platform type.</span></span> <span data-ttu-id="e6f3e-139">Os valores possíveis são: `desktop` , , , , , , , , `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` , `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` `unknown` .</span><span class="sxs-lookup"><span data-stu-id="e6f3e-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `cloudPC`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="e6f3e-140">configuração</span><span class="sxs-lookup"><span data-stu-id="e6f3e-140">setting</span></span>|<span data-ttu-id="e6f3e-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6f3e-141">String</span></span>|<span data-ttu-id="e6f3e-142">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="e6f3e-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="e6f3e-143">settingName</span><span class="sxs-lookup"><span data-stu-id="e6f3e-143">settingName</span></span>|<span data-ttu-id="e6f3e-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6f3e-144">String</span></span>|<span data-ttu-id="e6f3e-145">O nome da configuração sendo relatada</span><span class="sxs-lookup"><span data-stu-id="e6f3e-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="e6f3e-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="e6f3e-146">deviceId</span></span>|<span data-ttu-id="e6f3e-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6f3e-147">String</span></span>|<span data-ttu-id="e6f3e-148">A ID do dispositivo sendo relatada</span><span class="sxs-lookup"><span data-stu-id="e6f3e-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="e6f3e-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="e6f3e-149">deviceName</span></span>|<span data-ttu-id="e6f3e-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6f3e-150">String</span></span>|<span data-ttu-id="e6f3e-151">O nome do dispositivo sendo relatado</span><span class="sxs-lookup"><span data-stu-id="e6f3e-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="e6f3e-152">userId</span><span class="sxs-lookup"><span data-stu-id="e6f3e-152">userId</span></span>|<span data-ttu-id="e6f3e-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6f3e-153">String</span></span>|<span data-ttu-id="e6f3e-154">A ID do usuário sendo relatada</span><span class="sxs-lookup"><span data-stu-id="e6f3e-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="e6f3e-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="e6f3e-155">userEmail</span></span>|<span data-ttu-id="e6f3e-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6f3e-156">String</span></span>|<span data-ttu-id="e6f3e-157">O endereço de email do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="e6f3e-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="e6f3e-158">userName</span><span class="sxs-lookup"><span data-stu-id="e6f3e-158">userName</span></span>|<span data-ttu-id="e6f3e-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6f3e-159">String</span></span>|<span data-ttu-id="e6f3e-160">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="e6f3e-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="e6f3e-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e6f3e-161">userPrincipalName</span></span>|<span data-ttu-id="e6f3e-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6f3e-162">String</span></span>|<span data-ttu-id="e6f3e-163">O PrincipalName do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="e6f3e-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="e6f3e-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="e6f3e-164">deviceModel</span></span>|<span data-ttu-id="e6f3e-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6f3e-165">String</span></span>|<span data-ttu-id="e6f3e-166">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="e6f3e-166">The device model that is being reported</span></span>|
|<span data-ttu-id="e6f3e-167">state</span><span class="sxs-lookup"><span data-stu-id="e6f3e-167">state</span></span>|[<span data-ttu-id="e6f3e-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="e6f3e-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="e6f3e-169">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="e6f3e-169">The compliance state of the setting.</span></span> <span data-ttu-id="e6f3e-170">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="e6f3e-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="e6f3e-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e6f3e-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="e6f3e-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6f3e-172">DateTimeOffset</span></span>|<span data-ttu-id="e6f3e-173">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="e6f3e-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="e6f3e-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6f3e-174">Response</span></span>
<span data-ttu-id="e6f3e-175">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6f3e-175">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6f3e-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6f3e-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6f3e-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6f3e-177">Request</span></span>
<span data-ttu-id="e6f3e-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6f3e-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
Content-type: application/json
Content-length: 573

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
  "platformType": "windowsRT",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "userId": "User Id value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "deviceModel": "Device Model value",
  "state": "notApplicable",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
}
```

### <a name="response"></a><span data-ttu-id="e6f3e-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6f3e-179">Response</span></span>
<span data-ttu-id="e6f3e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6f3e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 622

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
  "id": "63593fc6-3fc6-6359-c63f-5963c63f5963",
  "platformType": "windowsRT",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "userId": "User Id value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "deviceModel": "Device Model value",
  "state": "notApplicable",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
}
```




