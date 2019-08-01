---
title: Atualizar deviceComplianceSettingState
description: Atualizar as propriedades de um objeto deviceComplianceSettingState objeto.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3d6e875526141cedd020b12b2032ac16edf1f754
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019258"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="30627-103">Atualizar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="30627-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="30627-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30627-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30627-105">Atualizar as propriedades de um objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objeto.</span><span class="sxs-lookup"><span data-stu-id="30627-105">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30627-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30627-106">Prerequisites</span></span>
<span data-ttu-id="30627-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30627-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30627-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30627-109">Permission type</span></span>|<span data-ttu-id="30627-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30627-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30627-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30627-111">Delegated (work or school account)</span></span>|<span data-ttu-id="30627-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30627-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="30627-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30627-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30627-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30627-114">Not supported.</span></span>|
|<span data-ttu-id="30627-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30627-115">Application</span></span>|<span data-ttu-id="30627-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30627-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30627-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30627-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="30627-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30627-118">Request headers</span></span>
|<span data-ttu-id="30627-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30627-119">Header</span></span>|<span data-ttu-id="30627-120">Valor</span><span class="sxs-lookup"><span data-stu-id="30627-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30627-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="30627-121">Authorization</span></span>|<span data-ttu-id="30627-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30627-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30627-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30627-123">Accept</span></span>|<span data-ttu-id="30627-124">application/json</span><span class="sxs-lookup"><span data-stu-id="30627-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30627-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30627-125">Request body</span></span>
<span data-ttu-id="30627-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="30627-126">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="30627-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="30627-127">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="30627-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30627-128">Property</span></span>|<span data-ttu-id="30627-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="30627-129">Type</span></span>|<span data-ttu-id="30627-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="30627-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30627-131">id</span><span class="sxs-lookup"><span data-stu-id="30627-131">id</span></span>|<span data-ttu-id="30627-132">String</span><span class="sxs-lookup"><span data-stu-id="30627-132">String</span></span>|<span data-ttu-id="30627-133">Chave da entidade</span><span class="sxs-lookup"><span data-stu-id="30627-133">Key of the entity</span></span>|
|<span data-ttu-id="30627-134">configuração</span><span class="sxs-lookup"><span data-stu-id="30627-134">setting</span></span>|<span data-ttu-id="30627-135">String</span><span class="sxs-lookup"><span data-stu-id="30627-135">String</span></span>|<span data-ttu-id="30627-136">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="30627-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="30627-137">settingName</span><span class="sxs-lookup"><span data-stu-id="30627-137">settingName</span></span>|<span data-ttu-id="30627-138">String</span><span class="sxs-lookup"><span data-stu-id="30627-138">String</span></span>|<span data-ttu-id="30627-139">O nome da configuração sendo relatada</span><span class="sxs-lookup"><span data-stu-id="30627-139">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="30627-140">deviceId</span><span class="sxs-lookup"><span data-stu-id="30627-140">deviceId</span></span>|<span data-ttu-id="30627-141">String</span><span class="sxs-lookup"><span data-stu-id="30627-141">String</span></span>|<span data-ttu-id="30627-142">A ID do dispositivo sendo relatada</span><span class="sxs-lookup"><span data-stu-id="30627-142">The Device Id that is being reported</span></span>|
|<span data-ttu-id="30627-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="30627-143">deviceName</span></span>|<span data-ttu-id="30627-144">String</span><span class="sxs-lookup"><span data-stu-id="30627-144">String</span></span>|<span data-ttu-id="30627-145">O nome do dispositivo sendo relatado</span><span class="sxs-lookup"><span data-stu-id="30627-145">The Device Name that is being reported</span></span>|
|<span data-ttu-id="30627-146">userId</span><span class="sxs-lookup"><span data-stu-id="30627-146">userId</span></span>|<span data-ttu-id="30627-147">String</span><span class="sxs-lookup"><span data-stu-id="30627-147">String</span></span>|<span data-ttu-id="30627-148">A ID do usuário sendo relatada</span><span class="sxs-lookup"><span data-stu-id="30627-148">The user Id that is being reported</span></span>|
|<span data-ttu-id="30627-149">userEmail</span><span class="sxs-lookup"><span data-stu-id="30627-149">userEmail</span></span>|<span data-ttu-id="30627-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="30627-150">String</span></span>|<span data-ttu-id="30627-151">O endereço de email do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="30627-151">The User email address that is being reported</span></span>|
|<span data-ttu-id="30627-152">userName</span><span class="sxs-lookup"><span data-stu-id="30627-152">userName</span></span>|<span data-ttu-id="30627-153">String</span><span class="sxs-lookup"><span data-stu-id="30627-153">String</span></span>|<span data-ttu-id="30627-154">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="30627-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="30627-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="30627-155">userPrincipalName</span></span>|<span data-ttu-id="30627-156">String</span><span class="sxs-lookup"><span data-stu-id="30627-156">String</span></span>|<span data-ttu-id="30627-157">O PrincipalName do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="30627-157">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="30627-158">deviceModel</span><span class="sxs-lookup"><span data-stu-id="30627-158">deviceModel</span></span>|<span data-ttu-id="30627-159">String</span><span class="sxs-lookup"><span data-stu-id="30627-159">String</span></span>|<span data-ttu-id="30627-160">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="30627-160">The device model that is being reported</span></span>|
|<span data-ttu-id="30627-161">state</span><span class="sxs-lookup"><span data-stu-id="30627-161">state</span></span>|[<span data-ttu-id="30627-162">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="30627-162">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="30627-163">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="30627-163">The compliance state of the setting.</span></span> <span data-ttu-id="30627-164">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="30627-164">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="30627-165">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="30627-165">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="30627-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30627-166">DateTimeOffset</span></span>|<span data-ttu-id="30627-167">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="30627-167">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="30627-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="30627-168">Response</span></span>
<span data-ttu-id="30627-169">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30627-169">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30627-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30627-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="30627-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30627-171">Request</span></span>
<span data-ttu-id="30627-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30627-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="30627-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="30627-173">Response</span></span>
<span data-ttu-id="30627-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30627-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



