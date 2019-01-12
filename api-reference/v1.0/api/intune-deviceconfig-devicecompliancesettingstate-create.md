---
title: Criar deviceComplianceSettingState
description: Criar um novo objeto deviceComplianceSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1914c143bc4c5c7bb40acfcdd4b57cead1070a8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956980"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="3b3c0-103">Criar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="3b3c0-103">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="3b3c0-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3b3c0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b3c0-105">Criar um novo objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="3b3c0-105">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b3c0-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b3c0-106">Prerequisites</span></span>
<span data-ttu-id="3b3c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b3c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b3c0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b3c0-109">Permission type</span></span>|<span data-ttu-id="3b3c0-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b3c0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b3c0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b3c0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3b3c0-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b3c0-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3b3c0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b3c0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b3c0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b3c0-114">Not supported.</span></span>|
|<span data-ttu-id="3b3c0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b3c0-115">Application</span></span>|<span data-ttu-id="3b3c0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b3c0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b3c0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b3c0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="3b3c0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b3c0-118">Request headers</span></span>
|<span data-ttu-id="3b3c0-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b3c0-119">Header</span></span>|<span data-ttu-id="3b3c0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="3b3c0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b3c0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b3c0-121">Authorization</span></span>|<span data-ttu-id="3b3c0-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b3c0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b3c0-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b3c0-123">Accept</span></span>|<span data-ttu-id="3b3c0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3b3c0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b3c0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b3c0-125">Request body</span></span>
<span data-ttu-id="3b3c0-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="3b3c0-126">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="3b3c0-127">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="3b3c0-127">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="3b3c0-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b3c0-128">Property</span></span>|<span data-ttu-id="3b3c0-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b3c0-129">Type</span></span>|<span data-ttu-id="3b3c0-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b3c0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b3c0-131">id</span><span class="sxs-lookup"><span data-stu-id="3b3c0-131">id</span></span>|<span data-ttu-id="3b3c0-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3c0-132">String</span></span>|<span data-ttu-id="3b3c0-133">Chave da entidade</span><span class="sxs-lookup"><span data-stu-id="3b3c0-133">Key of the entity</span></span>|
|<span data-ttu-id="3b3c0-134">configuração</span><span class="sxs-lookup"><span data-stu-id="3b3c0-134">setting</span></span>|<span data-ttu-id="3b3c0-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3c0-135">String</span></span>|<span data-ttu-id="3b3c0-136">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="3b3c0-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="3b3c0-137">settingName</span><span class="sxs-lookup"><span data-stu-id="3b3c0-137">settingName</span></span>|<span data-ttu-id="3b3c0-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3c0-138">String</span></span>|<span data-ttu-id="3b3c0-139">O nome da configuração sendo relatada</span><span class="sxs-lookup"><span data-stu-id="3b3c0-139">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="3b3c0-140">deviceId</span><span class="sxs-lookup"><span data-stu-id="3b3c0-140">deviceId</span></span>|<span data-ttu-id="3b3c0-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3c0-141">String</span></span>|<span data-ttu-id="3b3c0-142">A ID do dispositivo sendo relatada</span><span class="sxs-lookup"><span data-stu-id="3b3c0-142">The Device Id that is being reported</span></span>|
|<span data-ttu-id="3b3c0-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="3b3c0-143">deviceName</span></span>|<span data-ttu-id="3b3c0-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3c0-144">String</span></span>|<span data-ttu-id="3b3c0-145">O nome do dispositivo sendo relatado</span><span class="sxs-lookup"><span data-stu-id="3b3c0-145">The Device Name that is being reported</span></span>|
|<span data-ttu-id="3b3c0-146">userId</span><span class="sxs-lookup"><span data-stu-id="3b3c0-146">userId</span></span>|<span data-ttu-id="3b3c0-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3c0-147">String</span></span>|<span data-ttu-id="3b3c0-148">A ID do usuário sendo relatada</span><span class="sxs-lookup"><span data-stu-id="3b3c0-148">The user Id that is being reported</span></span>|
|<span data-ttu-id="3b3c0-149">userEmail</span><span class="sxs-lookup"><span data-stu-id="3b3c0-149">userEmail</span></span>|<span data-ttu-id="3b3c0-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3c0-150">String</span></span>|<span data-ttu-id="3b3c0-151">O endereço de email do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="3b3c0-151">The User email address that is being reported</span></span>|
|<span data-ttu-id="3b3c0-152">userName</span><span class="sxs-lookup"><span data-stu-id="3b3c0-152">userName</span></span>|<span data-ttu-id="3b3c0-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3c0-153">String</span></span>|<span data-ttu-id="3b3c0-154">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="3b3c0-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="3b3c0-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3b3c0-155">userPrincipalName</span></span>|<span data-ttu-id="3b3c0-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3c0-156">String</span></span>|<span data-ttu-id="3b3c0-157">O PrincipalName do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="3b3c0-157">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="3b3c0-158">deviceModel</span><span class="sxs-lookup"><span data-stu-id="3b3c0-158">deviceModel</span></span>|<span data-ttu-id="3b3c0-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3c0-159">String</span></span>|<span data-ttu-id="3b3c0-160">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="3b3c0-160">The device model that is being reported</span></span>|
|<span data-ttu-id="3b3c0-161">estado</span><span class="sxs-lookup"><span data-stu-id="3b3c0-161">state</span></span>|[<span data-ttu-id="3b3c0-162">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="3b3c0-162">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="3b3c0-163">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="3b3c0-163">The compliance state of the setting.</span></span> <span data-ttu-id="3b3c0-164">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="3b3c0-164">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="3b3c0-165">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3b3c0-165">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="3b3c0-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b3c0-166">DateTimeOffset</span></span>|<span data-ttu-id="3b3c0-167">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="3b3c0-167">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="3b3c0-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b3c0-168">Response</span></span>
<span data-ttu-id="3b3c0-169">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b3c0-169">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b3c0-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b3c0-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b3c0-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b3c0-171">Request</span></span>
<span data-ttu-id="3b3c0-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b3c0-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3b3c0-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b3c0-173">Response</span></span>
<span data-ttu-id="3b3c0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b3c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



