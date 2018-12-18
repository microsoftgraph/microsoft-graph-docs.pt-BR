---
title: Atualizar sharedPCConfiguration
description: Atualiza as propriedades de um objeto sharedPCConfiguration.
author: tfitzmac
ms.openlocfilehash: f9fbaf72531b130e41c01609e4d28eb35a7d5d84
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338728"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="f1baf-103">Atualizar sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1baf-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="f1baf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f1baf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1baf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f1baf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1baf-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f1baf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1baf-107">Atualiza as propriedades de um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1baf-107">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1baf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1baf-108">Prerequisites</span></span>
<span data-ttu-id="f1baf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1baf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1baf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1baf-111">Permission type</span></span>|<span data-ttu-id="f1baf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1baf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1baf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1baf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1baf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1baf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1baf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1baf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1baf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1baf-116">Not supported.</span></span>|
|<span data-ttu-id="f1baf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1baf-117">Application</span></span>|<span data-ttu-id="f1baf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1baf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1baf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1baf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f1baf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1baf-120">Request headers</span></span>
|<span data-ttu-id="f1baf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1baf-121">Header</span></span>|<span data-ttu-id="f1baf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f1baf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1baf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1baf-123">Authorization</span></span>|<span data-ttu-id="f1baf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1baf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1baf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f1baf-125">Accept</span></span>|<span data-ttu-id="f1baf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1baf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1baf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1baf-127">Request body</span></span>
<span data-ttu-id="f1baf-128">No corpo da solicitação, forneça uma representação JSON do objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1baf-128">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="f1baf-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1baf-129">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="f1baf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1baf-130">Property</span></span>|<span data-ttu-id="f1baf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1baf-131">Type</span></span>|<span data-ttu-id="f1baf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1baf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1baf-133">id</span><span class="sxs-lookup"><span data-stu-id="f1baf-133">id</span></span>|<span data-ttu-id="f1baf-134">String</span><span class="sxs-lookup"><span data-stu-id="f1baf-134">String</span></span>|<span data-ttu-id="f1baf-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f1baf-135">Key of the entity.</span></span> <span data-ttu-id="f1baf-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1baf-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1baf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1baf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f1baf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1baf-138">DateTimeOffset</span></span>|<span data-ttu-id="f1baf-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f1baf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f1baf-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1baf-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1baf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f1baf-141">roleScopeTagIds</span></span>|<span data-ttu-id="f1baf-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f1baf-142">String collection</span></span>|<span data-ttu-id="f1baf-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="f1baf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f1baf-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1baf-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1baf-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f1baf-145">supportsScopeTags</span></span>|<span data-ttu-id="f1baf-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1baf-146">Boolean</span></span>|<span data-ttu-id="f1baf-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f1baf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f1baf-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f1baf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f1baf-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="f1baf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f1baf-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1baf-150">This property is read-only.</span></span> <span data-ttu-id="f1baf-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1baf-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1baf-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1baf-152">createdDateTime</span></span>|<span data-ttu-id="f1baf-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1baf-153">DateTimeOffset</span></span>|<span data-ttu-id="f1baf-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f1baf-154">DateTime the object was created.</span></span> <span data-ttu-id="f1baf-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1baf-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1baf-156">description</span><span class="sxs-lookup"><span data-stu-id="f1baf-156">description</span></span>|<span data-ttu-id="f1baf-157">String</span><span class="sxs-lookup"><span data-stu-id="f1baf-157">String</span></span>|<span data-ttu-id="f1baf-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f1baf-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f1baf-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1baf-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1baf-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f1baf-160">displayName</span></span>|<span data-ttu-id="f1baf-161">String</span><span class="sxs-lookup"><span data-stu-id="f1baf-161">String</span></span>|<span data-ttu-id="f1baf-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f1baf-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f1baf-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1baf-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1baf-164">version</span><span class="sxs-lookup"><span data-stu-id="f1baf-164">version</span></span>|<span data-ttu-id="f1baf-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f1baf-165">Int32</span></span>|<span data-ttu-id="f1baf-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f1baf-166">Version of the device configuration.</span></span> <span data-ttu-id="f1baf-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1baf-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1baf-168">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="f1baf-168">accountManagerPolicy</span></span>|[<span data-ttu-id="f1baf-169">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="f1baf-169">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="f1baf-170">Especifica como as contas são gerenciadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="f1baf-170">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="f1baf-171">Aplica-se somente quando disableAccountManager é false.</span><span class="sxs-lookup"><span data-stu-id="f1baf-171">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="f1baf-172">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="f1baf-172">allowedAccounts</span></span>|[<span data-ttu-id="f1baf-173">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="f1baf-173">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="f1baf-174">Indica que tipos de contas podem ser usadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="f1baf-174">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="f1baf-175">Os valores possíveis são: `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="f1baf-175">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="f1baf-176">localStorage</span><span class="sxs-lookup"><span data-stu-id="f1baf-176">localStorage</span></span>|[<span data-ttu-id="f1baf-177">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="f1baf-177">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f1baf-178">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="f1baf-178">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="f1baf-179">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f1baf-179">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f1baf-180">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="f1baf-180">allowLocalStorage</span></span>|<span data-ttu-id="f1baf-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1baf-181">Boolean</span></span>|<span data-ttu-id="f1baf-182">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="f1baf-182">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="f1baf-183">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="f1baf-183">setAccountManager</span></span>|[<span data-ttu-id="f1baf-184">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="f1baf-184">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f1baf-185">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="f1baf-185">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="f1baf-186">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f1baf-186">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f1baf-187">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="f1baf-187">disableAccountManager</span></span>|<span data-ttu-id="f1baf-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1baf-188">Boolean</span></span>|<span data-ttu-id="f1baf-189">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="f1baf-189">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="f1baf-190">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="f1baf-190">setEduPolicies</span></span>|[<span data-ttu-id="f1baf-191">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="f1baf-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f1baf-192">Especifica se as políticas de ambiente de educação de PC compartilhada padrão devem ser ativado/desativado/não são configuradas.</span><span class="sxs-lookup"><span data-stu-id="f1baf-192">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="f1baf-193">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="f1baf-193">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="f1baf-194">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f1baf-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f1baf-195">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="f1baf-195">disableEduPolicies</span></span>|<span data-ttu-id="f1baf-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1baf-196">Boolean</span></span>|<span data-ttu-id="f1baf-197">Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="f1baf-197">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="f1baf-198">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="f1baf-198">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="f1baf-199">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="f1baf-199">setPowerPolicies</span></span>|[<span data-ttu-id="f1baf-200">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="f1baf-200">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f1baf-201">Especifica se as políticas de energia do PC compartilhada padrão devem ser ativado/desativado.</span><span class="sxs-lookup"><span data-stu-id="f1baf-201">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="f1baf-202">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f1baf-202">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f1baf-203">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="f1baf-203">disablePowerPolicies</span></span>|<span data-ttu-id="f1baf-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1baf-204">Boolean</span></span>|<span data-ttu-id="f1baf-205">Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="f1baf-205">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="f1baf-206">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="f1baf-206">signInOnResume</span></span>|[<span data-ttu-id="f1baf-207">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="f1baf-207">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f1baf-208">Especifica o requisito para entrar no sempre que o dispositivo retorna do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="f1baf-208">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="f1baf-209">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f1baf-209">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f1baf-210">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="f1baf-210">disableSignInOnResume</span></span>|<span data-ttu-id="f1baf-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1baf-211">Boolean</span></span>|<span data-ttu-id="f1baf-212">Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="f1baf-212">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="f1baf-213">enabled</span><span class="sxs-lookup"><span data-stu-id="f1baf-213">enabled</span></span>|<span data-ttu-id="f1baf-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1baf-214">Boolean</span></span>|<span data-ttu-id="f1baf-215">Habilita o modo de PC compartilhado e aplica as políticas de PC compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="f1baf-215">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="f1baf-216">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="f1baf-216">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="f1baf-217">Int32</span><span class="sxs-lookup"><span data-stu-id="f1baf-217">Int32</span></span>|<span data-ttu-id="f1baf-218">Especifica o tempo em segundos que um dispositivo deve ficar ocioso antes de o PC entrar em suspensão.</span><span class="sxs-lookup"><span data-stu-id="f1baf-218">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="f1baf-219">Definir esse valor como 0 impede que o tempo limite de suspensão ocorra.</span><span class="sxs-lookup"><span data-stu-id="f1baf-219">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="f1baf-220">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="f1baf-220">kioskAppDisplayName</span></span>|<span data-ttu-id="f1baf-221">String</span><span class="sxs-lookup"><span data-stu-id="f1baf-221">String</span></span>|<span data-ttu-id="f1baf-222">Especifica o texto de exibição para a conta mostrada na tela de entrada que inicializa o aplicativo especificado por SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="f1baf-222">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="f1baf-223">Aplicável somente quando KioskAppUserModelId está definido.</span><span class="sxs-lookup"><span data-stu-id="f1baf-223">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="f1baf-224">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="f1baf-224">kioskAppUserModelId</span></span>|<span data-ttu-id="f1baf-225">String</span><span class="sxs-lookup"><span data-stu-id="f1baf-225">String</span></span>|<span data-ttu-id="f1baf-226">Especifica a ID do modelo de usuário do aplicativo para uso com acesso atribuído.</span><span class="sxs-lookup"><span data-stu-id="f1baf-226">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="f1baf-227">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="f1baf-227">maintenanceStartTime</span></span>|<span data-ttu-id="f1baf-228">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f1baf-228">TimeOfDay</span></span>|<span data-ttu-id="f1baf-229">Especifica o horário de início diário da hora de manutenção.</span><span class="sxs-lookup"><span data-stu-id="f1baf-229">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="f1baf-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1baf-230">Response</span></span>
<span data-ttu-id="f1baf-231">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1baf-231">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1baf-232">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1baf-232">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1baf-233">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1baf-233">Request</span></span>
<span data-ttu-id="f1baf-234">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1baf-234">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f1baf-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1baf-235">Response</span></span>
<span data-ttu-id="f1baf-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1baf-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





