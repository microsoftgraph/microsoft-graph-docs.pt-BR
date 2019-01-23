---
title: Atualizar sharedPCConfiguration
description: Atualiza as propriedades de um objeto sharedPCConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: da0cbba1de768fffd572728d3d416de83917e582
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396326"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="00cf9-103">Atualizar sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="00cf9-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="00cf9-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="00cf9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="00cf9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="00cf9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00cf9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="00cf9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00cf9-107">Atualiza as propriedades de um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00cf9-107">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00cf9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="00cf9-108">Prerequisites</span></span>
<span data-ttu-id="00cf9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="00cf9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="00cf9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00cf9-111">Permission type</span></span>|<span data-ttu-id="00cf9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="00cf9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00cf9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00cf9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00cf9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00cf9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="00cf9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00cf9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00cf9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00cf9-116">Not supported.</span></span>|
|<span data-ttu-id="00cf9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00cf9-117">Application</span></span>|<span data-ttu-id="00cf9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00cf9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00cf9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00cf9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="00cf9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00cf9-120">Request headers</span></span>
|<span data-ttu-id="00cf9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="00cf9-121">Header</span></span>|<span data-ttu-id="00cf9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="00cf9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00cf9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="00cf9-123">Authorization</span></span>|<span data-ttu-id="00cf9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00cf9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00cf9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="00cf9-125">Accept</span></span>|<span data-ttu-id="00cf9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00cf9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00cf9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00cf9-127">Request body</span></span>
<span data-ttu-id="00cf9-128">No corpo da solicitação, forneça uma representação JSON do objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00cf9-128">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="00cf9-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00cf9-129">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="00cf9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00cf9-130">Property</span></span>|<span data-ttu-id="00cf9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="00cf9-131">Type</span></span>|<span data-ttu-id="00cf9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="00cf9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00cf9-133">id</span><span class="sxs-lookup"><span data-stu-id="00cf9-133">id</span></span>|<span data-ttu-id="00cf9-134">String</span><span class="sxs-lookup"><span data-stu-id="00cf9-134">String</span></span>|<span data-ttu-id="00cf9-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="00cf9-135">Key of the entity.</span></span> <span data-ttu-id="00cf9-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00cf9-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00cf9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00cf9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="00cf9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00cf9-138">DateTimeOffset</span></span>|<span data-ttu-id="00cf9-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="00cf9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="00cf9-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00cf9-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00cf9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="00cf9-141">roleScopeTagIds</span></span>|<span data-ttu-id="00cf9-142">String collection</span><span class="sxs-lookup"><span data-stu-id="00cf9-142">String collection</span></span>|<span data-ttu-id="00cf9-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="00cf9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="00cf9-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00cf9-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00cf9-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="00cf9-145">supportsScopeTags</span></span>|<span data-ttu-id="00cf9-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="00cf9-146">Boolean</span></span>|<span data-ttu-id="00cf9-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="00cf9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="00cf9-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="00cf9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="00cf9-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="00cf9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="00cf9-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="00cf9-150">This property is read-only.</span></span> <span data-ttu-id="00cf9-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00cf9-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00cf9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00cf9-152">createdDateTime</span></span>|<span data-ttu-id="00cf9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00cf9-153">DateTimeOffset</span></span>|<span data-ttu-id="00cf9-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="00cf9-154">DateTime the object was created.</span></span> <span data-ttu-id="00cf9-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00cf9-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00cf9-156">description</span><span class="sxs-lookup"><span data-stu-id="00cf9-156">description</span></span>|<span data-ttu-id="00cf9-157">String</span><span class="sxs-lookup"><span data-stu-id="00cf9-157">String</span></span>|<span data-ttu-id="00cf9-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00cf9-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="00cf9-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00cf9-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00cf9-160">displayName</span><span class="sxs-lookup"><span data-stu-id="00cf9-160">displayName</span></span>|<span data-ttu-id="00cf9-161">String</span><span class="sxs-lookup"><span data-stu-id="00cf9-161">String</span></span>|<span data-ttu-id="00cf9-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00cf9-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="00cf9-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00cf9-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00cf9-164">version</span><span class="sxs-lookup"><span data-stu-id="00cf9-164">version</span></span>|<span data-ttu-id="00cf9-165">Int32</span><span class="sxs-lookup"><span data-stu-id="00cf9-165">Int32</span></span>|<span data-ttu-id="00cf9-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00cf9-166">Version of the device configuration.</span></span> <span data-ttu-id="00cf9-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00cf9-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00cf9-168">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="00cf9-168">accountManagerPolicy</span></span>|[<span data-ttu-id="00cf9-169">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="00cf9-169">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="00cf9-170">Especifica como as contas são gerenciadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="00cf9-170">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="00cf9-171">Aplica-se somente quando disableAccountManager é false.</span><span class="sxs-lookup"><span data-stu-id="00cf9-171">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="00cf9-172">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="00cf9-172">allowedAccounts</span></span>|[<span data-ttu-id="00cf9-173">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="00cf9-173">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="00cf9-174">Indica que tipos de contas podem ser usadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="00cf9-174">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="00cf9-175">Os valores possíveis são: `notConfigured`, `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="00cf9-175">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="00cf9-176">localStorage</span><span class="sxs-lookup"><span data-stu-id="00cf9-176">localStorage</span></span>|<span data-ttu-id="00cf9-177">[habilitação] (.. /Resources/Intune-Shared-Enablement</span><span class="sxs-lookup"><span data-stu-id="00cf9-177">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="00cf9-178">.MD)</span><span class="sxs-lookup"><span data-stu-id="00cf9-178">.md)</span></span>|<span data-ttu-id="00cf9-179">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="00cf9-179">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="00cf9-180">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="00cf9-180">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="00cf9-181">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="00cf9-181">allowLocalStorage</span></span>|<span data-ttu-id="00cf9-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="00cf9-182">Boolean</span></span>|<span data-ttu-id="00cf9-183">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="00cf9-183">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="00cf9-184">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="00cf9-184">setAccountManager</span></span>|<span data-ttu-id="00cf9-185">[habilitação] (.. /Resources/Intune-Shared-Enablement</span><span class="sxs-lookup"><span data-stu-id="00cf9-185">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="00cf9-186">.MD)</span><span class="sxs-lookup"><span data-stu-id="00cf9-186">.md)</span></span>|<span data-ttu-id="00cf9-187">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="00cf9-187">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="00cf9-188">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="00cf9-188">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="00cf9-189">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="00cf9-189">disableAccountManager</span></span>|<span data-ttu-id="00cf9-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="00cf9-190">Boolean</span></span>|<span data-ttu-id="00cf9-191">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="00cf9-191">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="00cf9-192">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="00cf9-192">setEduPolicies</span></span>|<span data-ttu-id="00cf9-193">[habilitação] (.. /Resources/Intune-Shared-Enablement</span><span class="sxs-lookup"><span data-stu-id="00cf9-193">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="00cf9-194">.MD)</span><span class="sxs-lookup"><span data-stu-id="00cf9-194">.md)</span></span>|<span data-ttu-id="00cf9-195">Especifica se as políticas de ambiente de educação de PC compartilhada padrão devem ser ativado/desativado/não são configuradas.</span><span class="sxs-lookup"><span data-stu-id="00cf9-195">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="00cf9-196">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="00cf9-196">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="00cf9-197">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="00cf9-197">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="00cf9-198">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="00cf9-198">disableEduPolicies</span></span>|<span data-ttu-id="00cf9-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="00cf9-199">Boolean</span></span>|<span data-ttu-id="00cf9-200">Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="00cf9-200">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="00cf9-201">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="00cf9-201">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="00cf9-202">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="00cf9-202">setPowerPolicies</span></span>|<span data-ttu-id="00cf9-203">[habilitação] (.. /Resources/Intune-Shared-Enablement</span><span class="sxs-lookup"><span data-stu-id="00cf9-203">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="00cf9-204">.MD)</span><span class="sxs-lookup"><span data-stu-id="00cf9-204">.md)</span></span>|<span data-ttu-id="00cf9-205">Especifica se as políticas de energia do PC compartilhada padrão devem ser ativado/desativado.</span><span class="sxs-lookup"><span data-stu-id="00cf9-205">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="00cf9-206">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="00cf9-206">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="00cf9-207">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="00cf9-207">disablePowerPolicies</span></span>|<span data-ttu-id="00cf9-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="00cf9-208">Boolean</span></span>|<span data-ttu-id="00cf9-209">Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="00cf9-209">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="00cf9-210">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="00cf9-210">signInOnResume</span></span>|<span data-ttu-id="00cf9-211">[habilitação] (.. /Resources/Intune-Shared-Enablement</span><span class="sxs-lookup"><span data-stu-id="00cf9-211">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="00cf9-212">.MD)</span><span class="sxs-lookup"><span data-stu-id="00cf9-212">.md)</span></span>|<span data-ttu-id="00cf9-213">Especifica o requisito para entrar no sempre que o dispositivo retorna do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="00cf9-213">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="00cf9-214">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="00cf9-214">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="00cf9-215">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="00cf9-215">disableSignInOnResume</span></span>|<span data-ttu-id="00cf9-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="00cf9-216">Boolean</span></span>|<span data-ttu-id="00cf9-217">Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="00cf9-217">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="00cf9-218">enabled</span><span class="sxs-lookup"><span data-stu-id="00cf9-218">enabled</span></span>|<span data-ttu-id="00cf9-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="00cf9-219">Boolean</span></span>|<span data-ttu-id="00cf9-220">Habilita o modo de PC compartilhado e aplica as políticas de PC compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="00cf9-220">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="00cf9-221">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="00cf9-221">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="00cf9-222">Int32</span><span class="sxs-lookup"><span data-stu-id="00cf9-222">Int32</span></span>|<span data-ttu-id="00cf9-223">Especifica o tempo em segundos que um dispositivo deve ficar ocioso antes de o PC entrar em suspensão.</span><span class="sxs-lookup"><span data-stu-id="00cf9-223">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="00cf9-224">Definir esse valor como 0 impede que o tempo limite de suspensão ocorra.</span><span class="sxs-lookup"><span data-stu-id="00cf9-224">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="00cf9-225">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="00cf9-225">kioskAppDisplayName</span></span>|<span data-ttu-id="00cf9-226">String</span><span class="sxs-lookup"><span data-stu-id="00cf9-226">String</span></span>|<span data-ttu-id="00cf9-227">Especifica o texto de exibição para a conta mostrada na tela de entrada que inicializa o aplicativo especificado por SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="00cf9-227">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="00cf9-228">Aplicável somente quando KioskAppUserModelId está definido.</span><span class="sxs-lookup"><span data-stu-id="00cf9-228">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="00cf9-229">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="00cf9-229">kioskAppUserModelId</span></span>|<span data-ttu-id="00cf9-230">String</span><span class="sxs-lookup"><span data-stu-id="00cf9-230">String</span></span>|<span data-ttu-id="00cf9-231">Especifica a ID do modelo de usuário do aplicativo para uso com acesso atribuído.</span><span class="sxs-lookup"><span data-stu-id="00cf9-231">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="00cf9-232">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="00cf9-232">maintenanceStartTime</span></span>|<span data-ttu-id="00cf9-233">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="00cf9-233">TimeOfDay</span></span>|<span data-ttu-id="00cf9-234">Especifica o horário de início diário da hora de manutenção.</span><span class="sxs-lookup"><span data-stu-id="00cf9-234">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="00cf9-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="00cf9-235">Response</span></span>
<span data-ttu-id="00cf9-236">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00cf9-236">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00cf9-237">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00cf9-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="00cf9-238">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00cf9-238">Request</span></span>
<span data-ttu-id="00cf9-239">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="00cf9-239">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="00cf9-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="00cf9-240">Response</span></span>
<span data-ttu-id="00cf9-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00cf9-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




