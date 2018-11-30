---
title: Atualizar sharedPCConfiguration
description: Atualiza as propriedades de um objeto sharedPCConfiguration.
ms.openlocfilehash: 94b68e8d81bb73db979f1032fbc2c4efcdd668f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037516"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="9fa37-103">Atualizar sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="9fa37-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="9fa37-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9fa37-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fa37-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9fa37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9fa37-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9fa37-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9fa37-107">Atualiza as propriedades de um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9fa37-107">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9fa37-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9fa37-108">Prerequisites</span></span>
<span data-ttu-id="9fa37-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fa37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fa37-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fa37-111">Permission type</span></span>|<span data-ttu-id="9fa37-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9fa37-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fa37-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fa37-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9fa37-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fa37-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9fa37-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fa37-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fa37-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fa37-116">Not supported.</span></span>|
|<span data-ttu-id="9fa37-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fa37-117">Application</span></span>|<span data-ttu-id="9fa37-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fa37-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fa37-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fa37-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9fa37-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fa37-120">Request headers</span></span>
|<span data-ttu-id="9fa37-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9fa37-121">Header</span></span>|<span data-ttu-id="9fa37-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9fa37-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fa37-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fa37-123">Authorization</span></span>|<span data-ttu-id="9fa37-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fa37-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fa37-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9fa37-125">Accept</span></span>|<span data-ttu-id="9fa37-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9fa37-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fa37-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9fa37-127">Request body</span></span>
<span data-ttu-id="9fa37-128">No corpo da solicitação, forneça uma representação JSON do objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9fa37-128">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="9fa37-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9fa37-129">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="9fa37-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fa37-130">Property</span></span>|<span data-ttu-id="9fa37-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fa37-131">Type</span></span>|<span data-ttu-id="9fa37-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fa37-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fa37-133">id</span><span class="sxs-lookup"><span data-stu-id="9fa37-133">id</span></span>|<span data-ttu-id="9fa37-134">String</span><span class="sxs-lookup"><span data-stu-id="9fa37-134">String</span></span>|<span data-ttu-id="9fa37-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9fa37-135">Key of the entity.</span></span> <span data-ttu-id="9fa37-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9fa37-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9fa37-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9fa37-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9fa37-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fa37-138">DateTimeOffset</span></span>|<span data-ttu-id="9fa37-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9fa37-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9fa37-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9fa37-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9fa37-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9fa37-141">roleScopeTagIds</span></span>|<span data-ttu-id="9fa37-142">String collection</span><span class="sxs-lookup"><span data-stu-id="9fa37-142">String collection</span></span>|<span data-ttu-id="9fa37-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="9fa37-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9fa37-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9fa37-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9fa37-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9fa37-145">supportsScopeTags</span></span>|<span data-ttu-id="9fa37-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="9fa37-146">Boolean</span></span>|<span data-ttu-id="9fa37-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9fa37-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9fa37-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9fa37-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9fa37-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="9fa37-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9fa37-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9fa37-150">This property is read-only.</span></span> <span data-ttu-id="9fa37-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9fa37-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9fa37-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9fa37-152">createdDateTime</span></span>|<span data-ttu-id="9fa37-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fa37-153">DateTimeOffset</span></span>|<span data-ttu-id="9fa37-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9fa37-154">DateTime the object was created.</span></span> <span data-ttu-id="9fa37-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9fa37-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9fa37-156">description</span><span class="sxs-lookup"><span data-stu-id="9fa37-156">description</span></span>|<span data-ttu-id="9fa37-157">String</span><span class="sxs-lookup"><span data-stu-id="9fa37-157">String</span></span>|<span data-ttu-id="9fa37-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9fa37-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9fa37-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9fa37-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9fa37-160">displayName</span><span class="sxs-lookup"><span data-stu-id="9fa37-160">displayName</span></span>|<span data-ttu-id="9fa37-161">String</span><span class="sxs-lookup"><span data-stu-id="9fa37-161">String</span></span>|<span data-ttu-id="9fa37-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9fa37-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9fa37-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9fa37-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9fa37-164">version</span><span class="sxs-lookup"><span data-stu-id="9fa37-164">version</span></span>|<span data-ttu-id="9fa37-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9fa37-165">Int32</span></span>|<span data-ttu-id="9fa37-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9fa37-166">Version of the device configuration.</span></span> <span data-ttu-id="9fa37-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9fa37-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9fa37-168">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="9fa37-168">accountManagerPolicy</span></span>|[<span data-ttu-id="9fa37-169">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="9fa37-169">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="9fa37-170">Especifica como as contas são gerenciadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="9fa37-170">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="9fa37-171">Aplica-se somente quando disableAccountManager é false.</span><span class="sxs-lookup"><span data-stu-id="9fa37-171">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="9fa37-172">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="9fa37-172">allowedAccounts</span></span>|[<span data-ttu-id="9fa37-173">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="9fa37-173">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="9fa37-174">Indica que tipos de contas podem ser usadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="9fa37-174">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="9fa37-175">Os valores possíveis são: `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="9fa37-175">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="9fa37-176">localStorage</span><span class="sxs-lookup"><span data-stu-id="9fa37-176">localStorage</span></span>|[<span data-ttu-id="9fa37-177">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="9fa37-177">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9fa37-178">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="9fa37-178">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="9fa37-179">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9fa37-179">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9fa37-180">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="9fa37-180">allowLocalStorage</span></span>|<span data-ttu-id="9fa37-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="9fa37-181">Boolean</span></span>|<span data-ttu-id="9fa37-182">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="9fa37-182">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="9fa37-183">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="9fa37-183">setAccountManager</span></span>|[<span data-ttu-id="9fa37-184">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="9fa37-184">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9fa37-185">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="9fa37-185">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="9fa37-186">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9fa37-186">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9fa37-187">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="9fa37-187">disableAccountManager</span></span>|<span data-ttu-id="9fa37-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="9fa37-188">Boolean</span></span>|<span data-ttu-id="9fa37-189">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="9fa37-189">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="9fa37-190">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="9fa37-190">setEduPolicies</span></span>|[<span data-ttu-id="9fa37-191">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="9fa37-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9fa37-192">Especifica se as políticas de ambiente de educação de PC compartilhada padrão devem ser ativado/desativado/não são configuradas.</span><span class="sxs-lookup"><span data-stu-id="9fa37-192">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="9fa37-193">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="9fa37-193">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="9fa37-194">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9fa37-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9fa37-195">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="9fa37-195">disableEduPolicies</span></span>|<span data-ttu-id="9fa37-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="9fa37-196">Boolean</span></span>|<span data-ttu-id="9fa37-197">Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="9fa37-197">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="9fa37-198">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="9fa37-198">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="9fa37-199">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="9fa37-199">setPowerPolicies</span></span>|[<span data-ttu-id="9fa37-200">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="9fa37-200">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9fa37-201">Especifica se as políticas de energia do PC compartilhada padrão devem ser ativado/desativado.</span><span class="sxs-lookup"><span data-stu-id="9fa37-201">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="9fa37-202">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9fa37-202">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9fa37-203">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="9fa37-203">disablePowerPolicies</span></span>|<span data-ttu-id="9fa37-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="9fa37-204">Boolean</span></span>|<span data-ttu-id="9fa37-205">Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="9fa37-205">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="9fa37-206">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="9fa37-206">signInOnResume</span></span>|[<span data-ttu-id="9fa37-207">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="9fa37-207">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9fa37-208">Especifica o requisito para entrar no sempre que o dispositivo retorna do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="9fa37-208">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="9fa37-209">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9fa37-209">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9fa37-210">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="9fa37-210">disableSignInOnResume</span></span>|<span data-ttu-id="9fa37-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="9fa37-211">Boolean</span></span>|<span data-ttu-id="9fa37-212">Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="9fa37-212">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="9fa37-213">enabled</span><span class="sxs-lookup"><span data-stu-id="9fa37-213">enabled</span></span>|<span data-ttu-id="9fa37-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="9fa37-214">Boolean</span></span>|<span data-ttu-id="9fa37-215">Habilita o modo de PC compartilhado e aplica as políticas de PC compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="9fa37-215">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="9fa37-216">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="9fa37-216">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="9fa37-217">Int32</span><span class="sxs-lookup"><span data-stu-id="9fa37-217">Int32</span></span>|<span data-ttu-id="9fa37-218">Especifica o tempo em segundos que um dispositivo deve ficar ocioso antes de o PC entrar em suspensão.</span><span class="sxs-lookup"><span data-stu-id="9fa37-218">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="9fa37-219">Definir esse valor como 0 impede que o tempo limite de suspensão ocorra.</span><span class="sxs-lookup"><span data-stu-id="9fa37-219">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="9fa37-220">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="9fa37-220">kioskAppDisplayName</span></span>|<span data-ttu-id="9fa37-221">String</span><span class="sxs-lookup"><span data-stu-id="9fa37-221">String</span></span>|<span data-ttu-id="9fa37-222">Especifica o texto de exibição para a conta mostrada na tela de entrada que inicializa o aplicativo especificado por SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="9fa37-222">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="9fa37-223">Aplicável somente quando KioskAppUserModelId está definido.</span><span class="sxs-lookup"><span data-stu-id="9fa37-223">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="9fa37-224">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="9fa37-224">kioskAppUserModelId</span></span>|<span data-ttu-id="9fa37-225">String</span><span class="sxs-lookup"><span data-stu-id="9fa37-225">String</span></span>|<span data-ttu-id="9fa37-226">Especifica a ID do modelo de usuário do aplicativo para uso com acesso atribuído.</span><span class="sxs-lookup"><span data-stu-id="9fa37-226">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="9fa37-227">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="9fa37-227">maintenanceStartTime</span></span>|<span data-ttu-id="9fa37-228">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9fa37-228">TimeOfDay</span></span>|<span data-ttu-id="9fa37-229">Especifica o horário de início diário da hora de manutenção.</span><span class="sxs-lookup"><span data-stu-id="9fa37-229">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="9fa37-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fa37-230">Response</span></span>
<span data-ttu-id="9fa37-231">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9fa37-231">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fa37-232">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9fa37-232">Example</span></span>
### <a name="request"></a><span data-ttu-id="9fa37-233">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fa37-233">Request</span></span>
<span data-ttu-id="9fa37-234">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fa37-234">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1119

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "allowedAccounts": "domain",
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

### <a name="response"></a><span data-ttu-id="9fa37-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fa37-235">Response</span></span>
<span data-ttu-id="9fa37-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9fa37-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1287

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
  "allowedAccounts": "domain",
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





