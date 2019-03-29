---
title: Criar advancedThreatProtectionOnboardingDeviceSettingState
description: Criar um novo objeto advancedThreatProtectionOnboardingDeviceSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d877edcdc82cee35c7fc75c556ca5ac0035221ad
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980660"
---
# <a name="create-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="7b01a-103">Criar advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="7b01a-103">Create advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="7b01a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7b01a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b01a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7b01a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b01a-106">Criar um novo objeto [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="7b01a-106">Create a new [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b01a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7b01a-107">Prerequisites</span></span>
<span data-ttu-id="7b01a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b01a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b01a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b01a-110">Permission type</span></span>|<span data-ttu-id="7b01a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7b01a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b01a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b01a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7b01a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b01a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b01a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b01a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b01a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b01a-115">Not supported.</span></span>|
|<span data-ttu-id="7b01a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b01a-116">Application</span></span>|<span data-ttu-id="7b01a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b01a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b01a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b01a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="7b01a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b01a-119">Request headers</span></span>
|<span data-ttu-id="7b01a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7b01a-120">Header</span></span>|<span data-ttu-id="7b01a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7b01a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b01a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b01a-122">Authorization</span></span>|<span data-ttu-id="7b01a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b01a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b01a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7b01a-124">Accept</span></span>|<span data-ttu-id="7b01a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7b01a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b01a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b01a-126">Request body</span></span>
<span data-ttu-id="7b01a-127">No corpo da solicitação, forneça uma representação JSON do objeto advancedThreatProtectionOnboardingDeviceSettingState.</span><span class="sxs-lookup"><span data-stu-id="7b01a-127">In the request body, supply a JSON representation for the advancedThreatProtectionOnboardingDeviceSettingState object.</span></span>

<span data-ttu-id="7b01a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar advancedThreatProtectionOnboardingDeviceSettingState.</span><span class="sxs-lookup"><span data-stu-id="7b01a-128">The following table shows the properties that are required when you create the advancedThreatProtectionOnboardingDeviceSettingState.</span></span>

|<span data-ttu-id="7b01a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b01a-129">Property</span></span>|<span data-ttu-id="7b01a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b01a-130">Type</span></span>|<span data-ttu-id="7b01a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b01a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b01a-132">id</span><span class="sxs-lookup"><span data-stu-id="7b01a-132">id</span></span>|<span data-ttu-id="7b01a-133">String</span><span class="sxs-lookup"><span data-stu-id="7b01a-133">String</span></span>|<span data-ttu-id="7b01a-134">Chave da entidade</span><span class="sxs-lookup"><span data-stu-id="7b01a-134">Key of the entity</span></span>|
|<span data-ttu-id="7b01a-135">platformType</span><span class="sxs-lookup"><span data-stu-id="7b01a-135">platformType</span></span>|[<span data-ttu-id="7b01a-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="7b01a-136">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="7b01a-137">Tipo de plataforma de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7b01a-137">Device platform type.</span></span> <span data-ttu-id="7b01a-138">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` ,,,,,,,, , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="7b01a-138">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="7b01a-139">configuração</span><span class="sxs-lookup"><span data-stu-id="7b01a-139">setting</span></span>|<span data-ttu-id="7b01a-140">String</span><span class="sxs-lookup"><span data-stu-id="7b01a-140">String</span></span>|<span data-ttu-id="7b01a-141">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="7b01a-141">The setting class name and property name.</span></span>|
|<span data-ttu-id="7b01a-142">settingName</span><span class="sxs-lookup"><span data-stu-id="7b01a-142">settingName</span></span>|<span data-ttu-id="7b01a-143">String</span><span class="sxs-lookup"><span data-stu-id="7b01a-143">String</span></span>|<span data-ttu-id="7b01a-144">O nome da configuração sendo relatada</span><span class="sxs-lookup"><span data-stu-id="7b01a-144">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="7b01a-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="7b01a-145">deviceId</span></span>|<span data-ttu-id="7b01a-146">String</span><span class="sxs-lookup"><span data-stu-id="7b01a-146">String</span></span>|<span data-ttu-id="7b01a-147">A ID do dispositivo sendo relatada</span><span class="sxs-lookup"><span data-stu-id="7b01a-147">The Device Id that is being reported</span></span>|
|<span data-ttu-id="7b01a-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="7b01a-148">deviceName</span></span>|<span data-ttu-id="7b01a-149">String</span><span class="sxs-lookup"><span data-stu-id="7b01a-149">String</span></span>|<span data-ttu-id="7b01a-150">O nome do dispositivo sendo relatado</span><span class="sxs-lookup"><span data-stu-id="7b01a-150">The Device Name that is being reported</span></span>|
|<span data-ttu-id="7b01a-151">userId</span><span class="sxs-lookup"><span data-stu-id="7b01a-151">userId</span></span>|<span data-ttu-id="7b01a-152">String</span><span class="sxs-lookup"><span data-stu-id="7b01a-152">String</span></span>|<span data-ttu-id="7b01a-153">A ID do usuário sendo relatada</span><span class="sxs-lookup"><span data-stu-id="7b01a-153">The user Id that is being reported</span></span>|
|<span data-ttu-id="7b01a-154">userEmail</span><span class="sxs-lookup"><span data-stu-id="7b01a-154">userEmail</span></span>|<span data-ttu-id="7b01a-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7b01a-155">String</span></span>|<span data-ttu-id="7b01a-156">O endereço de email do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="7b01a-156">The User email address that is being reported</span></span>|
|<span data-ttu-id="7b01a-157">userName</span><span class="sxs-lookup"><span data-stu-id="7b01a-157">userName</span></span>|<span data-ttu-id="7b01a-158">String</span><span class="sxs-lookup"><span data-stu-id="7b01a-158">String</span></span>|<span data-ttu-id="7b01a-159">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="7b01a-159">The User Name that is being reported</span></span>|
|<span data-ttu-id="7b01a-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7b01a-160">userPrincipalName</span></span>|<span data-ttu-id="7b01a-161">String</span><span class="sxs-lookup"><span data-stu-id="7b01a-161">String</span></span>|<span data-ttu-id="7b01a-162">O PrincipalName do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="7b01a-162">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="7b01a-163">deviceModel</span><span class="sxs-lookup"><span data-stu-id="7b01a-163">deviceModel</span></span>|<span data-ttu-id="7b01a-164">String</span><span class="sxs-lookup"><span data-stu-id="7b01a-164">String</span></span>|<span data-ttu-id="7b01a-165">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="7b01a-165">The device model that is being reported</span></span>|
|<span data-ttu-id="7b01a-166">state</span><span class="sxs-lookup"><span data-stu-id="7b01a-166">state</span></span>|[<span data-ttu-id="7b01a-167">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="7b01a-167">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="7b01a-168">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="7b01a-168">The compliance state of the setting.</span></span> <span data-ttu-id="7b01a-169">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="7b01a-169">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="7b01a-170">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7b01a-170">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="7b01a-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b01a-171">DateTimeOffset</span></span>|<span data-ttu-id="7b01a-172">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="7b01a-172">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="7b01a-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b01a-173">Response</span></span>
<span data-ttu-id="7b01a-174">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b01a-174">If successful, this method returns a `201 Created` response code and a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b01a-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b01a-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b01a-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b01a-176">Request</span></span>
<span data-ttu-id="7b01a-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b01a-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
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

### <a name="response"></a><span data-ttu-id="7b01a-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b01a-178">Response</span></span>
<span data-ttu-id="7b01a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7b01a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




