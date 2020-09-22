---
title: Atualizar deviceComplianceSettingState
description: Atualizar as propriedades de um objeto deviceComplianceSettingState objeto.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4cfb9c4a5723c77a1e0ae53149830efe97d93a72
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985248"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="d57c3-103">Atualizar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="d57c3-103">Update deviceComplianceSettingState</span></span>

<span data-ttu-id="d57c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d57c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d57c3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d57c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d57c3-106">Atualizar as propriedades de um objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objeto.</span><span class="sxs-lookup"><span data-stu-id="d57c3-106">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d57c3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d57c3-107">Prerequisites</span></span>
<span data-ttu-id="d57c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d57c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d57c3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d57c3-110">Permission type</span></span>|<span data-ttu-id="d57c3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d57c3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d57c3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d57c3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d57c3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d57c3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d57c3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d57c3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d57c3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d57c3-115">Not supported.</span></span>|
|<span data-ttu-id="d57c3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d57c3-116">Application</span></span>|<span data-ttu-id="d57c3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d57c3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d57c3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d57c3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="d57c3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d57c3-119">Request headers</span></span>
|<span data-ttu-id="d57c3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d57c3-120">Header</span></span>|<span data-ttu-id="d57c3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d57c3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d57c3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d57c3-122">Authorization</span></span>|<span data-ttu-id="d57c3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d57c3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d57c3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d57c3-124">Accept</span></span>|<span data-ttu-id="d57c3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d57c3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d57c3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d57c3-126">Request body</span></span>
<span data-ttu-id="d57c3-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="d57c3-127">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="d57c3-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="d57c3-128">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="d57c3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d57c3-129">Property</span></span>|<span data-ttu-id="d57c3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d57c3-130">Type</span></span>|<span data-ttu-id="d57c3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d57c3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d57c3-132">id</span><span class="sxs-lookup"><span data-stu-id="d57c3-132">id</span></span>|<span data-ttu-id="d57c3-133">String</span><span class="sxs-lookup"><span data-stu-id="d57c3-133">String</span></span>|<span data-ttu-id="d57c3-134">Chave da entidade</span><span class="sxs-lookup"><span data-stu-id="d57c3-134">Key of the entity</span></span>|
|<span data-ttu-id="d57c3-135">configuração</span><span class="sxs-lookup"><span data-stu-id="d57c3-135">setting</span></span>|<span data-ttu-id="d57c3-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d57c3-136">String</span></span>|<span data-ttu-id="d57c3-137">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="d57c3-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="d57c3-138">settingName</span><span class="sxs-lookup"><span data-stu-id="d57c3-138">settingName</span></span>|<span data-ttu-id="d57c3-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d57c3-139">String</span></span>|<span data-ttu-id="d57c3-140">O nome da configuração sendo relatada</span><span class="sxs-lookup"><span data-stu-id="d57c3-140">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="d57c3-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="d57c3-141">deviceId</span></span>|<span data-ttu-id="d57c3-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d57c3-142">String</span></span>|<span data-ttu-id="d57c3-143">A ID do dispositivo sendo relatada</span><span class="sxs-lookup"><span data-stu-id="d57c3-143">The Device Id that is being reported</span></span>|
|<span data-ttu-id="d57c3-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="d57c3-144">deviceName</span></span>|<span data-ttu-id="d57c3-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d57c3-145">String</span></span>|<span data-ttu-id="d57c3-146">O nome do dispositivo sendo relatado</span><span class="sxs-lookup"><span data-stu-id="d57c3-146">The Device Name that is being reported</span></span>|
|<span data-ttu-id="d57c3-147">userId</span><span class="sxs-lookup"><span data-stu-id="d57c3-147">userId</span></span>|<span data-ttu-id="d57c3-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d57c3-148">String</span></span>|<span data-ttu-id="d57c3-149">A ID do usuário sendo relatada</span><span class="sxs-lookup"><span data-stu-id="d57c3-149">The user Id that is being reported</span></span>|
|<span data-ttu-id="d57c3-150">userEmail</span><span class="sxs-lookup"><span data-stu-id="d57c3-150">userEmail</span></span>|<span data-ttu-id="d57c3-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d57c3-151">String</span></span>|<span data-ttu-id="d57c3-152">O endereço de email do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="d57c3-152">The User email address that is being reported</span></span>|
|<span data-ttu-id="d57c3-153">userName</span><span class="sxs-lookup"><span data-stu-id="d57c3-153">userName</span></span>|<span data-ttu-id="d57c3-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d57c3-154">String</span></span>|<span data-ttu-id="d57c3-155">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="d57c3-155">The User Name that is being reported</span></span>|
|<span data-ttu-id="d57c3-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d57c3-156">userPrincipalName</span></span>|<span data-ttu-id="d57c3-157">String</span><span class="sxs-lookup"><span data-stu-id="d57c3-157">String</span></span>|<span data-ttu-id="d57c3-158">O PrincipalName do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="d57c3-158">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="d57c3-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="d57c3-159">deviceModel</span></span>|<span data-ttu-id="d57c3-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d57c3-160">String</span></span>|<span data-ttu-id="d57c3-161">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="d57c3-161">The device model that is being reported</span></span>|
|<span data-ttu-id="d57c3-162">state</span><span class="sxs-lookup"><span data-stu-id="d57c3-162">state</span></span>|[<span data-ttu-id="d57c3-163">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d57c3-163">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d57c3-164">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="d57c3-164">The compliance state of the setting.</span></span> <span data-ttu-id="d57c3-165">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="d57c3-165">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d57c3-166">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d57c3-166">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d57c3-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d57c3-167">DateTimeOffset</span></span>|<span data-ttu-id="d57c3-168">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="d57c3-168">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="d57c3-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="d57c3-169">Response</span></span>
<span data-ttu-id="d57c3-170">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d57c3-170">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d57c3-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d57c3-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="d57c3-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d57c3-172">Request</span></span>
<span data-ttu-id="d57c3-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d57c3-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
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

### <a name="response"></a><span data-ttu-id="d57c3-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="d57c3-174">Response</span></span>
<span data-ttu-id="d57c3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d57c3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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









