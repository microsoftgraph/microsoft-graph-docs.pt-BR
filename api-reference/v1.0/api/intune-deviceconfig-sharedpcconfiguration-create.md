---
title: Criar sharedPCConfiguration
description: Cria um novo objeto sharedPCConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a3d41a49530719d574b3754e360bf72c06f9d80
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038596"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="1b8df-103">Criar sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="1b8df-103">Create sharedPCConfiguration</span></span>

<span data-ttu-id="1b8df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b8df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b8df-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1b8df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b8df-106">Cria um novo objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b8df-106">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b8df-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1b8df-107">Prerequisites</span></span>
<span data-ttu-id="1b8df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b8df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b8df-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b8df-110">Permission type</span></span>|<span data-ttu-id="1b8df-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1b8df-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b8df-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b8df-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1b8df-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b8df-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1b8df-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b8df-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b8df-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b8df-115">Not supported.</span></span>|
|<span data-ttu-id="1b8df-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b8df-116">Application</span></span>|<span data-ttu-id="1b8df-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b8df-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b8df-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b8df-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1b8df-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b8df-119">Request headers</span></span>
|<span data-ttu-id="1b8df-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1b8df-120">Header</span></span>|<span data-ttu-id="1b8df-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1b8df-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b8df-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b8df-122">Authorization</span></span>|<span data-ttu-id="1b8df-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b8df-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b8df-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1b8df-124">Accept</span></span>|<span data-ttu-id="1b8df-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1b8df-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b8df-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b8df-126">Request body</span></span>
<span data-ttu-id="1b8df-127">No corpo da solicitação, forneça uma representação JSON do objeto sharedPCConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1b8df-127">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="1b8df-128">A tabela a seguir mostra as propriedades que são necessárias ao criar sharedPCConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1b8df-128">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="1b8df-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b8df-129">Property</span></span>|<span data-ttu-id="1b8df-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b8df-130">Type</span></span>|<span data-ttu-id="1b8df-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b8df-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b8df-132">id</span><span class="sxs-lookup"><span data-stu-id="1b8df-132">id</span></span>|<span data-ttu-id="1b8df-133">String</span><span class="sxs-lookup"><span data-stu-id="1b8df-133">String</span></span>|<span data-ttu-id="1b8df-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1b8df-134">Key of the entity.</span></span> <span data-ttu-id="1b8df-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b8df-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b8df-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b8df-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1b8df-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b8df-137">DateTimeOffset</span></span>|<span data-ttu-id="1b8df-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1b8df-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1b8df-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b8df-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b8df-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b8df-140">createdDateTime</span></span>|<span data-ttu-id="1b8df-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b8df-141">DateTimeOffset</span></span>|<span data-ttu-id="1b8df-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1b8df-142">DateTime the object was created.</span></span> <span data-ttu-id="1b8df-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b8df-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b8df-144">description</span><span class="sxs-lookup"><span data-stu-id="1b8df-144">description</span></span>|<span data-ttu-id="1b8df-145">String</span><span class="sxs-lookup"><span data-stu-id="1b8df-145">String</span></span>|<span data-ttu-id="1b8df-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1b8df-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1b8df-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b8df-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b8df-148">displayName</span><span class="sxs-lookup"><span data-stu-id="1b8df-148">displayName</span></span>|<span data-ttu-id="1b8df-149">String</span><span class="sxs-lookup"><span data-stu-id="1b8df-149">String</span></span>|<span data-ttu-id="1b8df-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1b8df-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1b8df-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b8df-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b8df-152">versão</span><span class="sxs-lookup"><span data-stu-id="1b8df-152">version</span></span>|<span data-ttu-id="1b8df-153">Int32</span><span class="sxs-lookup"><span data-stu-id="1b8df-153">Int32</span></span>|<span data-ttu-id="1b8df-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1b8df-154">Version of the device configuration.</span></span> <span data-ttu-id="1b8df-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b8df-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b8df-156">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="1b8df-156">accountManagerPolicy</span></span>|[<span data-ttu-id="1b8df-157">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="1b8df-157">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="1b8df-158">Especifica como as contas são gerenciadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="1b8df-158">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="1b8df-159">Aplica-se somente quando disableAccountManager é false.</span><span class="sxs-lookup"><span data-stu-id="1b8df-159">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="1b8df-160">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="1b8df-160">allowedAccounts</span></span>|[<span data-ttu-id="1b8df-161">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="1b8df-161">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="1b8df-162">Indica que tipos de contas podem ser usadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="1b8df-162">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="1b8df-163">Os valores possíveis são: `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="1b8df-163">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="1b8df-164">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="1b8df-164">allowLocalStorage</span></span>|<span data-ttu-id="1b8df-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b8df-165">Boolean</span></span>|<span data-ttu-id="1b8df-166">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="1b8df-166">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="1b8df-167">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="1b8df-167">disableAccountManager</span></span>|<span data-ttu-id="1b8df-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b8df-168">Boolean</span></span>|<span data-ttu-id="1b8df-169">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="1b8df-169">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="1b8df-170">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="1b8df-170">disableEduPolicies</span></span>|<span data-ttu-id="1b8df-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b8df-171">Boolean</span></span>|<span data-ttu-id="1b8df-172">Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="1b8df-172">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="1b8df-173">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="1b8df-173">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="1b8df-174">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="1b8df-174">disablePowerPolicies</span></span>|<span data-ttu-id="1b8df-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b8df-175">Boolean</span></span>|<span data-ttu-id="1b8df-176">Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="1b8df-176">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="1b8df-177">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="1b8df-177">disableSignInOnResume</span></span>|<span data-ttu-id="1b8df-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b8df-178">Boolean</span></span>|<span data-ttu-id="1b8df-179">Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="1b8df-179">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="1b8df-180">enabled</span><span class="sxs-lookup"><span data-stu-id="1b8df-180">enabled</span></span>|<span data-ttu-id="1b8df-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b8df-181">Boolean</span></span>|<span data-ttu-id="1b8df-182">Habilita o modo de PC compartilhado e aplica as políticas de PC compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="1b8df-182">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="1b8df-183">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="1b8df-183">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="1b8df-184">Int32</span><span class="sxs-lookup"><span data-stu-id="1b8df-184">Int32</span></span>|<span data-ttu-id="1b8df-185">Especifica o tempo em segundos que um dispositivo deve ficar ocioso antes de o PC entrar em suspensão.</span><span class="sxs-lookup"><span data-stu-id="1b8df-185">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="1b8df-186">Definir esse valor como 0 impede que o tempo limite de suspensão ocorra.</span><span class="sxs-lookup"><span data-stu-id="1b8df-186">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="1b8df-187">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="1b8df-187">kioskAppDisplayName</span></span>|<span data-ttu-id="1b8df-188">String</span><span class="sxs-lookup"><span data-stu-id="1b8df-188">String</span></span>|<span data-ttu-id="1b8df-189">Especifica o texto de exibição para a conta mostrada na tela de entrada que inicializa o aplicativo especificado por SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="1b8df-189">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="1b8df-190">Aplicável somente quando KioskAppUserModelId está definido.</span><span class="sxs-lookup"><span data-stu-id="1b8df-190">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="1b8df-191">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="1b8df-191">kioskAppUserModelId</span></span>|<span data-ttu-id="1b8df-192">String</span><span class="sxs-lookup"><span data-stu-id="1b8df-192">String</span></span>|<span data-ttu-id="1b8df-193">Especifica a ID do modelo de usuário do aplicativo para uso com acesso atribuído.</span><span class="sxs-lookup"><span data-stu-id="1b8df-193">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="1b8df-194">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="1b8df-194">maintenanceStartTime</span></span>|<span data-ttu-id="1b8df-195">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1b8df-195">TimeOfDay</span></span>|<span data-ttu-id="1b8df-196">Especifica o horário de início diário da hora de manutenção.</span><span class="sxs-lookup"><span data-stu-id="1b8df-196">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="1b8df-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b8df-197">Response</span></span>
<span data-ttu-id="1b8df-198">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b8df-198">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b8df-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b8df-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b8df-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b8df-200">Request</span></span>
<span data-ttu-id="1b8df-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b8df-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1b8df-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b8df-202">Response</span></span>
<span data-ttu-id="1b8df-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b8df-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









