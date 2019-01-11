---
title: Criar sharedPCConfiguration
description: Cria um novo objeto sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 454f70ba8a89bd502e541638a9ba8b3d24ae4f7a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882051"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="5f050-103">Criar sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="5f050-103">Create sharedPCConfiguration</span></span>

> <span data-ttu-id="5f050-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5f050-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f050-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5f050-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f050-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5f050-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f050-107">Cria um novo objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f050-107">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5f050-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5f050-108">Prerequisites</span></span>
<span data-ttu-id="5f050-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f050-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f050-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f050-111">Permission type</span></span>|<span data-ttu-id="5f050-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5f050-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f050-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f050-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5f050-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f050-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5f050-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f050-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f050-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f050-116">Not supported.</span></span>|
|<span data-ttu-id="5f050-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f050-117">Application</span></span>|<span data-ttu-id="5f050-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f050-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f050-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f050-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5f050-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f050-120">Request headers</span></span>
|<span data-ttu-id="5f050-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5f050-121">Header</span></span>|<span data-ttu-id="5f050-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5f050-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f050-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f050-123">Authorization</span></span>|<span data-ttu-id="5f050-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f050-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f050-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5f050-125">Accept</span></span>|<span data-ttu-id="5f050-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f050-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f050-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f050-127">Request body</span></span>
<span data-ttu-id="5f050-128">No corpo da solicitação, forneça uma representação JSON do objeto sharedPCConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5f050-128">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="5f050-129">A tabela a seguir mostra as propriedades que são necessárias ao criar sharedPCConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5f050-129">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="5f050-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f050-130">Property</span></span>|<span data-ttu-id="5f050-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f050-131">Type</span></span>|<span data-ttu-id="5f050-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f050-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f050-133">id</span><span class="sxs-lookup"><span data-stu-id="5f050-133">id</span></span>|<span data-ttu-id="5f050-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f050-134">String</span></span>|<span data-ttu-id="5f050-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5f050-135">Key of the entity.</span></span> <span data-ttu-id="5f050-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5f050-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f050-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f050-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5f050-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f050-138">DateTimeOffset</span></span>|<span data-ttu-id="5f050-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5f050-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5f050-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5f050-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f050-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5f050-141">roleScopeTagIds</span></span>|<span data-ttu-id="5f050-142">String collection</span><span class="sxs-lookup"><span data-stu-id="5f050-142">String collection</span></span>|<span data-ttu-id="5f050-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="5f050-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5f050-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5f050-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f050-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5f050-145">supportsScopeTags</span></span>|<span data-ttu-id="5f050-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="5f050-146">Boolean</span></span>|<span data-ttu-id="5f050-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="5f050-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5f050-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="5f050-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5f050-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="5f050-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5f050-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f050-150">This property is read-only.</span></span> <span data-ttu-id="5f050-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5f050-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f050-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5f050-152">createdDateTime</span></span>|<span data-ttu-id="5f050-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f050-153">DateTimeOffset</span></span>|<span data-ttu-id="5f050-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5f050-154">DateTime the object was created.</span></span> <span data-ttu-id="5f050-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5f050-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f050-156">description</span><span class="sxs-lookup"><span data-stu-id="5f050-156">description</span></span>|<span data-ttu-id="5f050-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f050-157">String</span></span>|<span data-ttu-id="5f050-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5f050-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5f050-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5f050-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f050-160">displayName</span><span class="sxs-lookup"><span data-stu-id="5f050-160">displayName</span></span>|<span data-ttu-id="5f050-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f050-161">String</span></span>|<span data-ttu-id="5f050-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5f050-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5f050-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5f050-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f050-164">version</span><span class="sxs-lookup"><span data-stu-id="5f050-164">version</span></span>|<span data-ttu-id="5f050-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5f050-165">Int32</span></span>|<span data-ttu-id="5f050-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5f050-166">Version of the device configuration.</span></span> <span data-ttu-id="5f050-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5f050-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f050-168">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="5f050-168">accountManagerPolicy</span></span>|[<span data-ttu-id="5f050-169">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="5f050-169">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="5f050-170">Especifica como as contas são gerenciadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="5f050-170">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="5f050-171">Aplica-se somente quando disableAccountManager é false.</span><span class="sxs-lookup"><span data-stu-id="5f050-171">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="5f050-172">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="5f050-172">allowedAccounts</span></span>|[<span data-ttu-id="5f050-173">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="5f050-173">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="5f050-174">Indica que tipos de contas podem ser usadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="5f050-174">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="5f050-175">Os valores possíveis são: `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="5f050-175">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="5f050-176">localStorage</span><span class="sxs-lookup"><span data-stu-id="5f050-176">localStorage</span></span>|[<span data-ttu-id="5f050-177">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="5f050-177">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="5f050-178">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="5f050-178">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="5f050-179">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="5f050-179">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="5f050-180">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="5f050-180">allowLocalStorage</span></span>|<span data-ttu-id="5f050-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="5f050-181">Boolean</span></span>|<span data-ttu-id="5f050-182">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="5f050-182">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="5f050-183">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="5f050-183">setAccountManager</span></span>|[<span data-ttu-id="5f050-184">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="5f050-184">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="5f050-185">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="5f050-185">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="5f050-186">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="5f050-186">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="5f050-187">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="5f050-187">disableAccountManager</span></span>|<span data-ttu-id="5f050-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="5f050-188">Boolean</span></span>|<span data-ttu-id="5f050-189">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="5f050-189">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="5f050-190">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="5f050-190">setEduPolicies</span></span>|[<span data-ttu-id="5f050-191">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="5f050-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="5f050-192">Especifica se as políticas de ambiente de educação de PC compartilhada padrão devem ser ativado/desativado/não são configuradas.</span><span class="sxs-lookup"><span data-stu-id="5f050-192">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="5f050-193">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="5f050-193">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="5f050-194">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="5f050-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="5f050-195">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="5f050-195">disableEduPolicies</span></span>|<span data-ttu-id="5f050-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="5f050-196">Boolean</span></span>|<span data-ttu-id="5f050-197">Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="5f050-197">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="5f050-198">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="5f050-198">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="5f050-199">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="5f050-199">setPowerPolicies</span></span>|[<span data-ttu-id="5f050-200">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="5f050-200">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="5f050-201">Especifica se as políticas de energia do PC compartilhada padrão devem ser ativado/desativado.</span><span class="sxs-lookup"><span data-stu-id="5f050-201">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="5f050-202">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="5f050-202">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="5f050-203">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="5f050-203">disablePowerPolicies</span></span>|<span data-ttu-id="5f050-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="5f050-204">Boolean</span></span>|<span data-ttu-id="5f050-205">Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="5f050-205">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="5f050-206">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="5f050-206">signInOnResume</span></span>|[<span data-ttu-id="5f050-207">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="5f050-207">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="5f050-208">Especifica o requisito para entrar no sempre que o dispositivo retorna do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="5f050-208">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="5f050-209">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="5f050-209">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="5f050-210">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="5f050-210">disableSignInOnResume</span></span>|<span data-ttu-id="5f050-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="5f050-211">Boolean</span></span>|<span data-ttu-id="5f050-212">Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="5f050-212">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="5f050-213">enabled</span><span class="sxs-lookup"><span data-stu-id="5f050-213">enabled</span></span>|<span data-ttu-id="5f050-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="5f050-214">Boolean</span></span>|<span data-ttu-id="5f050-215">Habilita o modo de PC compartilhado e aplica as políticas de PC compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="5f050-215">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="5f050-216">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="5f050-216">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="5f050-217">Int32</span><span class="sxs-lookup"><span data-stu-id="5f050-217">Int32</span></span>|<span data-ttu-id="5f050-218">Especifica o tempo em segundos que um dispositivo deve ficar ocioso antes de o PC entrar em suspensão.</span><span class="sxs-lookup"><span data-stu-id="5f050-218">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="5f050-219">Definir esse valor como 0 impede que o tempo limite de suspensão ocorra.</span><span class="sxs-lookup"><span data-stu-id="5f050-219">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="5f050-220">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="5f050-220">kioskAppDisplayName</span></span>|<span data-ttu-id="5f050-221">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f050-221">String</span></span>|<span data-ttu-id="5f050-222">Especifica o texto de exibição para a conta mostrada na tela de entrada que inicializa o aplicativo especificado por SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="5f050-222">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="5f050-223">Aplicável somente quando KioskAppUserModelId está definido.</span><span class="sxs-lookup"><span data-stu-id="5f050-223">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="5f050-224">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="5f050-224">kioskAppUserModelId</span></span>|<span data-ttu-id="5f050-225">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f050-225">String</span></span>|<span data-ttu-id="5f050-226">Especifica a ID do modelo de usuário do aplicativo para uso com acesso atribuído.</span><span class="sxs-lookup"><span data-stu-id="5f050-226">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="5f050-227">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="5f050-227">maintenanceStartTime</span></span>|<span data-ttu-id="5f050-228">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5f050-228">TimeOfDay</span></span>|<span data-ttu-id="5f050-229">Especifica o horário de início diário da hora de manutenção.</span><span class="sxs-lookup"><span data-stu-id="5f050-229">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="5f050-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f050-230">Response</span></span>
<span data-ttu-id="5f050-231">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f050-231">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f050-232">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f050-232">Example</span></span>
### <a name="request"></a><span data-ttu-id="5f050-233">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f050-233">Request</span></span>
<span data-ttu-id="5f050-234">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f050-234">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1179

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
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

### <a name="response"></a><span data-ttu-id="5f050-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f050-235">Response</span></span>
<span data-ttu-id="5f050-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f050-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





