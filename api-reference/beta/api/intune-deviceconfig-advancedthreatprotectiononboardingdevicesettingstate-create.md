---
title: Criar advancedThreatProtectionOnboardingDeviceSettingState
description: Crie um novo objeto de advancedThreatProtectionOnboardingDeviceSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 878d887ff792558e9fa82d04490254d1e7190308
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933782"
---
# <a name="create-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="d60b8-103">Criar advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="d60b8-103">Create advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="d60b8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d60b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d60b8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d60b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d60b8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d60b8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d60b8-107">Crie um novo objeto de [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="d60b8-107">Create a new [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d60b8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d60b8-108">Prerequisites</span></span>
<span data-ttu-id="d60b8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d60b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d60b8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d60b8-111">Permission type</span></span>|<span data-ttu-id="d60b8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d60b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d60b8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d60b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d60b8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d60b8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d60b8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d60b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d60b8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d60b8-116">Not supported.</span></span>|
|<span data-ttu-id="d60b8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d60b8-117">Application</span></span>|<span data-ttu-id="d60b8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d60b8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d60b8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d60b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="d60b8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d60b8-120">Request headers</span></span>
|<span data-ttu-id="d60b8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d60b8-121">Header</span></span>|<span data-ttu-id="d60b8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d60b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d60b8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d60b8-123">Authorization</span></span>|<span data-ttu-id="d60b8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d60b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d60b8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d60b8-125">Accept</span></span>|<span data-ttu-id="d60b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d60b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d60b8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d60b8-127">Request body</span></span>
<span data-ttu-id="d60b8-128">No corpo da solicitação, fornece uma representação JSON para o objeto advancedThreatProtectionOnboardingDeviceSettingState.</span><span class="sxs-lookup"><span data-stu-id="d60b8-128">In the request body, supply a JSON representation for the advancedThreatProtectionOnboardingDeviceSettingState object.</span></span>

<span data-ttu-id="d60b8-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o advancedThreatProtectionOnboardingDeviceSettingState.</span><span class="sxs-lookup"><span data-stu-id="d60b8-129">The following table shows the properties that are required when you create the advancedThreatProtectionOnboardingDeviceSettingState.</span></span>

|<span data-ttu-id="d60b8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d60b8-130">Property</span></span>|<span data-ttu-id="d60b8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d60b8-131">Type</span></span>|<span data-ttu-id="d60b8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d60b8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d60b8-133">id</span><span class="sxs-lookup"><span data-stu-id="d60b8-133">id</span></span>|<span data-ttu-id="d60b8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d60b8-134">String</span></span>|<span data-ttu-id="d60b8-135">Chave da entidade</span><span class="sxs-lookup"><span data-stu-id="d60b8-135">Key of the entity</span></span>|
|<span data-ttu-id="d60b8-136">platformType</span><span class="sxs-lookup"><span data-stu-id="d60b8-136">platformType</span></span>|[<span data-ttu-id="d60b8-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="d60b8-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="d60b8-138">Tipo de plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d60b8-138">Device platform type.</span></span> <span data-ttu-id="d60b8-139">Os valores possíveis são: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d60b8-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="d60b8-140">configuração</span><span class="sxs-lookup"><span data-stu-id="d60b8-140">setting</span></span>|<span data-ttu-id="d60b8-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d60b8-141">String</span></span>|<span data-ttu-id="d60b8-142">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="d60b8-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="d60b8-143">settingName</span><span class="sxs-lookup"><span data-stu-id="d60b8-143">settingName</span></span>|<span data-ttu-id="d60b8-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d60b8-144">String</span></span>|<span data-ttu-id="d60b8-145">O nome da configuração sendo relatada</span><span class="sxs-lookup"><span data-stu-id="d60b8-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="d60b8-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="d60b8-146">deviceId</span></span>|<span data-ttu-id="d60b8-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d60b8-147">String</span></span>|<span data-ttu-id="d60b8-148">A ID do dispositivo sendo relatada</span><span class="sxs-lookup"><span data-stu-id="d60b8-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="d60b8-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="d60b8-149">deviceName</span></span>|<span data-ttu-id="d60b8-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d60b8-150">String</span></span>|<span data-ttu-id="d60b8-151">O nome do dispositivo sendo relatado</span><span class="sxs-lookup"><span data-stu-id="d60b8-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="d60b8-152">userId</span><span class="sxs-lookup"><span data-stu-id="d60b8-152">userId</span></span>|<span data-ttu-id="d60b8-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d60b8-153">String</span></span>|<span data-ttu-id="d60b8-154">A ID do usuário sendo relatada</span><span class="sxs-lookup"><span data-stu-id="d60b8-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="d60b8-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="d60b8-155">userEmail</span></span>|<span data-ttu-id="d60b8-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d60b8-156">String</span></span>|<span data-ttu-id="d60b8-157">O endereço de email do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="d60b8-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="d60b8-158">userName</span><span class="sxs-lookup"><span data-stu-id="d60b8-158">userName</span></span>|<span data-ttu-id="d60b8-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d60b8-159">String</span></span>|<span data-ttu-id="d60b8-160">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="d60b8-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="d60b8-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d60b8-161">userPrincipalName</span></span>|<span data-ttu-id="d60b8-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d60b8-162">String</span></span>|<span data-ttu-id="d60b8-163">O PrincipalName do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="d60b8-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="d60b8-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="d60b8-164">deviceModel</span></span>|<span data-ttu-id="d60b8-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d60b8-165">String</span></span>|<span data-ttu-id="d60b8-166">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="d60b8-166">The device model that is being reported</span></span>|
|<span data-ttu-id="d60b8-167">estado</span><span class="sxs-lookup"><span data-stu-id="d60b8-167">state</span></span>|[<span data-ttu-id="d60b8-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d60b8-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d60b8-169">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="d60b8-169">The compliance state of the setting.</span></span> <span data-ttu-id="d60b8-170">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="d60b8-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d60b8-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d60b8-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d60b8-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d60b8-172">DateTimeOffset</span></span>|<span data-ttu-id="d60b8-173">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="d60b8-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="d60b8-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="d60b8-174">Response</span></span>
<span data-ttu-id="d60b8-175">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d60b8-175">If successful, this method returns a `201 Created` response code and a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d60b8-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d60b8-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="d60b8-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d60b8-177">Request</span></span>
<span data-ttu-id="d60b8-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d60b8-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d60b8-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="d60b8-179">Response</span></span>
<span data-ttu-id="d60b8-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d60b8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





