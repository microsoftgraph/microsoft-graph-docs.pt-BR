---
title: Atualizar sharedPCConfiguration
description: Atualiza as propriedades de um objeto sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 573378a13c11f3ac08f2c07e42db2358a55518e9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147394"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="94a99-103">Atualizar sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="94a99-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="94a99-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="94a99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94a99-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94a99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94a99-106">Atualiza as propriedades de um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="94a99-106">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94a99-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="94a99-107">Prerequisites</span></span>
<span data-ttu-id="94a99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="94a99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="94a99-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94a99-110">Permission type</span></span>|<span data-ttu-id="94a99-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="94a99-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94a99-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94a99-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94a99-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94a99-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="94a99-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94a99-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94a99-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94a99-115">Not supported.</span></span>|
|<span data-ttu-id="94a99-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94a99-116">Application</span></span>|<span data-ttu-id="94a99-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94a99-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94a99-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94a99-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="94a99-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94a99-119">Request headers</span></span>
|<span data-ttu-id="94a99-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94a99-120">Header</span></span>|<span data-ttu-id="94a99-121">Valor</span><span class="sxs-lookup"><span data-stu-id="94a99-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94a99-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="94a99-122">Authorization</span></span>|<span data-ttu-id="94a99-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94a99-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94a99-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="94a99-124">Accept</span></span>|<span data-ttu-id="94a99-125">application/json</span><span class="sxs-lookup"><span data-stu-id="94a99-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94a99-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94a99-126">Request body</span></span>
<span data-ttu-id="94a99-127">No corpo da solicitação, forneça uma representação JSON do objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="94a99-127">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="94a99-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="94a99-128">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="94a99-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94a99-129">Property</span></span>|<span data-ttu-id="94a99-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="94a99-130">Type</span></span>|<span data-ttu-id="94a99-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="94a99-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94a99-132">id</span><span class="sxs-lookup"><span data-stu-id="94a99-132">id</span></span>|<span data-ttu-id="94a99-133">String</span><span class="sxs-lookup"><span data-stu-id="94a99-133">String</span></span>|<span data-ttu-id="94a99-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="94a99-134">Key of the entity.</span></span> <span data-ttu-id="94a99-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94a99-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94a99-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94a99-136">lastModifiedDateTime</span></span>|<span data-ttu-id="94a99-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94a99-137">DateTimeOffset</span></span>|<span data-ttu-id="94a99-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="94a99-138">DateTime the object was last modified.</span></span> <span data-ttu-id="94a99-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94a99-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94a99-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="94a99-140">roleScopeTagIds</span></span>|<span data-ttu-id="94a99-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="94a99-141">String collection</span></span>|<span data-ttu-id="94a99-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="94a99-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="94a99-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94a99-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94a99-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="94a99-144">supportsScopeTags</span></span>|<span data-ttu-id="94a99-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="94a99-145">Boolean</span></span>|<span data-ttu-id="94a99-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="94a99-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="94a99-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="94a99-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="94a99-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="94a99-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="94a99-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="94a99-149">This property is read-only.</span></span> <span data-ttu-id="94a99-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94a99-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94a99-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94a99-151">createdDateTime</span></span>|<span data-ttu-id="94a99-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94a99-152">DateTimeOffset</span></span>|<span data-ttu-id="94a99-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="94a99-153">DateTime the object was created.</span></span> <span data-ttu-id="94a99-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94a99-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94a99-155">description</span><span class="sxs-lookup"><span data-stu-id="94a99-155">description</span></span>|<span data-ttu-id="94a99-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94a99-156">String</span></span>|<span data-ttu-id="94a99-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="94a99-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="94a99-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94a99-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94a99-159">displayName</span><span class="sxs-lookup"><span data-stu-id="94a99-159">displayName</span></span>|<span data-ttu-id="94a99-160">String</span><span class="sxs-lookup"><span data-stu-id="94a99-160">String</span></span>|<span data-ttu-id="94a99-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="94a99-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="94a99-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94a99-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94a99-163">version</span><span class="sxs-lookup"><span data-stu-id="94a99-163">version</span></span>|<span data-ttu-id="94a99-164">Int32</span><span class="sxs-lookup"><span data-stu-id="94a99-164">Int32</span></span>|<span data-ttu-id="94a99-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="94a99-165">Version of the device configuration.</span></span> <span data-ttu-id="94a99-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94a99-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94a99-167">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="94a99-167">accountManagerPolicy</span></span>|[<span data-ttu-id="94a99-168">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="94a99-168">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="94a99-169">Especifica como as contas são gerenciadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="94a99-169">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="94a99-170">Aplica-se somente quando disableAccountManager é false.</span><span class="sxs-lookup"><span data-stu-id="94a99-170">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="94a99-171">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="94a99-171">allowedAccounts</span></span>|[<span data-ttu-id="94a99-172">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="94a99-172">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="94a99-173">Indica que tipos de contas podem ser usadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="94a99-173">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="94a99-174">Os valores possíveis são: `notConfigured`, `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="94a99-174">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="94a99-175">localStorage</span><span class="sxs-lookup"><span data-stu-id="94a99-175">localStorage</span></span>|[<span data-ttu-id="94a99-176">habilitação</span><span class="sxs-lookup"><span data-stu-id="94a99-176">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="94a99-177">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="94a99-177">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="94a99-178">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="94a99-178">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="94a99-179">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="94a99-179">allowLocalStorage</span></span>|<span data-ttu-id="94a99-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="94a99-180">Boolean</span></span>|<span data-ttu-id="94a99-181">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="94a99-181">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="94a99-182">setAccountmanager</span><span class="sxs-lookup"><span data-stu-id="94a99-182">setAccountManager</span></span>|[<span data-ttu-id="94a99-183">habilitação</span><span class="sxs-lookup"><span data-stu-id="94a99-183">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="94a99-184">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="94a99-184">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="94a99-185">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="94a99-185">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="94a99-186">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="94a99-186">disableAccountManager</span></span>|<span data-ttu-id="94a99-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="94a99-187">Boolean</span></span>|<span data-ttu-id="94a99-188">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="94a99-188">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="94a99-189">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="94a99-189">setEduPolicies</span></span>|[<span data-ttu-id="94a99-190">habilitação</span><span class="sxs-lookup"><span data-stu-id="94a99-190">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="94a99-191">Especifica se as políticas de ambiente de educação de computador compartilhado padrão devem ser habilitadas/desabilitadas/não configuradas.</span><span class="sxs-lookup"><span data-stu-id="94a99-191">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="94a99-192">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="94a99-192">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="94a99-193">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="94a99-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="94a99-194">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="94a99-194">disableEduPolicies</span></span>|<span data-ttu-id="94a99-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="94a99-195">Boolean</span></span>|<span data-ttu-id="94a99-196">Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="94a99-196">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="94a99-197">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="94a99-197">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="94a99-198">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="94a99-198">setPowerPolicies</span></span>|[<span data-ttu-id="94a99-199">habilitação</span><span class="sxs-lookup"><span data-stu-id="94a99-199">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="94a99-200">Especifica se as políticas de energia padrão do computador compartilhado devem ser ativadas/desativadas.</span><span class="sxs-lookup"><span data-stu-id="94a99-200">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="94a99-201">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="94a99-201">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="94a99-202">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="94a99-202">disablePowerPolicies</span></span>|<span data-ttu-id="94a99-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="94a99-203">Boolean</span></span>|<span data-ttu-id="94a99-204">Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="94a99-204">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="94a99-205">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="94a99-205">signInOnResume</span></span>|[<span data-ttu-id="94a99-206">habilitação</span><span class="sxs-lookup"><span data-stu-id="94a99-206">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="94a99-207">Especifica o requisito para entrar sempre que o dispositivo é ativado do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="94a99-207">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="94a99-208">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="94a99-208">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="94a99-209">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="94a99-209">disableSignInOnResume</span></span>|<span data-ttu-id="94a99-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="94a99-210">Boolean</span></span>|<span data-ttu-id="94a99-211">Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="94a99-211">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="94a99-212">enabled</span><span class="sxs-lookup"><span data-stu-id="94a99-212">enabled</span></span>|<span data-ttu-id="94a99-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="94a99-213">Boolean</span></span>|<span data-ttu-id="94a99-214">Habilita o modo de PC compartilhado e aplica as políticas de PC compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="94a99-214">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="94a99-215">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="94a99-215">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="94a99-216">Int32</span><span class="sxs-lookup"><span data-stu-id="94a99-216">Int32</span></span>|<span data-ttu-id="94a99-217">Especifica o tempo em segundos que um dispositivo deve ficar ocioso antes de o PC entrar em suspensão.</span><span class="sxs-lookup"><span data-stu-id="94a99-217">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="94a99-218">Definir esse valor como 0 impede que o tempo limite de suspensão ocorra.</span><span class="sxs-lookup"><span data-stu-id="94a99-218">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="94a99-219">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="94a99-219">kioskAppDisplayName</span></span>|<span data-ttu-id="94a99-220">String</span><span class="sxs-lookup"><span data-stu-id="94a99-220">String</span></span>|<span data-ttu-id="94a99-221">Especifica o texto de exibição para a conta mostrada na tela de entrada que inicializa o aplicativo especificado por SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="94a99-221">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="94a99-222">Aplicável somente quando KioskAppUserModelId está definido.</span><span class="sxs-lookup"><span data-stu-id="94a99-222">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="94a99-223">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="94a99-223">kioskAppUserModelId</span></span>|<span data-ttu-id="94a99-224">String</span><span class="sxs-lookup"><span data-stu-id="94a99-224">String</span></span>|<span data-ttu-id="94a99-225">Especifica a ID do modelo de usuário do aplicativo para uso com acesso atribuído.</span><span class="sxs-lookup"><span data-stu-id="94a99-225">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="94a99-226">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="94a99-226">maintenanceStartTime</span></span>|<span data-ttu-id="94a99-227">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="94a99-227">TimeOfDay</span></span>|<span data-ttu-id="94a99-228">Especifica o horário de início diário da hora de manutenção.</span><span class="sxs-lookup"><span data-stu-id="94a99-228">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="94a99-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="94a99-229">Response</span></span>
<span data-ttu-id="94a99-230">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94a99-230">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94a99-231">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94a99-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="94a99-232">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94a99-232">Request</span></span>
<span data-ttu-id="94a99-233">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94a99-233">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1114

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
  "maintenanceStartTime": "11:59:24.7240000"
}
```

### <a name="response"></a><span data-ttu-id="94a99-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="94a99-234">Response</span></span>
<span data-ttu-id="94a99-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94a99-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1286

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
  "maintenanceStartTime": "11:59:24.7240000"
}
```




