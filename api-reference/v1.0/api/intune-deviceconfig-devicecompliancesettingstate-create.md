---
title: Criar deviceComplianceSettingState
description: Criar um novo objeto deviceComplianceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0cb1deb234005cfdb7a206ddabbbc562f8e91299
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758376"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="75537-103">Criar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="75537-103">Create deviceComplianceSettingState</span></span>

<span data-ttu-id="75537-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75537-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75537-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75537-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75537-106">Criar um novo objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="75537-106">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75537-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="75537-107">Prerequisites</span></span>
<span data-ttu-id="75537-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75537-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75537-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75537-110">Permission type</span></span>|<span data-ttu-id="75537-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75537-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75537-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75537-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75537-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75537-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75537-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75537-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75537-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75537-115">Not supported.</span></span>|
|<span data-ttu-id="75537-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75537-116">Application</span></span>|<span data-ttu-id="75537-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75537-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75537-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75537-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="75537-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75537-119">Request headers</span></span>
|<span data-ttu-id="75537-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75537-120">Header</span></span>|<span data-ttu-id="75537-121">Valor</span><span class="sxs-lookup"><span data-stu-id="75537-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75537-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="75537-122">Authorization</span></span>|<span data-ttu-id="75537-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75537-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75537-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="75537-124">Accept</span></span>|<span data-ttu-id="75537-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75537-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75537-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75537-126">Request body</span></span>
<span data-ttu-id="75537-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="75537-127">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="75537-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="75537-128">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="75537-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75537-129">Property</span></span>|<span data-ttu-id="75537-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="75537-130">Type</span></span>|<span data-ttu-id="75537-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="75537-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75537-132">id</span><span class="sxs-lookup"><span data-stu-id="75537-132">id</span></span>|<span data-ttu-id="75537-133">String</span><span class="sxs-lookup"><span data-stu-id="75537-133">String</span></span>|<span data-ttu-id="75537-134">Chave da entidade</span><span class="sxs-lookup"><span data-stu-id="75537-134">Key of the entity</span></span>|
|<span data-ttu-id="75537-135">configuração</span><span class="sxs-lookup"><span data-stu-id="75537-135">setting</span></span>|<span data-ttu-id="75537-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75537-136">String</span></span>|<span data-ttu-id="75537-137">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="75537-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="75537-138">settingName</span><span class="sxs-lookup"><span data-stu-id="75537-138">settingName</span></span>|<span data-ttu-id="75537-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75537-139">String</span></span>|<span data-ttu-id="75537-140">O nome da configuração sendo relatada</span><span class="sxs-lookup"><span data-stu-id="75537-140">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="75537-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="75537-141">deviceId</span></span>|<span data-ttu-id="75537-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75537-142">String</span></span>|<span data-ttu-id="75537-143">A ID do dispositivo sendo relatada</span><span class="sxs-lookup"><span data-stu-id="75537-143">The Device Id that is being reported</span></span>|
|<span data-ttu-id="75537-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="75537-144">deviceName</span></span>|<span data-ttu-id="75537-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75537-145">String</span></span>|<span data-ttu-id="75537-146">O nome do dispositivo sendo relatado</span><span class="sxs-lookup"><span data-stu-id="75537-146">The Device Name that is being reported</span></span>|
|<span data-ttu-id="75537-147">userId</span><span class="sxs-lookup"><span data-stu-id="75537-147">userId</span></span>|<span data-ttu-id="75537-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75537-148">String</span></span>|<span data-ttu-id="75537-149">A ID do usuário sendo relatada</span><span class="sxs-lookup"><span data-stu-id="75537-149">The user Id that is being reported</span></span>|
|<span data-ttu-id="75537-150">userEmail</span><span class="sxs-lookup"><span data-stu-id="75537-150">userEmail</span></span>|<span data-ttu-id="75537-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75537-151">String</span></span>|<span data-ttu-id="75537-152">O endereço de email do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="75537-152">The User email address that is being reported</span></span>|
|<span data-ttu-id="75537-153">userName</span><span class="sxs-lookup"><span data-stu-id="75537-153">userName</span></span>|<span data-ttu-id="75537-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75537-154">String</span></span>|<span data-ttu-id="75537-155">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="75537-155">The User Name that is being reported</span></span>|
|<span data-ttu-id="75537-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="75537-156">userPrincipalName</span></span>|<span data-ttu-id="75537-157">String</span><span class="sxs-lookup"><span data-stu-id="75537-157">String</span></span>|<span data-ttu-id="75537-158">O PrincipalName do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="75537-158">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="75537-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="75537-159">deviceModel</span></span>|<span data-ttu-id="75537-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75537-160">String</span></span>|<span data-ttu-id="75537-161">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="75537-161">The device model that is being reported</span></span>|
|<span data-ttu-id="75537-162">state</span><span class="sxs-lookup"><span data-stu-id="75537-162">state</span></span>|[<span data-ttu-id="75537-163">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="75537-163">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="75537-164">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="75537-164">The compliance state of the setting.</span></span> <span data-ttu-id="75537-165">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="75537-165">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="75537-166">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="75537-166">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="75537-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75537-167">DateTimeOffset</span></span>|<span data-ttu-id="75537-168">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="75537-168">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="75537-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="75537-169">Response</span></span>
<span data-ttu-id="75537-170">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75537-170">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75537-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75537-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="75537-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75537-172">Request</span></span>
<span data-ttu-id="75537-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75537-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="75537-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="75537-174">Response</span></span>
<span data-ttu-id="75537-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75537-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




