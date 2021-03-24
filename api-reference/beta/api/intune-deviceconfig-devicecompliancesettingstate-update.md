---
title: Atualizar deviceComplianceSettingState
description: Atualizar as propriedades de um objeto deviceComplianceSettingState objeto.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 39de4f02a19e514c91ba4eec21620900d0898192
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128128"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="861fd-103">Atualizar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="861fd-103">Update deviceComplianceSettingState</span></span>

<span data-ttu-id="861fd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="861fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="861fd-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="861fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="861fd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="861fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="861fd-107">Atualizar as propriedades de um objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objeto.</span><span class="sxs-lookup"><span data-stu-id="861fd-107">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="861fd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="861fd-108">Prerequisites</span></span>
<span data-ttu-id="861fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="861fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="861fd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="861fd-111">Permission type</span></span>|<span data-ttu-id="861fd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="861fd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="861fd-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="861fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="861fd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="861fd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="861fd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="861fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="861fd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="861fd-116">Not supported.</span></span>|
|<span data-ttu-id="861fd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="861fd-117">Application</span></span>|<span data-ttu-id="861fd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="861fd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="861fd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="861fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="861fd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="861fd-120">Request headers</span></span>
|<span data-ttu-id="861fd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="861fd-121">Header</span></span>|<span data-ttu-id="861fd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="861fd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="861fd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="861fd-123">Authorization</span></span>|<span data-ttu-id="861fd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="861fd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="861fd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="861fd-125">Accept</span></span>|<span data-ttu-id="861fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="861fd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="861fd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="861fd-127">Request body</span></span>
<span data-ttu-id="861fd-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="861fd-128">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="861fd-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="861fd-129">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="861fd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="861fd-130">Property</span></span>|<span data-ttu-id="861fd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="861fd-131">Type</span></span>|<span data-ttu-id="861fd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="861fd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="861fd-133">id</span><span class="sxs-lookup"><span data-stu-id="861fd-133">id</span></span>|<span data-ttu-id="861fd-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="861fd-134">String</span></span>|<span data-ttu-id="861fd-135">Chave da entidade</span><span class="sxs-lookup"><span data-stu-id="861fd-135">Key of the entity</span></span>|
|<span data-ttu-id="861fd-136">platformType</span><span class="sxs-lookup"><span data-stu-id="861fd-136">platformType</span></span>|[<span data-ttu-id="861fd-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="861fd-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="861fd-138">Tipo de plataforma de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="861fd-138">Device platform type.</span></span> <span data-ttu-id="861fd-139">Os valores possíveis são: `desktop` , , , , , , , , `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` , `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` `unknown` .</span><span class="sxs-lookup"><span data-stu-id="861fd-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `cloudPC`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="861fd-140">configuração</span><span class="sxs-lookup"><span data-stu-id="861fd-140">setting</span></span>|<span data-ttu-id="861fd-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="861fd-141">String</span></span>|<span data-ttu-id="861fd-142">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="861fd-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="861fd-143">settingName</span><span class="sxs-lookup"><span data-stu-id="861fd-143">settingName</span></span>|<span data-ttu-id="861fd-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="861fd-144">String</span></span>|<span data-ttu-id="861fd-145">O nome da configuração sendo relatada</span><span class="sxs-lookup"><span data-stu-id="861fd-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="861fd-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="861fd-146">deviceId</span></span>|<span data-ttu-id="861fd-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="861fd-147">String</span></span>|<span data-ttu-id="861fd-148">A ID do dispositivo sendo relatada</span><span class="sxs-lookup"><span data-stu-id="861fd-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="861fd-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="861fd-149">deviceName</span></span>|<span data-ttu-id="861fd-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="861fd-150">String</span></span>|<span data-ttu-id="861fd-151">O nome do dispositivo sendo relatado</span><span class="sxs-lookup"><span data-stu-id="861fd-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="861fd-152">userId</span><span class="sxs-lookup"><span data-stu-id="861fd-152">userId</span></span>|<span data-ttu-id="861fd-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="861fd-153">String</span></span>|<span data-ttu-id="861fd-154">A ID do usuário sendo relatada</span><span class="sxs-lookup"><span data-stu-id="861fd-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="861fd-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="861fd-155">userEmail</span></span>|<span data-ttu-id="861fd-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="861fd-156">String</span></span>|<span data-ttu-id="861fd-157">O endereço de email do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="861fd-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="861fd-158">userName</span><span class="sxs-lookup"><span data-stu-id="861fd-158">userName</span></span>|<span data-ttu-id="861fd-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="861fd-159">String</span></span>|<span data-ttu-id="861fd-160">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="861fd-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="861fd-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="861fd-161">userPrincipalName</span></span>|<span data-ttu-id="861fd-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="861fd-162">String</span></span>|<span data-ttu-id="861fd-163">O PrincipalName do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="861fd-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="861fd-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="861fd-164">deviceModel</span></span>|<span data-ttu-id="861fd-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="861fd-165">String</span></span>|<span data-ttu-id="861fd-166">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="861fd-166">The device model that is being reported</span></span>|
|<span data-ttu-id="861fd-167">state</span><span class="sxs-lookup"><span data-stu-id="861fd-167">state</span></span>|[<span data-ttu-id="861fd-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="861fd-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="861fd-169">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="861fd-169">The compliance state of the setting.</span></span> <span data-ttu-id="861fd-170">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="861fd-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="861fd-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="861fd-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="861fd-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="861fd-172">DateTimeOffset</span></span>|<span data-ttu-id="861fd-173">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="861fd-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="861fd-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="861fd-174">Response</span></span>
<span data-ttu-id="861fd-175">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="861fd-175">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="861fd-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="861fd-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="861fd-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="861fd-177">Request</span></span>
<span data-ttu-id="861fd-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="861fd-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
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

### <a name="response"></a><span data-ttu-id="861fd-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="861fd-179">Response</span></span>
<span data-ttu-id="861fd-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="861fd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




