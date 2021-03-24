---
title: Atualizar sharedPCConfiguration
description: Atualiza as propriedades de um objeto sharedPCConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0ed8402d459a750f120754a5e33a087656de958b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137081"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="db366-103">Atualizar sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="db366-103">Update sharedPCConfiguration</span></span>

<span data-ttu-id="db366-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db366-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db366-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="db366-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db366-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="db366-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db366-107">Atualiza as propriedades de um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db366-107">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db366-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="db366-108">Prerequisites</span></span>
<span data-ttu-id="db366-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db366-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db366-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db366-111">Permission type</span></span>|<span data-ttu-id="db366-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db366-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db366-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db366-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db366-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db366-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="db366-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db366-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db366-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db366-116">Not supported.</span></span>|
|<span data-ttu-id="db366-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db366-117">Application</span></span>|<span data-ttu-id="db366-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db366-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db366-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db366-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="db366-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db366-120">Request headers</span></span>
|<span data-ttu-id="db366-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db366-121">Header</span></span>|<span data-ttu-id="db366-122">Valor</span><span class="sxs-lookup"><span data-stu-id="db366-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db366-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="db366-123">Authorization</span></span>|<span data-ttu-id="db366-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db366-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db366-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="db366-125">Accept</span></span>|<span data-ttu-id="db366-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db366-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db366-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db366-127">Request body</span></span>
<span data-ttu-id="db366-128">No corpo da solicitação, forneça uma representação JSON do objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db366-128">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="db366-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db366-129">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="db366-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db366-130">Property</span></span>|<span data-ttu-id="db366-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="db366-131">Type</span></span>|<span data-ttu-id="db366-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="db366-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db366-133">id</span><span class="sxs-lookup"><span data-stu-id="db366-133">id</span></span>|<span data-ttu-id="db366-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db366-134">String</span></span>|<span data-ttu-id="db366-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="db366-135">Key of the entity.</span></span> <span data-ttu-id="db366-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db366-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db366-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db366-137">lastModifiedDateTime</span></span>|<span data-ttu-id="db366-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db366-138">DateTimeOffset</span></span>|<span data-ttu-id="db366-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="db366-139">DateTime the object was last modified.</span></span> <span data-ttu-id="db366-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db366-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db366-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="db366-141">roleScopeTagIds</span></span>|<span data-ttu-id="db366-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="db366-142">String collection</span></span>|<span data-ttu-id="db366-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="db366-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="db366-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db366-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db366-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="db366-145">supportsScopeTags</span></span>|<span data-ttu-id="db366-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="db366-146">Boolean</span></span>|<span data-ttu-id="db366-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="db366-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="db366-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="db366-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="db366-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="db366-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="db366-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="db366-150">This property is read-only.</span></span> <span data-ttu-id="db366-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db366-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db366-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="db366-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="db366-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="db366-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="db366-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="db366-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="db366-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db366-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db366-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="db366-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="db366-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="db366-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="db366-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="db366-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="db366-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db366-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db366-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="db366-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="db366-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="db366-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="db366-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="db366-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="db366-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db366-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db366-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db366-164">createdDateTime</span></span>|<span data-ttu-id="db366-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db366-165">DateTimeOffset</span></span>|<span data-ttu-id="db366-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="db366-166">DateTime the object was created.</span></span> <span data-ttu-id="db366-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db366-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db366-168">descrição</span><span class="sxs-lookup"><span data-stu-id="db366-168">description</span></span>|<span data-ttu-id="db366-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db366-169">String</span></span>|<span data-ttu-id="db366-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db366-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="db366-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db366-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db366-172">displayName</span><span class="sxs-lookup"><span data-stu-id="db366-172">displayName</span></span>|<span data-ttu-id="db366-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db366-173">String</span></span>|<span data-ttu-id="db366-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db366-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="db366-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db366-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db366-176">versão</span><span class="sxs-lookup"><span data-stu-id="db366-176">version</span></span>|<span data-ttu-id="db366-177">Int32</span><span class="sxs-lookup"><span data-stu-id="db366-177">Int32</span></span>|<span data-ttu-id="db366-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db366-178">Version of the device configuration.</span></span> <span data-ttu-id="db366-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db366-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db366-180">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="db366-180">accountManagerPolicy</span></span>|[<span data-ttu-id="db366-181">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="db366-181">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="db366-182">Especifica como as contas são gerenciadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="db366-182">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="db366-183">Aplica-se somente quando disableAccountManager é false.</span><span class="sxs-lookup"><span data-stu-id="db366-183">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="db366-184">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="db366-184">allowedAccounts</span></span>|[<span data-ttu-id="db366-185">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="db366-185">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="db366-186">Indica que tipos de contas podem ser usadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="db366-186">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="db366-187">Os valores possíveis são: `notConfigured`, `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="db366-187">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="db366-188">localStorage</span><span class="sxs-lookup"><span data-stu-id="db366-188">localStorage</span></span>|[<span data-ttu-id="db366-189">enablement</span><span class="sxs-lookup"><span data-stu-id="db366-189">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="db366-190">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="db366-190">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="db366-191">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="db366-191">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="db366-192">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="db366-192">allowLocalStorage</span></span>|<span data-ttu-id="db366-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="db366-193">Boolean</span></span>|<span data-ttu-id="db366-194">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="db366-194">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="db366-195">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="db366-195">setAccountManager</span></span>|[<span data-ttu-id="db366-196">enablement</span><span class="sxs-lookup"><span data-stu-id="db366-196">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="db366-197">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="db366-197">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="db366-198">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="db366-198">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="db366-199">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="db366-199">disableAccountManager</span></span>|<span data-ttu-id="db366-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="db366-200">Boolean</span></span>|<span data-ttu-id="db366-201">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="db366-201">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="db366-202">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="db366-202">setEduPolicies</span></span>|[<span data-ttu-id="db366-203">enablement</span><span class="sxs-lookup"><span data-stu-id="db366-203">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="db366-204">Especifica se as políticas de ambiente de educação do computador compartilhado padrão devem ser habilitadas/desabilitadas/não configuradas.</span><span class="sxs-lookup"><span data-stu-id="db366-204">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="db366-205">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="db366-205">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="db366-206">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="db366-206">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="db366-207">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="db366-207">disableEduPolicies</span></span>|<span data-ttu-id="db366-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="db366-208">Boolean</span></span>|<span data-ttu-id="db366-209">Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="db366-209">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="db366-210">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="db366-210">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="db366-211">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="db366-211">setPowerPolicies</span></span>|[<span data-ttu-id="db366-212">enablement</span><span class="sxs-lookup"><span data-stu-id="db366-212">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="db366-213">Especifica se as políticas de energia do computador compartilhado padrão devem ser habilitadas/desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="db366-213">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="db366-214">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="db366-214">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="db366-215">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="db366-215">disablePowerPolicies</span></span>|<span data-ttu-id="db366-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="db366-216">Boolean</span></span>|<span data-ttu-id="db366-217">Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="db366-217">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="db366-218">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="db366-218">signInOnResume</span></span>|[<span data-ttu-id="db366-219">enablement</span><span class="sxs-lookup"><span data-stu-id="db366-219">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="db366-220">Especifica o requisito de entrar sempre que o dispositivo acordar do modo de sono.</span><span class="sxs-lookup"><span data-stu-id="db366-220">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="db366-221">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="db366-221">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="db366-222">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="db366-222">disableSignInOnResume</span></span>|<span data-ttu-id="db366-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="db366-223">Boolean</span></span>|<span data-ttu-id="db366-224">Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="db366-224">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="db366-225">enabled</span><span class="sxs-lookup"><span data-stu-id="db366-225">enabled</span></span>|<span data-ttu-id="db366-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="db366-226">Boolean</span></span>|<span data-ttu-id="db366-227">Habilita o modo de PC compartilhado e aplica as políticas de PC compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="db366-227">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="db366-228">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="db366-228">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="db366-229">Int32</span><span class="sxs-lookup"><span data-stu-id="db366-229">Int32</span></span>|<span data-ttu-id="db366-230">Especifica o tempo em segundos que um dispositivo deve ficar ocioso antes de o PC entrar em suspensão.</span><span class="sxs-lookup"><span data-stu-id="db366-230">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="db366-231">Definir esse valor como 0 impede que o tempo limite de suspensão ocorra.</span><span class="sxs-lookup"><span data-stu-id="db366-231">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="db366-232">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="db366-232">kioskAppDisplayName</span></span>|<span data-ttu-id="db366-233">String</span><span class="sxs-lookup"><span data-stu-id="db366-233">String</span></span>|<span data-ttu-id="db366-234">Especifica o texto de exibição para a conta mostrada na tela de entrada que inicializa o aplicativo especificado por SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="db366-234">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="db366-235">Aplicável somente quando KioskAppUserModelId está definido.</span><span class="sxs-lookup"><span data-stu-id="db366-235">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="db366-236">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="db366-236">kioskAppUserModelId</span></span>|<span data-ttu-id="db366-237">String</span><span class="sxs-lookup"><span data-stu-id="db366-237">String</span></span>|<span data-ttu-id="db366-238">Especifica a ID do modelo de usuário do aplicativo para uso com acesso atribuído.</span><span class="sxs-lookup"><span data-stu-id="db366-238">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="db366-239">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="db366-239">maintenanceStartTime</span></span>|<span data-ttu-id="db366-240">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="db366-240">TimeOfDay</span></span>|<span data-ttu-id="db366-241">Especifica o horário de início diário da hora de manutenção.</span><span class="sxs-lookup"><span data-stu-id="db366-241">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="db366-242">fastFirstSignIn</span><span class="sxs-lookup"><span data-stu-id="db366-242">fastFirstSignIn</span></span>|[<span data-ttu-id="db366-243">enablement</span><span class="sxs-lookup"><span data-stu-id="db366-243">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="db366-244">Especifica se as novas contas não administrativas do Azure AD serão conectadas automaticamente a contas locais de candidatos pré-configurados.</span><span class="sxs-lookup"><span data-stu-id="db366-244">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="db366-245">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="db366-245">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="db366-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="db366-246">Response</span></span>
<span data-ttu-id="db366-247">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db366-247">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db366-248">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db366-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="db366-249">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db366-249">Request</span></span>
<span data-ttu-id="db366-250">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db366-250">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1920

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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

### <a name="response"></a><span data-ttu-id="db366-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="db366-251">Response</span></span>
<span data-ttu-id="db366-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db366-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2092

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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




