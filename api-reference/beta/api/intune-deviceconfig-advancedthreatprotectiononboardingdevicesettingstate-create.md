---
title: Criar advancedThreatProtectionOnboardingDeviceSettingState
description: Criar um novo objeto advancedThreatProtectionOnboardingDeviceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 576ac7eaf5e44cdd3539c1d4a281c3612880e733
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793147"
---
# <a name="create-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="6f930-103">Criar advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="6f930-103">Create advancedThreatProtectionOnboardingDeviceSettingState</span></span>

<span data-ttu-id="6f930-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f930-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f930-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6f930-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f930-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6f930-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f930-107">Criar um novo objeto [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="6f930-107">Create a new [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f930-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6f930-108">Prerequisites</span></span>
<span data-ttu-id="6f930-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6f930-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6f930-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f930-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f930-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f930-111">Permission type</span></span>|<span data-ttu-id="6f930-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6f930-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f930-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f930-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f930-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f930-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f930-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f930-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f930-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f930-116">Not supported.</span></span>|
|<span data-ttu-id="6f930-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f930-117">Application</span></span>|<span data-ttu-id="6f930-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f930-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f930-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f930-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="6f930-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f930-120">Request headers</span></span>
|<span data-ttu-id="6f930-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f930-121">Header</span></span>|<span data-ttu-id="6f930-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6f930-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f930-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f930-123">Authorization</span></span>|<span data-ttu-id="6f930-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f930-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f930-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6f930-125">Accept</span></span>|<span data-ttu-id="6f930-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f930-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f930-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f930-127">Request body</span></span>
<span data-ttu-id="6f930-128">No corpo da solicitação, forneça uma representação JSON do objeto advancedThreatProtectionOnboardingDeviceSettingState.</span><span class="sxs-lookup"><span data-stu-id="6f930-128">In the request body, supply a JSON representation for the advancedThreatProtectionOnboardingDeviceSettingState object.</span></span>

<span data-ttu-id="6f930-129">A tabela a seguir mostra as propriedades que são necessárias ao criar advancedThreatProtectionOnboardingDeviceSettingState.</span><span class="sxs-lookup"><span data-stu-id="6f930-129">The following table shows the properties that are required when you create the advancedThreatProtectionOnboardingDeviceSettingState.</span></span>

|<span data-ttu-id="6f930-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f930-130">Property</span></span>|<span data-ttu-id="6f930-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f930-131">Type</span></span>|<span data-ttu-id="6f930-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f930-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f930-133">id</span><span class="sxs-lookup"><span data-stu-id="6f930-133">id</span></span>|<span data-ttu-id="6f930-134">String</span><span class="sxs-lookup"><span data-stu-id="6f930-134">String</span></span>|<span data-ttu-id="6f930-135">Chave da entidade</span><span class="sxs-lookup"><span data-stu-id="6f930-135">Key of the entity</span></span>|
|<span data-ttu-id="6f930-136">platformType</span><span class="sxs-lookup"><span data-stu-id="6f930-136">platformType</span></span>|[<span data-ttu-id="6f930-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="6f930-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="6f930-138">Tipo de plataforma de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6f930-138">Device platform type.</span></span> <span data-ttu-id="6f930-139">Os valores possíveis são:,,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` , `macMDM` , `holoLens` , `surfaceHub` , `androidForWork` , `androidEnterprise` , `windows10x` `androidnGMS` `blackberry` `palm` `unknown` ,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="6f930-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="6f930-140">configuração</span><span class="sxs-lookup"><span data-stu-id="6f930-140">setting</span></span>|<span data-ttu-id="6f930-141">String</span><span class="sxs-lookup"><span data-stu-id="6f930-141">String</span></span>|<span data-ttu-id="6f930-142">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="6f930-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="6f930-143">settingName</span><span class="sxs-lookup"><span data-stu-id="6f930-143">settingName</span></span>|<span data-ttu-id="6f930-144">String</span><span class="sxs-lookup"><span data-stu-id="6f930-144">String</span></span>|<span data-ttu-id="6f930-145">O nome da configuração sendo relatada</span><span class="sxs-lookup"><span data-stu-id="6f930-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="6f930-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="6f930-146">deviceId</span></span>|<span data-ttu-id="6f930-147">String</span><span class="sxs-lookup"><span data-stu-id="6f930-147">String</span></span>|<span data-ttu-id="6f930-148">A ID do dispositivo sendo relatada</span><span class="sxs-lookup"><span data-stu-id="6f930-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="6f930-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="6f930-149">deviceName</span></span>|<span data-ttu-id="6f930-150">String</span><span class="sxs-lookup"><span data-stu-id="6f930-150">String</span></span>|<span data-ttu-id="6f930-151">O nome do dispositivo sendo relatado</span><span class="sxs-lookup"><span data-stu-id="6f930-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="6f930-152">userId</span><span class="sxs-lookup"><span data-stu-id="6f930-152">userId</span></span>|<span data-ttu-id="6f930-153">String</span><span class="sxs-lookup"><span data-stu-id="6f930-153">String</span></span>|<span data-ttu-id="6f930-154">A ID do usuário sendo relatada</span><span class="sxs-lookup"><span data-stu-id="6f930-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="6f930-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="6f930-155">userEmail</span></span>|<span data-ttu-id="6f930-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f930-156">String</span></span>|<span data-ttu-id="6f930-157">O endereço de email do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="6f930-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="6f930-158">userName</span><span class="sxs-lookup"><span data-stu-id="6f930-158">userName</span></span>|<span data-ttu-id="6f930-159">String</span><span class="sxs-lookup"><span data-stu-id="6f930-159">String</span></span>|<span data-ttu-id="6f930-160">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="6f930-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="6f930-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6f930-161">userPrincipalName</span></span>|<span data-ttu-id="6f930-162">String</span><span class="sxs-lookup"><span data-stu-id="6f930-162">String</span></span>|<span data-ttu-id="6f930-163">O PrincipalName do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="6f930-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="6f930-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="6f930-164">deviceModel</span></span>|<span data-ttu-id="6f930-165">String</span><span class="sxs-lookup"><span data-stu-id="6f930-165">String</span></span>|<span data-ttu-id="6f930-166">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="6f930-166">The device model that is being reported</span></span>|
|<span data-ttu-id="6f930-167">state</span><span class="sxs-lookup"><span data-stu-id="6f930-167">state</span></span>|[<span data-ttu-id="6f930-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="6f930-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="6f930-169">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="6f930-169">The compliance state of the setting.</span></span> <span data-ttu-id="6f930-170">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="6f930-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="6f930-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6f930-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="6f930-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f930-172">DateTimeOffset</span></span>|<span data-ttu-id="6f930-173">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="6f930-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="6f930-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f930-174">Response</span></span>
<span data-ttu-id="6f930-175">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f930-175">If successful, this method returns a `201 Created` response code and a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f930-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f930-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f930-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f930-177">Request</span></span>
<span data-ttu-id="6f930-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f930-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6f930-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f930-179">Response</span></span>
<span data-ttu-id="6f930-180">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="6f930-180">Here is an example of the response.</span></span> <span data-ttu-id="6f930-181">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="6f930-181">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6f930-182">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="6f930-182">All of the properties will be returned from an actual call.</span></span>
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



