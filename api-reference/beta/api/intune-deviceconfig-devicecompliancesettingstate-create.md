---
title: Criar deviceComplianceSettingState
description: Criar um novo objeto deviceComplianceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7f31cf3bae143d92ba981cab2f6eea1391cb1044
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49213900"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="0e08a-103">Criar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="0e08a-103">Create deviceComplianceSettingState</span></span>

<span data-ttu-id="0e08a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e08a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e08a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e08a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e08a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e08a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e08a-107">Criar um novo objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="0e08a-107">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e08a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0e08a-108">Prerequisites</span></span>
<span data-ttu-id="0e08a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e08a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e08a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e08a-111">Permission type</span></span>|<span data-ttu-id="0e08a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0e08a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e08a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e08a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e08a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e08a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e08a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e08a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e08a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e08a-116">Not supported.</span></span>|
|<span data-ttu-id="0e08a-117">Application</span><span class="sxs-lookup"><span data-stu-id="0e08a-117">Application</span></span>|<span data-ttu-id="0e08a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e08a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e08a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e08a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="0e08a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e08a-120">Request headers</span></span>
|<span data-ttu-id="0e08a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0e08a-121">Header</span></span>|<span data-ttu-id="0e08a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0e08a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e08a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e08a-123">Authorization</span></span>|<span data-ttu-id="0e08a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e08a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e08a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0e08a-125">Accept</span></span>|<span data-ttu-id="0e08a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e08a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e08a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e08a-127">Request body</span></span>
<span data-ttu-id="0e08a-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="0e08a-128">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="0e08a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="0e08a-129">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="0e08a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e08a-130">Property</span></span>|<span data-ttu-id="0e08a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e08a-131">Type</span></span>|<span data-ttu-id="0e08a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e08a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e08a-133">id</span><span class="sxs-lookup"><span data-stu-id="0e08a-133">id</span></span>|<span data-ttu-id="0e08a-134">String</span><span class="sxs-lookup"><span data-stu-id="0e08a-134">String</span></span>|<span data-ttu-id="0e08a-135">Chave da entidade</span><span class="sxs-lookup"><span data-stu-id="0e08a-135">Key of the entity</span></span>|
|<span data-ttu-id="0e08a-136">platformType</span><span class="sxs-lookup"><span data-stu-id="0e08a-136">platformType</span></span>|[<span data-ttu-id="0e08a-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="0e08a-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="0e08a-138">Tipo de plataforma de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0e08a-138">Device platform type.</span></span> <span data-ttu-id="0e08a-139">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` , `androidForWork` , `androidEnterprise` , `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` `unknown` ,,,,,.</span><span class="sxs-lookup"><span data-stu-id="0e08a-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `cloudPC`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="0e08a-140">configuração</span><span class="sxs-lookup"><span data-stu-id="0e08a-140">setting</span></span>|<span data-ttu-id="0e08a-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e08a-141">String</span></span>|<span data-ttu-id="0e08a-142">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="0e08a-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="0e08a-143">settingName</span><span class="sxs-lookup"><span data-stu-id="0e08a-143">settingName</span></span>|<span data-ttu-id="0e08a-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e08a-144">String</span></span>|<span data-ttu-id="0e08a-145">O nome da configuração sendo relatada</span><span class="sxs-lookup"><span data-stu-id="0e08a-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="0e08a-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="0e08a-146">deviceId</span></span>|<span data-ttu-id="0e08a-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e08a-147">String</span></span>|<span data-ttu-id="0e08a-148">A ID do dispositivo sendo relatada</span><span class="sxs-lookup"><span data-stu-id="0e08a-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="0e08a-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="0e08a-149">deviceName</span></span>|<span data-ttu-id="0e08a-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e08a-150">String</span></span>|<span data-ttu-id="0e08a-151">O nome do dispositivo sendo relatado</span><span class="sxs-lookup"><span data-stu-id="0e08a-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="0e08a-152">userId</span><span class="sxs-lookup"><span data-stu-id="0e08a-152">userId</span></span>|<span data-ttu-id="0e08a-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e08a-153">String</span></span>|<span data-ttu-id="0e08a-154">A ID do usuário sendo relatada</span><span class="sxs-lookup"><span data-stu-id="0e08a-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="0e08a-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="0e08a-155">userEmail</span></span>|<span data-ttu-id="0e08a-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e08a-156">String</span></span>|<span data-ttu-id="0e08a-157">O endereço de email do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="0e08a-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="0e08a-158">userName</span><span class="sxs-lookup"><span data-stu-id="0e08a-158">userName</span></span>|<span data-ttu-id="0e08a-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e08a-159">String</span></span>|<span data-ttu-id="0e08a-160">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="0e08a-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="0e08a-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0e08a-161">userPrincipalName</span></span>|<span data-ttu-id="0e08a-162">String</span><span class="sxs-lookup"><span data-stu-id="0e08a-162">String</span></span>|<span data-ttu-id="0e08a-163">O PrincipalName do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="0e08a-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="0e08a-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="0e08a-164">deviceModel</span></span>|<span data-ttu-id="0e08a-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e08a-165">String</span></span>|<span data-ttu-id="0e08a-166">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="0e08a-166">The device model that is being reported</span></span>|
|<span data-ttu-id="0e08a-167">state</span><span class="sxs-lookup"><span data-stu-id="0e08a-167">state</span></span>|[<span data-ttu-id="0e08a-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="0e08a-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="0e08a-169">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="0e08a-169">The compliance state of the setting.</span></span> <span data-ttu-id="0e08a-170">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="0e08a-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="0e08a-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0e08a-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="0e08a-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e08a-172">DateTimeOffset</span></span>|<span data-ttu-id="0e08a-173">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="0e08a-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="0e08a-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e08a-174">Response</span></span>
<span data-ttu-id="0e08a-175">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e08a-175">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e08a-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e08a-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e08a-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e08a-177">Request</span></span>
<span data-ttu-id="0e08a-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e08a-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
Content-type: application/json
Content-length: 549

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
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

### <a name="response"></a><span data-ttu-id="0e08a-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e08a-179">Response</span></span>
<span data-ttu-id="0e08a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e08a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 598

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "9905f955-f955-9905-55f9-059955f90599",
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




