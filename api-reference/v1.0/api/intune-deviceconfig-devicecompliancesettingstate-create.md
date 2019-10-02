---
title: Criar deviceComplianceSettingState
description: Criar um novo objeto deviceComplianceSettingState.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 63f96acfa229360438434b08328d1799dc3819b2
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354102"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="b0fda-103">Criar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="b0fda-103">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="b0fda-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0fda-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0fda-105">Criar um novo objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="b0fda-105">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0fda-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0fda-106">Prerequisites</span></span>
<span data-ttu-id="b0fda-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0fda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0fda-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0fda-109">Permission type</span></span>|<span data-ttu-id="b0fda-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b0fda-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0fda-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0fda-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b0fda-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0fda-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0fda-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0fda-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0fda-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0fda-114">Not supported.</span></span>|
|<span data-ttu-id="b0fda-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0fda-115">Application</span></span>|<span data-ttu-id="b0fda-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0fda-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0fda-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0fda-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="b0fda-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0fda-118">Request headers</span></span>
|<span data-ttu-id="b0fda-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0fda-119">Header</span></span>|<span data-ttu-id="b0fda-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b0fda-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0fda-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0fda-121">Authorization</span></span>|<span data-ttu-id="b0fda-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0fda-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0fda-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b0fda-123">Accept</span></span>|<span data-ttu-id="b0fda-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b0fda-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0fda-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0fda-125">Request body</span></span>
<span data-ttu-id="b0fda-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="b0fda-126">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="b0fda-127">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="b0fda-127">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="b0fda-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0fda-128">Property</span></span>|<span data-ttu-id="b0fda-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0fda-129">Type</span></span>|<span data-ttu-id="b0fda-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0fda-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0fda-131">id</span><span class="sxs-lookup"><span data-stu-id="b0fda-131">id</span></span>|<span data-ttu-id="b0fda-132">String</span><span class="sxs-lookup"><span data-stu-id="b0fda-132">String</span></span>|<span data-ttu-id="b0fda-133">Chave da entidade</span><span class="sxs-lookup"><span data-stu-id="b0fda-133">Key of the entity</span></span>|
|<span data-ttu-id="b0fda-134">configuração</span><span class="sxs-lookup"><span data-stu-id="b0fda-134">setting</span></span>|<span data-ttu-id="b0fda-135">String</span><span class="sxs-lookup"><span data-stu-id="b0fda-135">String</span></span>|<span data-ttu-id="b0fda-136">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="b0fda-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="b0fda-137">settingName</span><span class="sxs-lookup"><span data-stu-id="b0fda-137">settingName</span></span>|<span data-ttu-id="b0fda-138">String</span><span class="sxs-lookup"><span data-stu-id="b0fda-138">String</span></span>|<span data-ttu-id="b0fda-139">O nome da configuração sendo relatada</span><span class="sxs-lookup"><span data-stu-id="b0fda-139">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="b0fda-140">deviceId</span><span class="sxs-lookup"><span data-stu-id="b0fda-140">deviceId</span></span>|<span data-ttu-id="b0fda-141">String</span><span class="sxs-lookup"><span data-stu-id="b0fda-141">String</span></span>|<span data-ttu-id="b0fda-142">A ID do dispositivo sendo relatada</span><span class="sxs-lookup"><span data-stu-id="b0fda-142">The Device Id that is being reported</span></span>|
|<span data-ttu-id="b0fda-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="b0fda-143">deviceName</span></span>|<span data-ttu-id="b0fda-144">String</span><span class="sxs-lookup"><span data-stu-id="b0fda-144">String</span></span>|<span data-ttu-id="b0fda-145">O nome do dispositivo sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b0fda-145">The Device Name that is being reported</span></span>|
|<span data-ttu-id="b0fda-146">userId</span><span class="sxs-lookup"><span data-stu-id="b0fda-146">userId</span></span>|<span data-ttu-id="b0fda-147">String</span><span class="sxs-lookup"><span data-stu-id="b0fda-147">String</span></span>|<span data-ttu-id="b0fda-148">A ID do usuário sendo relatada</span><span class="sxs-lookup"><span data-stu-id="b0fda-148">The user Id that is being reported</span></span>|
|<span data-ttu-id="b0fda-149">userEmail</span><span class="sxs-lookup"><span data-stu-id="b0fda-149">userEmail</span></span>|<span data-ttu-id="b0fda-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0fda-150">String</span></span>|<span data-ttu-id="b0fda-151">O endereço de email do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b0fda-151">The User email address that is being reported</span></span>|
|<span data-ttu-id="b0fda-152">userName</span><span class="sxs-lookup"><span data-stu-id="b0fda-152">userName</span></span>|<span data-ttu-id="b0fda-153">String</span><span class="sxs-lookup"><span data-stu-id="b0fda-153">String</span></span>|<span data-ttu-id="b0fda-154">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b0fda-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="b0fda-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b0fda-155">userPrincipalName</span></span>|<span data-ttu-id="b0fda-156">String</span><span class="sxs-lookup"><span data-stu-id="b0fda-156">String</span></span>|<span data-ttu-id="b0fda-157">O PrincipalName do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b0fda-157">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="b0fda-158">deviceModel</span><span class="sxs-lookup"><span data-stu-id="b0fda-158">deviceModel</span></span>|<span data-ttu-id="b0fda-159">String</span><span class="sxs-lookup"><span data-stu-id="b0fda-159">String</span></span>|<span data-ttu-id="b0fda-160">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b0fda-160">The device model that is being reported</span></span>|
|<span data-ttu-id="b0fda-161">state</span><span class="sxs-lookup"><span data-stu-id="b0fda-161">state</span></span>|[<span data-ttu-id="b0fda-162">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b0fda-162">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b0fda-163">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="b0fda-163">The compliance state of the setting.</span></span> <span data-ttu-id="b0fda-164">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b0fda-164">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b0fda-165">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b0fda-165">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b0fda-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0fda-166">DateTimeOffset</span></span>|<span data-ttu-id="b0fda-167">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="b0fda-167">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="b0fda-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0fda-168">Response</span></span>
<span data-ttu-id="b0fda-169">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0fda-169">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0fda-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0fda-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0fda-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0fda-171">Request</span></span>
<span data-ttu-id="b0fda-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0fda-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b0fda-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0fda-173">Response</span></span>
<span data-ttu-id="b0fda-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0fda-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




