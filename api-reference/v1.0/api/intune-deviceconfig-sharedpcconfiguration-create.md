---
title: Criar sharedPCConfiguration
description: Cria um novo objeto sharedPCConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 27ea8296da13cc1ef8e84637ff0a7208d865f2d0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43387565"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="a7c79-103">Criar sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7c79-103">Create sharedPCConfiguration</span></span>

<span data-ttu-id="a7c79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7c79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7c79-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a7c79-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7c79-106">Cria um novo objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7c79-106">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7c79-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a7c79-107">Prerequisites</span></span>
<span data-ttu-id="a7c79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7c79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7c79-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7c79-110">Permission type</span></span>|<span data-ttu-id="a7c79-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a7c79-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7c79-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7c79-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a7c79-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7c79-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7c79-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7c79-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7c79-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7c79-115">Not supported.</span></span>|
|<span data-ttu-id="a7c79-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7c79-116">Application</span></span>|<span data-ttu-id="a7c79-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7c79-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7c79-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7c79-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a7c79-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7c79-119">Request headers</span></span>
|<span data-ttu-id="a7c79-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a7c79-120">Header</span></span>|<span data-ttu-id="a7c79-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a7c79-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7c79-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7c79-122">Authorization</span></span>|<span data-ttu-id="a7c79-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7c79-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7c79-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a7c79-124">Accept</span></span>|<span data-ttu-id="a7c79-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a7c79-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7c79-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7c79-126">Request body</span></span>
<span data-ttu-id="a7c79-127">No corpo da solicitação, forneça uma representação JSON do objeto sharedPCConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a7c79-127">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="a7c79-128">A tabela a seguir mostra as propriedades que são necessárias ao criar sharedPCConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a7c79-128">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="a7c79-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7c79-129">Property</span></span>|<span data-ttu-id="a7c79-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7c79-130">Type</span></span>|<span data-ttu-id="a7c79-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7c79-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7c79-132">id</span><span class="sxs-lookup"><span data-stu-id="a7c79-132">id</span></span>|<span data-ttu-id="a7c79-133">String</span><span class="sxs-lookup"><span data-stu-id="a7c79-133">String</span></span>|<span data-ttu-id="a7c79-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a7c79-134">Key of the entity.</span></span> <span data-ttu-id="a7c79-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7c79-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7c79-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7c79-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a7c79-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7c79-137">DateTimeOffset</span></span>|<span data-ttu-id="a7c79-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a7c79-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a7c79-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7c79-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7c79-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7c79-140">createdDateTime</span></span>|<span data-ttu-id="a7c79-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7c79-141">DateTimeOffset</span></span>|<span data-ttu-id="a7c79-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a7c79-142">DateTime the object was created.</span></span> <span data-ttu-id="a7c79-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7c79-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7c79-144">description</span><span class="sxs-lookup"><span data-stu-id="a7c79-144">description</span></span>|<span data-ttu-id="a7c79-145">String</span><span class="sxs-lookup"><span data-stu-id="a7c79-145">String</span></span>|<span data-ttu-id="a7c79-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a7c79-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a7c79-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7c79-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7c79-148">displayName</span><span class="sxs-lookup"><span data-stu-id="a7c79-148">displayName</span></span>|<span data-ttu-id="a7c79-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7c79-149">String</span></span>|<span data-ttu-id="a7c79-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a7c79-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a7c79-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7c79-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7c79-152">versão</span><span class="sxs-lookup"><span data-stu-id="a7c79-152">version</span></span>|<span data-ttu-id="a7c79-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a7c79-153">Int32</span></span>|<span data-ttu-id="a7c79-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a7c79-154">Version of the device configuration.</span></span> <span data-ttu-id="a7c79-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7c79-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7c79-156">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="a7c79-156">accountManagerPolicy</span></span>|[<span data-ttu-id="a7c79-157">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="a7c79-157">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="a7c79-158">Especifica como as contas são gerenciadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="a7c79-158">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="a7c79-159">Aplica-se somente quando disableAccountManager é false.</span><span class="sxs-lookup"><span data-stu-id="a7c79-159">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="a7c79-160">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="a7c79-160">allowedAccounts</span></span>|[<span data-ttu-id="a7c79-161">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="a7c79-161">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="a7c79-162">Indica que tipos de contas podem ser usadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="a7c79-162">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="a7c79-163">Os valores possíveis são: `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="a7c79-163">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="a7c79-164">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="a7c79-164">allowLocalStorage</span></span>|<span data-ttu-id="a7c79-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="a7c79-165">Boolean</span></span>|<span data-ttu-id="a7c79-166">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="a7c79-166">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="a7c79-167">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="a7c79-167">disableAccountManager</span></span>|<span data-ttu-id="a7c79-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="a7c79-168">Boolean</span></span>|<span data-ttu-id="a7c79-169">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="a7c79-169">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="a7c79-170">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="a7c79-170">disableEduPolicies</span></span>|<span data-ttu-id="a7c79-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="a7c79-171">Boolean</span></span>|<span data-ttu-id="a7c79-172">Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="a7c79-172">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="a7c79-173">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="a7c79-173">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="a7c79-174">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="a7c79-174">disablePowerPolicies</span></span>|<span data-ttu-id="a7c79-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="a7c79-175">Boolean</span></span>|<span data-ttu-id="a7c79-176">Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="a7c79-176">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="a7c79-177">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="a7c79-177">disableSignInOnResume</span></span>|<span data-ttu-id="a7c79-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="a7c79-178">Boolean</span></span>|<span data-ttu-id="a7c79-179">Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="a7c79-179">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="a7c79-180">enabled</span><span class="sxs-lookup"><span data-stu-id="a7c79-180">enabled</span></span>|<span data-ttu-id="a7c79-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7c79-181">Boolean</span></span>|<span data-ttu-id="a7c79-182">Habilita o modo de PC compartilhado e aplica as políticas de PC compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="a7c79-182">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="a7c79-183">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="a7c79-183">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="a7c79-184">Int32</span><span class="sxs-lookup"><span data-stu-id="a7c79-184">Int32</span></span>|<span data-ttu-id="a7c79-185">Especifica o tempo em segundos que um dispositivo deve ficar ocioso antes de o PC entrar em suspensão.</span><span class="sxs-lookup"><span data-stu-id="a7c79-185">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="a7c79-186">Definir esse valor como 0 impede que o tempo limite de suspensão ocorra.</span><span class="sxs-lookup"><span data-stu-id="a7c79-186">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="a7c79-187">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="a7c79-187">kioskAppDisplayName</span></span>|<span data-ttu-id="a7c79-188">String</span><span class="sxs-lookup"><span data-stu-id="a7c79-188">String</span></span>|<span data-ttu-id="a7c79-189">Especifica o texto de exibição para a conta mostrada na tela de entrada que inicializa o aplicativo especificado por SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="a7c79-189">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="a7c79-190">Aplicável somente quando KioskAppUserModelId está definido.</span><span class="sxs-lookup"><span data-stu-id="a7c79-190">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="a7c79-191">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="a7c79-191">kioskAppUserModelId</span></span>|<span data-ttu-id="a7c79-192">String</span><span class="sxs-lookup"><span data-stu-id="a7c79-192">String</span></span>|<span data-ttu-id="a7c79-193">Especifica a ID do modelo de usuário do aplicativo para uso com acesso atribuído.</span><span class="sxs-lookup"><span data-stu-id="a7c79-193">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="a7c79-194">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="a7c79-194">maintenanceStartTime</span></span>|<span data-ttu-id="a7c79-195">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a7c79-195">TimeOfDay</span></span>|<span data-ttu-id="a7c79-196">Especifica o horário de início diário da hora de manutenção.</span><span class="sxs-lookup"><span data-stu-id="a7c79-196">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="a7c79-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7c79-197">Response</span></span>
<span data-ttu-id="a7c79-198">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7c79-198">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7c79-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7c79-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7c79-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7c79-200">Request</span></span>
<span data-ttu-id="a7c79-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7c79-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="a7c79-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7c79-202">Response</span></span>
<span data-ttu-id="a7c79-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7c79-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






