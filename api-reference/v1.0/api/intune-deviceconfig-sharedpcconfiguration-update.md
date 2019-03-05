---
title: Atualizar sharedPCConfiguration
description: Atualiza as propriedades de um objeto sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f1162374198cb4bf960e28e34fab9fd7de161faf
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259413"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="cc4e4-103">Atualizar sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="cc4e4-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="cc4e4-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc4e4-105">Atualiza as propriedades de um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc4e4-105">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc4e4-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cc4e4-106">Prerequisites</span></span>
<span data-ttu-id="cc4e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cc4e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cc4e4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc4e4-109">Permission type</span></span>|<span data-ttu-id="cc4e4-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cc4e4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc4e4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc4e4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cc4e4-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc4e4-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cc4e4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc4e4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc4e4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-114">Not supported.</span></span>|
|<span data-ttu-id="cc4e4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc4e4-115">Application</span></span>|<span data-ttu-id="cc4e4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc4e4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc4e4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cc4e4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc4e4-118">Request headers</span></span>
|<span data-ttu-id="cc4e4-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc4e4-119">Header</span></span>|<span data-ttu-id="cc4e4-120">Valor</span><span class="sxs-lookup"><span data-stu-id="cc4e4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc4e4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc4e4-121">Authorization</span></span>|<span data-ttu-id="cc4e4-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc4e4-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cc4e4-123">Accept</span></span>|<span data-ttu-id="cc4e4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cc4e4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc4e4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc4e4-125">Request body</span></span>
<span data-ttu-id="cc4e4-126">No corpo da solicitação, forneça uma representação JSON do objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc4e4-126">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="cc4e4-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc4e4-127">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="cc4e4-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc4e4-128">Property</span></span>|<span data-ttu-id="cc4e4-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc4e4-129">Type</span></span>|<span data-ttu-id="cc4e4-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc4e4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc4e4-131">id</span><span class="sxs-lookup"><span data-stu-id="cc4e4-131">id</span></span>|<span data-ttu-id="cc4e4-132">String</span><span class="sxs-lookup"><span data-stu-id="cc4e4-132">String</span></span>|<span data-ttu-id="cc4e4-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-133">Key of the entity.</span></span> <span data-ttu-id="cc4e4-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc4e4-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc4e4-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc4e4-135">lastModifiedDateTime</span></span>|<span data-ttu-id="cc4e4-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc4e4-136">DateTimeOffset</span></span>|<span data-ttu-id="cc4e4-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-137">DateTime the object was last modified.</span></span> <span data-ttu-id="cc4e4-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc4e4-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc4e4-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc4e4-139">createdDateTime</span></span>|<span data-ttu-id="cc4e4-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc4e4-140">DateTimeOffset</span></span>|<span data-ttu-id="cc4e4-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-141">DateTime the object was created.</span></span> <span data-ttu-id="cc4e4-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc4e4-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc4e4-143">description</span><span class="sxs-lookup"><span data-stu-id="cc4e4-143">description</span></span>|<span data-ttu-id="cc4e4-144">String</span><span class="sxs-lookup"><span data-stu-id="cc4e4-144">String</span></span>|<span data-ttu-id="cc4e4-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cc4e4-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc4e4-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc4e4-147">displayName</span><span class="sxs-lookup"><span data-stu-id="cc4e4-147">displayName</span></span>|<span data-ttu-id="cc4e4-148">String</span><span class="sxs-lookup"><span data-stu-id="cc4e4-148">String</span></span>|<span data-ttu-id="cc4e4-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cc4e4-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc4e4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc4e4-151">version</span><span class="sxs-lookup"><span data-stu-id="cc4e4-151">version</span></span>|<span data-ttu-id="cc4e4-152">Int32</span><span class="sxs-lookup"><span data-stu-id="cc4e4-152">Int32</span></span>|<span data-ttu-id="cc4e4-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-153">Version of the device configuration.</span></span> <span data-ttu-id="cc4e4-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc4e4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc4e4-155">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="cc4e4-155">accountManagerPolicy</span></span>|[<span data-ttu-id="cc4e4-156">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="cc4e4-156">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="cc4e4-157">Especifica como as contas são gerenciadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-157">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="cc4e4-158">Aplica-se somente quando disableAccountManager é false.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-158">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="cc4e4-159">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="cc4e4-159">allowedAccounts</span></span>|[<span data-ttu-id="cc4e4-160">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="cc4e4-160">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="cc4e4-161">Indica que tipos de contas podem ser usadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-161">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="cc4e4-162">Os valores possíveis são: `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-162">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="cc4e4-163">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="cc4e4-163">allowLocalStorage</span></span>|<span data-ttu-id="cc4e4-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc4e4-164">Boolean</span></span>|<span data-ttu-id="cc4e4-165">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-165">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="cc4e4-166">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="cc4e4-166">disableAccountManager</span></span>|<span data-ttu-id="cc4e4-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc4e4-167">Boolean</span></span>|<span data-ttu-id="cc4e4-168">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-168">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="cc4e4-169">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="cc4e4-169">disableEduPolicies</span></span>|<span data-ttu-id="cc4e4-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc4e4-170">Boolean</span></span>|<span data-ttu-id="cc4e4-171">Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-171">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="cc4e4-172">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-172">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="cc4e4-173">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="cc4e4-173">disablePowerPolicies</span></span>|<span data-ttu-id="cc4e4-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc4e4-174">Boolean</span></span>|<span data-ttu-id="cc4e4-175">Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-175">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="cc4e4-176">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="cc4e4-176">disableSignInOnResume</span></span>|<span data-ttu-id="cc4e4-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="cc4e4-177">Boolean</span></span>|<span data-ttu-id="cc4e4-178">Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-178">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="cc4e4-179">enabled</span><span class="sxs-lookup"><span data-stu-id="cc4e4-179">enabled</span></span>|<span data-ttu-id="cc4e4-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc4e4-180">Boolean</span></span>|<span data-ttu-id="cc4e4-181">Habilita o modo de PC compartilhado e aplica as políticas de PC compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-181">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="cc4e4-182">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="cc4e4-182">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="cc4e4-183">Int32</span><span class="sxs-lookup"><span data-stu-id="cc4e4-183">Int32</span></span>|<span data-ttu-id="cc4e4-184">Especifica o tempo em segundos que um dispositivo deve ficar ocioso antes de o PC entrar em suspensão.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-184">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="cc4e4-185">Definir esse valor como 0 impede que o tempo limite de suspensão ocorra.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-185">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="cc4e4-186">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="cc4e4-186">kioskAppDisplayName</span></span>|<span data-ttu-id="cc4e4-187">String</span><span class="sxs-lookup"><span data-stu-id="cc4e4-187">String</span></span>|<span data-ttu-id="cc4e4-188">Especifica o texto de exibição para a conta mostrada na tela de entrada que inicializa o aplicativo especificado por SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-188">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="cc4e4-189">Aplicável somente quando KioskAppUserModelId está definido.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-189">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="cc4e4-190">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="cc4e4-190">kioskAppUserModelId</span></span>|<span data-ttu-id="cc4e4-191">String</span><span class="sxs-lookup"><span data-stu-id="cc4e4-191">String</span></span>|<span data-ttu-id="cc4e4-192">Especifica a ID do modelo de usuário do aplicativo para uso com acesso atribuído.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-192">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="cc4e4-193">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="cc4e4-193">maintenanceStartTime</span></span>|<span data-ttu-id="cc4e4-194">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="cc4e4-194">TimeOfDay</span></span>|<span data-ttu-id="cc4e4-195">Especifica o horário de início diário da hora de manutenção.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-195">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="cc4e4-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc4e4-196">Response</span></span>
<span data-ttu-id="cc4e4-197">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-197">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc4e4-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc4e4-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc4e4-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc4e4-199">Request</span></span>
<span data-ttu-id="cc4e4-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cc4e4-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc4e4-201">Response</span></span>
<span data-ttu-id="cc4e4-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc4e4-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



