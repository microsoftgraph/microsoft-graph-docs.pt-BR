---
title: Criar deviceComplianceSettingState
description: Criar um novo objeto deviceComplianceSettingState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3bb79b130b1e77167ad8aecbd87d462b15581cce
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402717"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="b6e13-103">Criar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="b6e13-103">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="b6e13-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="b6e13-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b6e13-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b6e13-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6e13-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b6e13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6e13-107">Criar um novo objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="b6e13-107">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6e13-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6e13-108">Prerequisites</span></span>
<span data-ttu-id="b6e13-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b6e13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b6e13-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6e13-111">Permission type</span></span>|<span data-ttu-id="b6e13-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6e13-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6e13-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6e13-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6e13-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6e13-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6e13-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6e13-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6e13-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6e13-116">Not supported.</span></span>|
|<span data-ttu-id="b6e13-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6e13-117">Application</span></span>|<span data-ttu-id="b6e13-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6e13-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6e13-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6e13-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="b6e13-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6e13-120">Request headers</span></span>
|<span data-ttu-id="b6e13-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6e13-121">Header</span></span>|<span data-ttu-id="b6e13-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b6e13-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6e13-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6e13-123">Authorization</span></span>|<span data-ttu-id="b6e13-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6e13-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6e13-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6e13-125">Accept</span></span>|<span data-ttu-id="b6e13-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6e13-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6e13-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6e13-127">Request body</span></span>
<span data-ttu-id="b6e13-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="b6e13-128">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="b6e13-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="b6e13-129">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="b6e13-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6e13-130">Property</span></span>|<span data-ttu-id="b6e13-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6e13-131">Type</span></span>|<span data-ttu-id="b6e13-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6e13-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6e13-133">id</span><span class="sxs-lookup"><span data-stu-id="b6e13-133">id</span></span>|<span data-ttu-id="b6e13-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e13-134">String</span></span>|<span data-ttu-id="b6e13-135">Chave da entidade</span><span class="sxs-lookup"><span data-stu-id="b6e13-135">Key of the entity</span></span>|
|<span data-ttu-id="b6e13-136">platformType</span><span class="sxs-lookup"><span data-stu-id="b6e13-136">platformType</span></span>|[<span data-ttu-id="b6e13-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="b6e13-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="b6e13-138">Tipo de plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6e13-138">Device platform type.</span></span> <span data-ttu-id="b6e13-139">Os valores possíveis são: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="b6e13-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="b6e13-140">configuração</span><span class="sxs-lookup"><span data-stu-id="b6e13-140">setting</span></span>|<span data-ttu-id="b6e13-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e13-141">String</span></span>|<span data-ttu-id="b6e13-142">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="b6e13-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="b6e13-143">settingName</span><span class="sxs-lookup"><span data-stu-id="b6e13-143">settingName</span></span>|<span data-ttu-id="b6e13-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e13-144">String</span></span>|<span data-ttu-id="b6e13-145">O nome da configuração sendo relatada</span><span class="sxs-lookup"><span data-stu-id="b6e13-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="b6e13-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="b6e13-146">deviceId</span></span>|<span data-ttu-id="b6e13-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e13-147">String</span></span>|<span data-ttu-id="b6e13-148">A ID do dispositivo sendo relatada</span><span class="sxs-lookup"><span data-stu-id="b6e13-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="b6e13-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="b6e13-149">deviceName</span></span>|<span data-ttu-id="b6e13-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e13-150">String</span></span>|<span data-ttu-id="b6e13-151">O nome do dispositivo sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b6e13-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="b6e13-152">userId</span><span class="sxs-lookup"><span data-stu-id="b6e13-152">userId</span></span>|<span data-ttu-id="b6e13-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e13-153">String</span></span>|<span data-ttu-id="b6e13-154">A ID do usuário sendo relatada</span><span class="sxs-lookup"><span data-stu-id="b6e13-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="b6e13-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="b6e13-155">userEmail</span></span>|<span data-ttu-id="b6e13-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e13-156">String</span></span>|<span data-ttu-id="b6e13-157">O endereço de email do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b6e13-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="b6e13-158">userName</span><span class="sxs-lookup"><span data-stu-id="b6e13-158">userName</span></span>|<span data-ttu-id="b6e13-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e13-159">String</span></span>|<span data-ttu-id="b6e13-160">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b6e13-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="b6e13-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b6e13-161">userPrincipalName</span></span>|<span data-ttu-id="b6e13-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e13-162">String</span></span>|<span data-ttu-id="b6e13-163">O PrincipalName do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b6e13-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="b6e13-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="b6e13-164">deviceModel</span></span>|<span data-ttu-id="b6e13-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e13-165">String</span></span>|<span data-ttu-id="b6e13-166">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b6e13-166">The device model that is being reported</span></span>|
|<span data-ttu-id="b6e13-167">estado</span><span class="sxs-lookup"><span data-stu-id="b6e13-167">state</span></span>|[<span data-ttu-id="b6e13-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b6e13-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b6e13-169">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="b6e13-169">The compliance state of the setting.</span></span> <span data-ttu-id="b6e13-170">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b6e13-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b6e13-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b6e13-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b6e13-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6e13-172">DateTimeOffset</span></span>|<span data-ttu-id="b6e13-173">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="b6e13-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="b6e13-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6e13-174">Response</span></span>
<span data-ttu-id="b6e13-175">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6e13-175">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6e13-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6e13-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6e13-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6e13-177">Request</span></span>
<span data-ttu-id="b6e13-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6e13-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b6e13-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6e13-179">Response</span></span>
<span data-ttu-id="b6e13-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6e13-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




