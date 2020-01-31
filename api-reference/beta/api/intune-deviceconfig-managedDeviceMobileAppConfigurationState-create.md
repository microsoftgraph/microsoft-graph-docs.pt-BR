---
title: Criar managedDeviceMobileAppConfigurationState
description: Criar um novo objeto managedDeviceMobileAppConfigurationState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ab87332a5dedc2aaffbae19966fce737bcbdf1b
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636044"
---
# <a name="create-manageddevicemobileappconfigurationstate"></a><span data-ttu-id="a519f-103">Criar managedDeviceMobileAppConfigurationState</span><span class="sxs-lookup"><span data-stu-id="a519f-103">Create managedDeviceMobileAppConfigurationState</span></span>

> <span data-ttu-id="a519f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a519f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a519f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a519f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a519f-106">Criar um novo objeto managedDeviceMobileAppConfigurationState.</span><span class="sxs-lookup"><span data-stu-id="a519f-106">Create a new managedDeviceMobileAppConfigurationState object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a519f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a519f-107">Prerequisites</span></span>
<span data-ttu-id="a519f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a519f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a519f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a519f-110">Permission type</span></span>|<span data-ttu-id="a519f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a519f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a519f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a519f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a519f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a519f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a519f-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a519f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a519f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a519f-115">Not supported.</span></span>|
|<span data-ttu-id="a519f-116">Application</span><span class="sxs-lookup"><span data-stu-id="a519f-116">Application</span></span>|<span data-ttu-id="a519f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a519f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a519f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a519f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/managedDeviceMobileAppConfigurationStates
```

## <a name="request-headers"></a><span data-ttu-id="a519f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a519f-119">Request headers</span></span>
|<span data-ttu-id="a519f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a519f-120">Header</span></span>|<span data-ttu-id="a519f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a519f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a519f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a519f-122">Authorization</span></span>|<span data-ttu-id="a519f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a519f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a519f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a519f-124">Accept</span></span>|<span data-ttu-id="a519f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a519f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a519f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a519f-126">Request body</span></span>
<span data-ttu-id="a519f-127">No corpo da solicitação, forneça uma representação JSON do objeto managedDeviceMobileAppConfigurationState.</span><span class="sxs-lookup"><span data-stu-id="a519f-127">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationState object.</span></span>

<span data-ttu-id="a519f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceMobileAppConfigurationState.</span><span class="sxs-lookup"><span data-stu-id="a519f-128">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationState.</span></span>

|<span data-ttu-id="a519f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a519f-129">Property</span></span>|<span data-ttu-id="a519f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a519f-130">Type</span></span>|<span data-ttu-id="a519f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a519f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a519f-132">id</span><span class="sxs-lookup"><span data-stu-id="a519f-132">id</span></span>|<span data-ttu-id="a519f-133">String</span><span class="sxs-lookup"><span data-stu-id="a519f-133">String</span></span>|<span data-ttu-id="a519f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a519f-134">Key of the entity.</span></span>|
|<span data-ttu-id="a519f-135">settingStates</span><span class="sxs-lookup"><span data-stu-id="a519f-135">settingStates</span></span>|<span data-ttu-id="a519f-136">coleção managedDeviceMobileAppConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="a519f-136">managedDeviceMobileAppConfigurationSettingState collection</span></span>|<span data-ttu-id="a519f-137">**TODO: Adicione descrição.**</span><span class="sxs-lookup"><span data-stu-id="a519f-137">**TODO: Add description.**</span></span>|
|<span data-ttu-id="a519f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="a519f-138">displayName</span></span>|<span data-ttu-id="a519f-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a519f-139">String</span></span>|<span data-ttu-id="a519f-140">O nome da política dessa policyBase</span><span class="sxs-lookup"><span data-stu-id="a519f-140">The name of the policy for this policyBase</span></span>|
|<span data-ttu-id="a519f-141">versão</span><span class="sxs-lookup"><span data-stu-id="a519f-141">version</span></span>|<span data-ttu-id="a519f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a519f-142">Int32</span></span>|<span data-ttu-id="a519f-143">A versão da política</span><span class="sxs-lookup"><span data-stu-id="a519f-143">The version of the policy</span></span>|
|<span data-ttu-id="a519f-144">platformType</span><span class="sxs-lookup"><span data-stu-id="a519f-144">platformType</span></span>|<span data-ttu-id="a519f-145">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="a519f-145">policyPlatformType</span></span>|<span data-ttu-id="a519f-146">Tipo de plataforma ao qual a política se aplica.</span><span class="sxs-lookup"><span data-stu-id="a519f-146">Platform type that the policy applies to.</span></span> <span data-ttu-id="a519f-147">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="a519f-147">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="a519f-148">state</span><span class="sxs-lookup"><span data-stu-id="a519f-148">state</span></span>|<span data-ttu-id="a519f-149">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a519f-149">complianceStatus</span></span>|<span data-ttu-id="a519f-150">O estado de conformidade da política.</span><span class="sxs-lookup"><span data-stu-id="a519f-150">The compliance state of the policy.</span></span> <span data-ttu-id="a519f-151">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a519f-151">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a519f-152">settingCount</span><span class="sxs-lookup"><span data-stu-id="a519f-152">settingCount</span></span>|<span data-ttu-id="a519f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a519f-153">Int32</span></span>|<span data-ttu-id="a519f-154">Contagem de quantas configurações uma política contém</span><span class="sxs-lookup"><span data-stu-id="a519f-154">Count of how many setting a policy holds</span></span>|
|<span data-ttu-id="a519f-155">userId</span><span class="sxs-lookup"><span data-stu-id="a519f-155">userId</span></span>|<span data-ttu-id="a519f-156">String</span><span class="sxs-lookup"><span data-stu-id="a519f-156">String</span></span>|<span data-ttu-id="a519f-157">O identificador exclusivo do usuário deve ser GUID</span><span class="sxs-lookup"><span data-stu-id="a519f-157">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="a519f-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a519f-158">userPrincipalName</span></span>|<span data-ttu-id="a519f-159">String</span><span class="sxs-lookup"><span data-stu-id="a519f-159">String</span></span>|<span data-ttu-id="a519f-160">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="a519f-160">User Principal Name</span></span>|



## <a name="response"></a><span data-ttu-id="a519f-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="a519f-161">Response</span></span>
<span data-ttu-id="a519f-162">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto managedDeviceMobileAppConfigurationState no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a519f-162">If successful, this method returns a `201 Created` response code and a managedDeviceMobileAppConfigurationState object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a519f-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a519f-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="a519f-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a519f-164">Request</span></span>
<span data-ttu-id="a519f-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a519f-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/managedDeviceMobileAppConfigurationStates
Content-type: application/json
Content-length: 1093

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationState",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "notApplicable",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "androidForWork",
  "state": "notApplicable",
  "settingCount": 12,
  "userId": "User Id value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="a519f-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="a519f-166">Response</span></span>
<span data-ttu-id="a519f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a519f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1142

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationState",
  "id": "659554f2-54f2-6595-f254-9565f2549565",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "notApplicable",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "androidForWork",
  "state": "notApplicable",
  "settingCount": 12,
  "userId": "User Id value",
  "userPrincipalName": "User Principal Name value"
}
```



