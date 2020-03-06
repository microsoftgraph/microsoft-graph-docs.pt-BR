---
title: Atualizar deviceComplianceSettingState
description: Atualizar as propriedades de um objeto deviceComplianceSettingState objeto.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: de5c9bf9b2f19bf60bf35391a918916dd02ca9d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514912"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="d1dda-103">Atualizar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="d1dda-103">Update deviceComplianceSettingState</span></span>

<span data-ttu-id="d1dda-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1dda-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1dda-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d1dda-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1dda-106">Atualizar as propriedades de um objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objeto.</span><span class="sxs-lookup"><span data-stu-id="d1dda-106">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1dda-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d1dda-107">Prerequisites</span></span>
<span data-ttu-id="d1dda-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1dda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1dda-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1dda-110">Permission type</span></span>|<span data-ttu-id="d1dda-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d1dda-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1dda-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1dda-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d1dda-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1dda-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1dda-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1dda-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1dda-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1dda-115">Not supported.</span></span>|
|<span data-ttu-id="d1dda-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1dda-116">Application</span></span>|<span data-ttu-id="d1dda-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1dda-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1dda-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1dda-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="d1dda-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1dda-119">Request headers</span></span>
|<span data-ttu-id="d1dda-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d1dda-120">Header</span></span>|<span data-ttu-id="d1dda-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d1dda-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1dda-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1dda-122">Authorization</span></span>|<span data-ttu-id="d1dda-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1dda-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1dda-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d1dda-124">Accept</span></span>|<span data-ttu-id="d1dda-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d1dda-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1dda-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1dda-126">Request body</span></span>
<span data-ttu-id="d1dda-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="d1dda-127">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="d1dda-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="d1dda-128">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="d1dda-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1dda-129">Property</span></span>|<span data-ttu-id="d1dda-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1dda-130">Type</span></span>|<span data-ttu-id="d1dda-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1dda-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1dda-132">id</span><span class="sxs-lookup"><span data-stu-id="d1dda-132">id</span></span>|<span data-ttu-id="d1dda-133">String</span><span class="sxs-lookup"><span data-stu-id="d1dda-133">String</span></span>|<span data-ttu-id="d1dda-134">Chave da entidade</span><span class="sxs-lookup"><span data-stu-id="d1dda-134">Key of the entity</span></span>|
|<span data-ttu-id="d1dda-135">configuração</span><span class="sxs-lookup"><span data-stu-id="d1dda-135">setting</span></span>|<span data-ttu-id="d1dda-136">String</span><span class="sxs-lookup"><span data-stu-id="d1dda-136">String</span></span>|<span data-ttu-id="d1dda-137">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="d1dda-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="d1dda-138">settingName</span><span class="sxs-lookup"><span data-stu-id="d1dda-138">settingName</span></span>|<span data-ttu-id="d1dda-139">String</span><span class="sxs-lookup"><span data-stu-id="d1dda-139">String</span></span>|<span data-ttu-id="d1dda-140">O nome da configuração sendo relatada</span><span class="sxs-lookup"><span data-stu-id="d1dda-140">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="d1dda-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="d1dda-141">deviceId</span></span>|<span data-ttu-id="d1dda-142">String</span><span class="sxs-lookup"><span data-stu-id="d1dda-142">String</span></span>|<span data-ttu-id="d1dda-143">A ID do dispositivo sendo relatada</span><span class="sxs-lookup"><span data-stu-id="d1dda-143">The Device Id that is being reported</span></span>|
|<span data-ttu-id="d1dda-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="d1dda-144">deviceName</span></span>|<span data-ttu-id="d1dda-145">String</span><span class="sxs-lookup"><span data-stu-id="d1dda-145">String</span></span>|<span data-ttu-id="d1dda-146">O nome do dispositivo sendo relatado</span><span class="sxs-lookup"><span data-stu-id="d1dda-146">The Device Name that is being reported</span></span>|
|<span data-ttu-id="d1dda-147">userId</span><span class="sxs-lookup"><span data-stu-id="d1dda-147">userId</span></span>|<span data-ttu-id="d1dda-148">String</span><span class="sxs-lookup"><span data-stu-id="d1dda-148">String</span></span>|<span data-ttu-id="d1dda-149">A ID do usuário sendo relatada</span><span class="sxs-lookup"><span data-stu-id="d1dda-149">The user Id that is being reported</span></span>|
|<span data-ttu-id="d1dda-150">userEmail</span><span class="sxs-lookup"><span data-stu-id="d1dda-150">userEmail</span></span>|<span data-ttu-id="d1dda-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1dda-151">String</span></span>|<span data-ttu-id="d1dda-152">O endereço de email do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="d1dda-152">The User email address that is being reported</span></span>|
|<span data-ttu-id="d1dda-153">userName</span><span class="sxs-lookup"><span data-stu-id="d1dda-153">userName</span></span>|<span data-ttu-id="d1dda-154">String</span><span class="sxs-lookup"><span data-stu-id="d1dda-154">String</span></span>|<span data-ttu-id="d1dda-155">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="d1dda-155">The User Name that is being reported</span></span>|
|<span data-ttu-id="d1dda-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d1dda-156">userPrincipalName</span></span>|<span data-ttu-id="d1dda-157">String</span><span class="sxs-lookup"><span data-stu-id="d1dda-157">String</span></span>|<span data-ttu-id="d1dda-158">O PrincipalName do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="d1dda-158">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="d1dda-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="d1dda-159">deviceModel</span></span>|<span data-ttu-id="d1dda-160">String</span><span class="sxs-lookup"><span data-stu-id="d1dda-160">String</span></span>|<span data-ttu-id="d1dda-161">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="d1dda-161">The device model that is being reported</span></span>|
|<span data-ttu-id="d1dda-162">state</span><span class="sxs-lookup"><span data-stu-id="d1dda-162">state</span></span>|[<span data-ttu-id="d1dda-163">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d1dda-163">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d1dda-164">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="d1dda-164">The compliance state of the setting.</span></span> <span data-ttu-id="d1dda-165">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="d1dda-165">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d1dda-166">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d1dda-166">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d1dda-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1dda-167">DateTimeOffset</span></span>|<span data-ttu-id="d1dda-168">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="d1dda-168">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="d1dda-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1dda-169">Response</span></span>
<span data-ttu-id="d1dda-170">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1dda-170">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1dda-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1dda-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1dda-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1dda-172">Request</span></span>
<span data-ttu-id="d1dda-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1dda-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d1dda-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1dda-174">Response</span></span>
<span data-ttu-id="d1dda-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1dda-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




