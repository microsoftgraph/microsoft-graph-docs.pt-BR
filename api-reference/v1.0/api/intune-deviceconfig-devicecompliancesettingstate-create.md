---
title: Criar deviceComplianceSettingState
description: Criar um novo objeto deviceComplianceSettingState.
ms.openlocfilehash: d9d1e8fb4d30fbb63381cdf90928ab815539ffca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003395"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="3f11b-103">Criar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="3f11b-103">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="3f11b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3f11b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3f11b-105">Criar um novo objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="3f11b-105">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3f11b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3f11b-106">Prerequisites</span></span>
<span data-ttu-id="3f11b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f11b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f11b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f11b-109">Permission type</span></span>|<span data-ttu-id="3f11b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3f11b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f11b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f11b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3f11b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f11b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3f11b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f11b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f11b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f11b-114">Not supported.</span></span>|
|<span data-ttu-id="3f11b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f11b-115">Application</span></span>|<span data-ttu-id="3f11b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f11b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f11b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f11b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="3f11b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f11b-118">Request headers</span></span>
|<span data-ttu-id="3f11b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3f11b-119">Header</span></span>|<span data-ttu-id="3f11b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="3f11b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f11b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f11b-121">Authorization</span></span>|<span data-ttu-id="3f11b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f11b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f11b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3f11b-123">Accept</span></span>|<span data-ttu-id="3f11b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3f11b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f11b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f11b-125">Request body</span></span>
<span data-ttu-id="3f11b-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="3f11b-126">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="3f11b-127">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="3f11b-127">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="3f11b-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f11b-128">Property</span></span>|<span data-ttu-id="3f11b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f11b-129">Type</span></span>|<span data-ttu-id="3f11b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f11b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f11b-131">id</span><span class="sxs-lookup"><span data-stu-id="3f11b-131">id</span></span>|<span data-ttu-id="3f11b-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f11b-132">String</span></span>|<span data-ttu-id="3f11b-133">Chave da entidade</span><span class="sxs-lookup"><span data-stu-id="3f11b-133">Key of the entity</span></span>|
|<span data-ttu-id="3f11b-134">configuração</span><span class="sxs-lookup"><span data-stu-id="3f11b-134">setting</span></span>|<span data-ttu-id="3f11b-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f11b-135">String</span></span>|<span data-ttu-id="3f11b-136">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="3f11b-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="3f11b-137">settingName</span><span class="sxs-lookup"><span data-stu-id="3f11b-137">settingName</span></span>|<span data-ttu-id="3f11b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f11b-138">String</span></span>|<span data-ttu-id="3f11b-139">O nome da configuração sendo relatada</span><span class="sxs-lookup"><span data-stu-id="3f11b-139">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="3f11b-140">deviceId</span><span class="sxs-lookup"><span data-stu-id="3f11b-140">deviceId</span></span>|<span data-ttu-id="3f11b-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f11b-141">String</span></span>|<span data-ttu-id="3f11b-142">A ID do dispositivo sendo relatada</span><span class="sxs-lookup"><span data-stu-id="3f11b-142">The Device Id that is being reported</span></span>|
|<span data-ttu-id="3f11b-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="3f11b-143">deviceName</span></span>|<span data-ttu-id="3f11b-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f11b-144">String</span></span>|<span data-ttu-id="3f11b-145">O nome do dispositivo sendo relatado</span><span class="sxs-lookup"><span data-stu-id="3f11b-145">The Device Name that is being reported</span></span>|
|<span data-ttu-id="3f11b-146">userId</span><span class="sxs-lookup"><span data-stu-id="3f11b-146">userId</span></span>|<span data-ttu-id="3f11b-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f11b-147">String</span></span>|<span data-ttu-id="3f11b-148">A ID do usuário sendo relatada</span><span class="sxs-lookup"><span data-stu-id="3f11b-148">The user Id that is being reported</span></span>|
|<span data-ttu-id="3f11b-149">userEmail</span><span class="sxs-lookup"><span data-stu-id="3f11b-149">userEmail</span></span>|<span data-ttu-id="3f11b-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f11b-150">String</span></span>|<span data-ttu-id="3f11b-151">O endereço de email do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="3f11b-151">The User email address that is being reported</span></span>|
|<span data-ttu-id="3f11b-152">userName</span><span class="sxs-lookup"><span data-stu-id="3f11b-152">userName</span></span>|<span data-ttu-id="3f11b-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f11b-153">String</span></span>|<span data-ttu-id="3f11b-154">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="3f11b-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="3f11b-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3f11b-155">userPrincipalName</span></span>|<span data-ttu-id="3f11b-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f11b-156">String</span></span>|<span data-ttu-id="3f11b-157">O PrincipalName do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="3f11b-157">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="3f11b-158">deviceModel</span><span class="sxs-lookup"><span data-stu-id="3f11b-158">deviceModel</span></span>|<span data-ttu-id="3f11b-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f11b-159">String</span></span>|<span data-ttu-id="3f11b-160">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="3f11b-160">The device model that is being reported</span></span>|
|<span data-ttu-id="3f11b-161">state</span><span class="sxs-lookup"><span data-stu-id="3f11b-161">state</span></span>|[<span data-ttu-id="3f11b-162">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="3f11b-162">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="3f11b-163">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="3f11b-163">The compliance state of the setting.</span></span> <span data-ttu-id="3f11b-164">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="3f11b-164">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="3f11b-165">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3f11b-165">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="3f11b-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f11b-166">DateTimeOffset</span></span>|<span data-ttu-id="3f11b-167">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="3f11b-167">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="3f11b-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f11b-168">Response</span></span>
<span data-ttu-id="3f11b-169">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f11b-169">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f11b-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f11b-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="3f11b-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f11b-171">Request</span></span>
<span data-ttu-id="3f11b-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f11b-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
Content-type: application/json
Content-length: 517

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
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

### <a name="response"></a><span data-ttu-id="3f11b-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f11b-173">Response</span></span>
<span data-ttu-id="3f11b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3f11b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 566

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "9905f955-f955-9905-55f9-059955f90599",
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



