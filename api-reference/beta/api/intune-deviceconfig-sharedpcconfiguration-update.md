---
title: Atualizar sharedPCConfiguration
description: Atualiza as propriedades de um objeto sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ecc5c3cbb7d63195fc832177a391231a051d77fb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792178"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="16210-103">Atualizar sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="16210-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="16210-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="16210-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16210-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="16210-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16210-106">Atualiza as propriedades de um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16210-106">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16210-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="16210-107">Prerequisites</span></span>
<span data-ttu-id="16210-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16210-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16210-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16210-110">Permission type</span></span>|<span data-ttu-id="16210-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="16210-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16210-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16210-112">Delegated (work or school account)</span></span>|<span data-ttu-id="16210-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16210-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16210-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16210-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16210-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16210-115">Not supported.</span></span>|
|<span data-ttu-id="16210-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16210-116">Application</span></span>|<span data-ttu-id="16210-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16210-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16210-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16210-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="16210-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16210-119">Request headers</span></span>
|<span data-ttu-id="16210-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16210-120">Header</span></span>|<span data-ttu-id="16210-121">Valor</span><span class="sxs-lookup"><span data-stu-id="16210-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16210-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="16210-122">Authorization</span></span>|<span data-ttu-id="16210-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16210-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16210-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="16210-124">Accept</span></span>|<span data-ttu-id="16210-125">application/json</span><span class="sxs-lookup"><span data-stu-id="16210-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16210-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16210-126">Request body</span></span>
<span data-ttu-id="16210-127">No corpo da solicitação, forneça uma representação JSON do objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16210-127">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="16210-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16210-128">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="16210-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16210-129">Property</span></span>|<span data-ttu-id="16210-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="16210-130">Type</span></span>|<span data-ttu-id="16210-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="16210-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16210-132">id</span><span class="sxs-lookup"><span data-stu-id="16210-132">id</span></span>|<span data-ttu-id="16210-133">String</span><span class="sxs-lookup"><span data-stu-id="16210-133">String</span></span>|<span data-ttu-id="16210-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="16210-134">Key of the entity.</span></span> <span data-ttu-id="16210-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16210-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16210-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16210-136">lastModifiedDateTime</span></span>|<span data-ttu-id="16210-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16210-137">DateTimeOffset</span></span>|<span data-ttu-id="16210-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="16210-138">DateTime the object was last modified.</span></span> <span data-ttu-id="16210-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16210-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16210-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="16210-140">roleScopeTagIds</span></span>|<span data-ttu-id="16210-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="16210-141">String collection</span></span>|<span data-ttu-id="16210-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="16210-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="16210-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16210-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16210-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="16210-144">supportsScopeTags</span></span>|<span data-ttu-id="16210-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="16210-145">Boolean</span></span>|<span data-ttu-id="16210-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="16210-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="16210-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="16210-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="16210-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="16210-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="16210-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="16210-149">This property is read-only.</span></span> <span data-ttu-id="16210-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16210-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16210-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16210-151">createdDateTime</span></span>|<span data-ttu-id="16210-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16210-152">DateTimeOffset</span></span>|<span data-ttu-id="16210-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="16210-153">DateTime the object was created.</span></span> <span data-ttu-id="16210-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16210-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16210-155">description</span><span class="sxs-lookup"><span data-stu-id="16210-155">description</span></span>|<span data-ttu-id="16210-156">String</span><span class="sxs-lookup"><span data-stu-id="16210-156">String</span></span>|<span data-ttu-id="16210-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16210-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="16210-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16210-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16210-159">displayName</span><span class="sxs-lookup"><span data-stu-id="16210-159">displayName</span></span>|<span data-ttu-id="16210-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16210-160">String</span></span>|<span data-ttu-id="16210-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16210-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="16210-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16210-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16210-163">versão</span><span class="sxs-lookup"><span data-stu-id="16210-163">version</span></span>|<span data-ttu-id="16210-164">Int32</span><span class="sxs-lookup"><span data-stu-id="16210-164">Int32</span></span>|<span data-ttu-id="16210-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16210-165">Version of the device configuration.</span></span> <span data-ttu-id="16210-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16210-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16210-167">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="16210-167">accountManagerPolicy</span></span>|[<span data-ttu-id="16210-168">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="16210-168">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="16210-169">Especifica como as contas são gerenciadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="16210-169">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="16210-170">Aplica-se somente quando disableAccountManager é false.</span><span class="sxs-lookup"><span data-stu-id="16210-170">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="16210-171">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="16210-171">allowedAccounts</span></span>|[<span data-ttu-id="16210-172">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="16210-172">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="16210-173">Indica que tipos de contas podem ser usadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="16210-173">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="16210-174">Os valores possíveis são: `notConfigured`, `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="16210-174">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="16210-175">localStorage</span><span class="sxs-lookup"><span data-stu-id="16210-175">localStorage</span></span>|[<span data-ttu-id="16210-176">habilitação</span><span class="sxs-lookup"><span data-stu-id="16210-176">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="16210-177">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="16210-177">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="16210-178">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="16210-178">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="16210-179">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="16210-179">allowLocalStorage</span></span>|<span data-ttu-id="16210-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="16210-180">Boolean</span></span>|<span data-ttu-id="16210-181">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="16210-181">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="16210-182">setAccountmanager</span><span class="sxs-lookup"><span data-stu-id="16210-182">setAccountManager</span></span>|[<span data-ttu-id="16210-183">habilitação</span><span class="sxs-lookup"><span data-stu-id="16210-183">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="16210-184">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="16210-184">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="16210-185">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="16210-185">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="16210-186">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="16210-186">disableAccountManager</span></span>|<span data-ttu-id="16210-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="16210-187">Boolean</span></span>|<span data-ttu-id="16210-188">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="16210-188">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="16210-189">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="16210-189">setEduPolicies</span></span>|[<span data-ttu-id="16210-190">habilitação</span><span class="sxs-lookup"><span data-stu-id="16210-190">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="16210-191">Especifica se as políticas de ambiente de educação de computador compartilhado padrão devem ser habilitadas/desabilitadas/não configuradas.</span><span class="sxs-lookup"><span data-stu-id="16210-191">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="16210-192">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="16210-192">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="16210-193">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="16210-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="16210-194">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="16210-194">disableEduPolicies</span></span>|<span data-ttu-id="16210-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="16210-195">Boolean</span></span>|<span data-ttu-id="16210-196">Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="16210-196">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="16210-197">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="16210-197">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="16210-198">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="16210-198">setPowerPolicies</span></span>|[<span data-ttu-id="16210-199">habilitação</span><span class="sxs-lookup"><span data-stu-id="16210-199">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="16210-200">Especifica se as políticas de energia padrão do computador compartilhado devem ser ativadas/desativadas.</span><span class="sxs-lookup"><span data-stu-id="16210-200">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="16210-201">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="16210-201">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="16210-202">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="16210-202">disablePowerPolicies</span></span>|<span data-ttu-id="16210-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="16210-203">Boolean</span></span>|<span data-ttu-id="16210-204">Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="16210-204">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="16210-205">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="16210-205">signInOnResume</span></span>|[<span data-ttu-id="16210-206">habilitação</span><span class="sxs-lookup"><span data-stu-id="16210-206">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="16210-207">Especifica o requisito para entrar sempre que o dispositivo é ativado do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="16210-207">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="16210-208">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="16210-208">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="16210-209">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="16210-209">disableSignInOnResume</span></span>|<span data-ttu-id="16210-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="16210-210">Boolean</span></span>|<span data-ttu-id="16210-211">Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="16210-211">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="16210-212">enabled</span><span class="sxs-lookup"><span data-stu-id="16210-212">enabled</span></span>|<span data-ttu-id="16210-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="16210-213">Boolean</span></span>|<span data-ttu-id="16210-214">Habilita o modo de PC compartilhado e aplica as políticas de PC compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="16210-214">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="16210-215">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="16210-215">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="16210-216">Int32</span><span class="sxs-lookup"><span data-stu-id="16210-216">Int32</span></span>|<span data-ttu-id="16210-217">Especifica o tempo em segundos que um dispositivo deve ficar ocioso antes de o PC entrar em suspensão.</span><span class="sxs-lookup"><span data-stu-id="16210-217">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="16210-218">Definir esse valor como 0 impede que o tempo limite de suspensão ocorra.</span><span class="sxs-lookup"><span data-stu-id="16210-218">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="16210-219">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="16210-219">kioskAppDisplayName</span></span>|<span data-ttu-id="16210-220">String</span><span class="sxs-lookup"><span data-stu-id="16210-220">String</span></span>|<span data-ttu-id="16210-221">Especifica o texto de exibição para a conta mostrada na tela de entrada que inicializa o aplicativo especificado por SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="16210-221">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="16210-222">Aplicável somente quando KioskAppUserModelId está definido.</span><span class="sxs-lookup"><span data-stu-id="16210-222">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="16210-223">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="16210-223">kioskAppUserModelId</span></span>|<span data-ttu-id="16210-224">String</span><span class="sxs-lookup"><span data-stu-id="16210-224">String</span></span>|<span data-ttu-id="16210-225">Especifica a ID do modelo de usuário do aplicativo para uso com acesso atribuído.</span><span class="sxs-lookup"><span data-stu-id="16210-225">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="16210-226">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="16210-226">maintenanceStartTime</span></span>|<span data-ttu-id="16210-227">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="16210-227">TimeOfDay</span></span>|<span data-ttu-id="16210-228">Especifica o horário de início diário da hora de manutenção.</span><span class="sxs-lookup"><span data-stu-id="16210-228">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="16210-229">fastFirstSignIn</span><span class="sxs-lookup"><span data-stu-id="16210-229">fastFirstSignIn</span></span>|[<span data-ttu-id="16210-230">habilitação</span><span class="sxs-lookup"><span data-stu-id="16210-230">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="16210-231">Especifica se a conexão automática de novas contas não administrativas do Azure AD para contas locais de candidatos pré-configuradas.</span><span class="sxs-lookup"><span data-stu-id="16210-231">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="16210-232">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="16210-232">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="16210-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="16210-233">Response</span></span>
<span data-ttu-id="16210-234">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16210-234">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16210-235">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16210-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="16210-236">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16210-236">Request</span></span>
<span data-ttu-id="16210-237">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16210-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1147

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "allowedAccounts": "guest",
  "localStorage": "enabled",
  "allowLocalStorage": true,
  "setAccountManager": "enabled",
  "disableAccountManager": true,
  "setEduPolicies": "enabled",
  "disableEduPolicies": true,
  "setPowerPolicies": "enabled",
  "disablePowerPolicies": true,
  "signInOnResume": "enabled",
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000",
  "fastFirstSignIn": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="16210-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="16210-238">Response</span></span>
<span data-ttu-id="16210-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16210-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1319

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "allowedAccounts": "guest",
  "localStorage": "enabled",
  "allowLocalStorage": true,
  "setAccountManager": "enabled",
  "disableAccountManager": true,
  "setEduPolicies": "enabled",
  "disableEduPolicies": true,
  "setPowerPolicies": "enabled",
  "disablePowerPolicies": true,
  "signInOnResume": "enabled",
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000",
  "fastFirstSignIn": "enabled"
}
```





