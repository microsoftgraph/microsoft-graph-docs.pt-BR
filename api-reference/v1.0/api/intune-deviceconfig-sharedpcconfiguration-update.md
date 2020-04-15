---
title: Atualizar sharedPCConfiguration
description: Atualiza as propriedades de um objeto sharedPCConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e14edc0bfa3cf26f9d15dc7f4b3f3cc98d724744
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43387393"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="32f1c-103">Atualizar sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="32f1c-103">Update sharedPCConfiguration</span></span>

<span data-ttu-id="32f1c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32f1c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32f1c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="32f1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32f1c-106">Atualiza as propriedades de um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32f1c-106">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32f1c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="32f1c-107">Prerequisites</span></span>
<span data-ttu-id="32f1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32f1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32f1c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32f1c-110">Permission type</span></span>|<span data-ttu-id="32f1c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="32f1c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32f1c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32f1c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32f1c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32f1c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="32f1c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32f1c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32f1c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32f1c-115">Not supported.</span></span>|
|<span data-ttu-id="32f1c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32f1c-116">Application</span></span>|<span data-ttu-id="32f1c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32f1c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32f1c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32f1c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="32f1c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32f1c-119">Request headers</span></span>
|<span data-ttu-id="32f1c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32f1c-120">Header</span></span>|<span data-ttu-id="32f1c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="32f1c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32f1c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="32f1c-122">Authorization</span></span>|<span data-ttu-id="32f1c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32f1c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32f1c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="32f1c-124">Accept</span></span>|<span data-ttu-id="32f1c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="32f1c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32f1c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32f1c-126">Request body</span></span>
<span data-ttu-id="32f1c-127">No corpo da solicitação, forneça uma representação JSON do objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32f1c-127">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="32f1c-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32f1c-128">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="32f1c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32f1c-129">Property</span></span>|<span data-ttu-id="32f1c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="32f1c-130">Type</span></span>|<span data-ttu-id="32f1c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="32f1c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32f1c-132">id</span><span class="sxs-lookup"><span data-stu-id="32f1c-132">id</span></span>|<span data-ttu-id="32f1c-133">String</span><span class="sxs-lookup"><span data-stu-id="32f1c-133">String</span></span>|<span data-ttu-id="32f1c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="32f1c-134">Key of the entity.</span></span> <span data-ttu-id="32f1c-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="32f1c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32f1c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32f1c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="32f1c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32f1c-137">DateTimeOffset</span></span>|<span data-ttu-id="32f1c-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="32f1c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="32f1c-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="32f1c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32f1c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32f1c-140">createdDateTime</span></span>|<span data-ttu-id="32f1c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32f1c-141">DateTimeOffset</span></span>|<span data-ttu-id="32f1c-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="32f1c-142">DateTime the object was created.</span></span> <span data-ttu-id="32f1c-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="32f1c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32f1c-144">description</span><span class="sxs-lookup"><span data-stu-id="32f1c-144">description</span></span>|<span data-ttu-id="32f1c-145">String</span><span class="sxs-lookup"><span data-stu-id="32f1c-145">String</span></span>|<span data-ttu-id="32f1c-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="32f1c-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="32f1c-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="32f1c-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32f1c-148">displayName</span><span class="sxs-lookup"><span data-stu-id="32f1c-148">displayName</span></span>|<span data-ttu-id="32f1c-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32f1c-149">String</span></span>|<span data-ttu-id="32f1c-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="32f1c-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="32f1c-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="32f1c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32f1c-152">versão</span><span class="sxs-lookup"><span data-stu-id="32f1c-152">version</span></span>|<span data-ttu-id="32f1c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="32f1c-153">Int32</span></span>|<span data-ttu-id="32f1c-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="32f1c-154">Version of the device configuration.</span></span> <span data-ttu-id="32f1c-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="32f1c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32f1c-156">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="32f1c-156">accountManagerPolicy</span></span>|[<span data-ttu-id="32f1c-157">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="32f1c-157">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="32f1c-158">Especifica como as contas são gerenciadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="32f1c-158">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="32f1c-159">Aplica-se somente quando disableAccountManager é false.</span><span class="sxs-lookup"><span data-stu-id="32f1c-159">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="32f1c-160">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="32f1c-160">allowedAccounts</span></span>|[<span data-ttu-id="32f1c-161">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="32f1c-161">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="32f1c-162">Indica que tipos de contas podem ser usadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="32f1c-162">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="32f1c-163">Os valores possíveis são: `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="32f1c-163">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="32f1c-164">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="32f1c-164">allowLocalStorage</span></span>|<span data-ttu-id="32f1c-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="32f1c-165">Boolean</span></span>|<span data-ttu-id="32f1c-166">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="32f1c-166">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="32f1c-167">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="32f1c-167">disableAccountManager</span></span>|<span data-ttu-id="32f1c-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="32f1c-168">Boolean</span></span>|<span data-ttu-id="32f1c-169">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="32f1c-169">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="32f1c-170">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="32f1c-170">disableEduPolicies</span></span>|<span data-ttu-id="32f1c-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="32f1c-171">Boolean</span></span>|<span data-ttu-id="32f1c-172">Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="32f1c-172">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="32f1c-173">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="32f1c-173">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="32f1c-174">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="32f1c-174">disablePowerPolicies</span></span>|<span data-ttu-id="32f1c-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="32f1c-175">Boolean</span></span>|<span data-ttu-id="32f1c-176">Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="32f1c-176">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="32f1c-177">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="32f1c-177">disableSignInOnResume</span></span>|<span data-ttu-id="32f1c-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="32f1c-178">Boolean</span></span>|<span data-ttu-id="32f1c-179">Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="32f1c-179">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="32f1c-180">enabled</span><span class="sxs-lookup"><span data-stu-id="32f1c-180">enabled</span></span>|<span data-ttu-id="32f1c-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="32f1c-181">Boolean</span></span>|<span data-ttu-id="32f1c-182">Habilita o modo de PC compartilhado e aplica as políticas de PC compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="32f1c-182">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="32f1c-183">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="32f1c-183">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="32f1c-184">Int32</span><span class="sxs-lookup"><span data-stu-id="32f1c-184">Int32</span></span>|<span data-ttu-id="32f1c-185">Especifica o tempo em segundos que um dispositivo deve ficar ocioso antes de o PC entrar em suspensão.</span><span class="sxs-lookup"><span data-stu-id="32f1c-185">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="32f1c-186">Definir esse valor como 0 impede que o tempo limite de suspensão ocorra.</span><span class="sxs-lookup"><span data-stu-id="32f1c-186">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="32f1c-187">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="32f1c-187">kioskAppDisplayName</span></span>|<span data-ttu-id="32f1c-188">String</span><span class="sxs-lookup"><span data-stu-id="32f1c-188">String</span></span>|<span data-ttu-id="32f1c-189">Especifica o texto de exibição para a conta mostrada na tela de entrada que inicializa o aplicativo especificado por SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="32f1c-189">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="32f1c-190">Aplicável somente quando KioskAppUserModelId está definido.</span><span class="sxs-lookup"><span data-stu-id="32f1c-190">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="32f1c-191">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="32f1c-191">kioskAppUserModelId</span></span>|<span data-ttu-id="32f1c-192">String</span><span class="sxs-lookup"><span data-stu-id="32f1c-192">String</span></span>|<span data-ttu-id="32f1c-193">Especifica a ID do modelo de usuário do aplicativo para uso com acesso atribuído.</span><span class="sxs-lookup"><span data-stu-id="32f1c-193">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="32f1c-194">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="32f1c-194">maintenanceStartTime</span></span>|<span data-ttu-id="32f1c-195">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="32f1c-195">TimeOfDay</span></span>|<span data-ttu-id="32f1c-196">Especifica o horário de início diário da hora de manutenção.</span><span class="sxs-lookup"><span data-stu-id="32f1c-196">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="32f1c-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="32f1c-197">Response</span></span>
<span data-ttu-id="32f1c-198">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32f1c-198">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32f1c-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32f1c-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="32f1c-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32f1c-200">Request</span></span>
<span data-ttu-id="32f1c-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32f1c-201">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 860

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```

### <a name="response"></a><span data-ttu-id="32f1c-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="32f1c-202">Response</span></span>
<span data-ttu-id="32f1c-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32f1c-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1032

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```






