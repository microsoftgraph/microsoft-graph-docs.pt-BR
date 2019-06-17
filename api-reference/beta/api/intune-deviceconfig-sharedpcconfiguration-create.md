---
title: Criar sharedPCConfiguration
description: Cria um novo objeto sharedPCConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6efb3225f750581babd035fb044e130ed1b5a84
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34962880"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="06d14-103">Criar sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="06d14-103">Create sharedPCConfiguration</span></span>

> <span data-ttu-id="06d14-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="06d14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06d14-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06d14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06d14-106">Cria um novo objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06d14-106">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06d14-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06d14-107">Prerequisites</span></span>
<span data-ttu-id="06d14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06d14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06d14-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06d14-110">Permission type</span></span>|<span data-ttu-id="06d14-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06d14-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06d14-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06d14-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06d14-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06d14-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06d14-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06d14-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06d14-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06d14-115">Not supported.</span></span>|
|<span data-ttu-id="06d14-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06d14-116">Application</span></span>|<span data-ttu-id="06d14-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06d14-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06d14-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06d14-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="06d14-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06d14-119">Request headers</span></span>
|<span data-ttu-id="06d14-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06d14-120">Header</span></span>|<span data-ttu-id="06d14-121">Valor</span><span class="sxs-lookup"><span data-stu-id="06d14-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06d14-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="06d14-122">Authorization</span></span>|<span data-ttu-id="06d14-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06d14-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06d14-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06d14-124">Accept</span></span>|<span data-ttu-id="06d14-125">application/json</span><span class="sxs-lookup"><span data-stu-id="06d14-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06d14-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06d14-126">Request body</span></span>
<span data-ttu-id="06d14-127">No corpo da solicitação, forneça uma representação JSON do objeto sharedPCConfiguration.</span><span class="sxs-lookup"><span data-stu-id="06d14-127">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="06d14-128">A tabela a seguir mostra as propriedades que são necessárias ao criar sharedPCConfiguration.</span><span class="sxs-lookup"><span data-stu-id="06d14-128">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="06d14-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06d14-129">Property</span></span>|<span data-ttu-id="06d14-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="06d14-130">Type</span></span>|<span data-ttu-id="06d14-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="06d14-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06d14-132">id</span><span class="sxs-lookup"><span data-stu-id="06d14-132">id</span></span>|<span data-ttu-id="06d14-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06d14-133">String</span></span>|<span data-ttu-id="06d14-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="06d14-134">Key of the entity.</span></span> <span data-ttu-id="06d14-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06d14-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06d14-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06d14-136">lastModifiedDateTime</span></span>|<span data-ttu-id="06d14-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06d14-137">DateTimeOffset</span></span>|<span data-ttu-id="06d14-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="06d14-138">DateTime the object was last modified.</span></span> <span data-ttu-id="06d14-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06d14-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06d14-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="06d14-140">roleScopeTagIds</span></span>|<span data-ttu-id="06d14-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="06d14-141">String collection</span></span>|<span data-ttu-id="06d14-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="06d14-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="06d14-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06d14-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06d14-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="06d14-144">supportsScopeTags</span></span>|<span data-ttu-id="06d14-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="06d14-145">Boolean</span></span>|<span data-ttu-id="06d14-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="06d14-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="06d14-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="06d14-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="06d14-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="06d14-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="06d14-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="06d14-149">This property is read-only.</span></span> <span data-ttu-id="06d14-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06d14-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06d14-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="06d14-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="06d14-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="06d14-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="06d14-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="06d14-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="06d14-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06d14-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06d14-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="06d14-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="06d14-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="06d14-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="06d14-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="06d14-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="06d14-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06d14-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06d14-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="06d14-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="06d14-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="06d14-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="06d14-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="06d14-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="06d14-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06d14-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06d14-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06d14-163">createdDateTime</span></span>|<span data-ttu-id="06d14-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06d14-164">DateTimeOffset</span></span>|<span data-ttu-id="06d14-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="06d14-165">DateTime the object was created.</span></span> <span data-ttu-id="06d14-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06d14-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06d14-167">descrição</span><span class="sxs-lookup"><span data-stu-id="06d14-167">description</span></span>|<span data-ttu-id="06d14-168">String</span><span class="sxs-lookup"><span data-stu-id="06d14-168">String</span></span>|<span data-ttu-id="06d14-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06d14-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="06d14-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06d14-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06d14-171">displayName</span><span class="sxs-lookup"><span data-stu-id="06d14-171">displayName</span></span>|<span data-ttu-id="06d14-172">String</span><span class="sxs-lookup"><span data-stu-id="06d14-172">String</span></span>|<span data-ttu-id="06d14-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06d14-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="06d14-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06d14-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06d14-175">versão</span><span class="sxs-lookup"><span data-stu-id="06d14-175">version</span></span>|<span data-ttu-id="06d14-176">Int32</span><span class="sxs-lookup"><span data-stu-id="06d14-176">Int32</span></span>|<span data-ttu-id="06d14-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06d14-177">Version of the device configuration.</span></span> <span data-ttu-id="06d14-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06d14-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06d14-179">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="06d14-179">accountManagerPolicy</span></span>|[<span data-ttu-id="06d14-180">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="06d14-180">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="06d14-181">Especifica como as contas são gerenciadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="06d14-181">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="06d14-182">Aplica-se somente quando disableAccountManager é false.</span><span class="sxs-lookup"><span data-stu-id="06d14-182">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="06d14-183">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="06d14-183">allowedAccounts</span></span>|[<span data-ttu-id="06d14-184">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="06d14-184">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="06d14-185">Indica que tipos de contas podem ser usadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="06d14-185">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="06d14-186">Os valores possíveis são: `notConfigured`, `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="06d14-186">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="06d14-187">localStorage</span><span class="sxs-lookup"><span data-stu-id="06d14-187">localStorage</span></span>|[<span data-ttu-id="06d14-188">habilitação</span><span class="sxs-lookup"><span data-stu-id="06d14-188">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="06d14-189">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="06d14-189">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="06d14-190">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="06d14-190">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="06d14-191">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="06d14-191">allowLocalStorage</span></span>|<span data-ttu-id="06d14-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="06d14-192">Boolean</span></span>|<span data-ttu-id="06d14-193">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="06d14-193">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="06d14-194">setaccountmanager</span><span class="sxs-lookup"><span data-stu-id="06d14-194">setAccountManager</span></span>|[<span data-ttu-id="06d14-195">habilitação</span><span class="sxs-lookup"><span data-stu-id="06d14-195">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="06d14-196">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="06d14-196">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="06d14-197">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="06d14-197">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="06d14-198">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="06d14-198">disableAccountManager</span></span>|<span data-ttu-id="06d14-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="06d14-199">Boolean</span></span>|<span data-ttu-id="06d14-200">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="06d14-200">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="06d14-201">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="06d14-201">setEduPolicies</span></span>|[<span data-ttu-id="06d14-202">habilitação</span><span class="sxs-lookup"><span data-stu-id="06d14-202">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="06d14-203">Especifica se as políticas de ambiente de educação de computador compartilhado padrão devem ser habilitadas/desabilitadas/não configuradas.</span><span class="sxs-lookup"><span data-stu-id="06d14-203">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="06d14-204">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="06d14-204">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="06d14-205">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="06d14-205">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="06d14-206">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="06d14-206">disableEduPolicies</span></span>|<span data-ttu-id="06d14-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="06d14-207">Boolean</span></span>|<span data-ttu-id="06d14-208">Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="06d14-208">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="06d14-209">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="06d14-209">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="06d14-210">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="06d14-210">setPowerPolicies</span></span>|[<span data-ttu-id="06d14-211">habilitação</span><span class="sxs-lookup"><span data-stu-id="06d14-211">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="06d14-212">Especifica se as políticas de energia padrão do computador compartilhado devem ser ativadas/desativadas.</span><span class="sxs-lookup"><span data-stu-id="06d14-212">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="06d14-213">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="06d14-213">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="06d14-214">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="06d14-214">disablePowerPolicies</span></span>|<span data-ttu-id="06d14-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="06d14-215">Boolean</span></span>|<span data-ttu-id="06d14-216">Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="06d14-216">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="06d14-217">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="06d14-217">signInOnResume</span></span>|[<span data-ttu-id="06d14-218">habilitação</span><span class="sxs-lookup"><span data-stu-id="06d14-218">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="06d14-219">Especifica o requisito para entrar sempre que o dispositivo é ativado do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="06d14-219">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="06d14-220">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="06d14-220">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="06d14-221">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="06d14-221">disableSignInOnResume</span></span>|<span data-ttu-id="06d14-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="06d14-222">Boolean</span></span>|<span data-ttu-id="06d14-223">Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="06d14-223">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="06d14-224">enabled</span><span class="sxs-lookup"><span data-stu-id="06d14-224">enabled</span></span>|<span data-ttu-id="06d14-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="06d14-225">Boolean</span></span>|<span data-ttu-id="06d14-226">Habilita o modo de PC compartilhado e aplica as políticas de PC compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="06d14-226">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="06d14-227">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="06d14-227">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="06d14-228">Int32</span><span class="sxs-lookup"><span data-stu-id="06d14-228">Int32</span></span>|<span data-ttu-id="06d14-229">Especifica o tempo em segundos que um dispositivo deve ficar ocioso antes de o PC entrar em suspensão.</span><span class="sxs-lookup"><span data-stu-id="06d14-229">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="06d14-230">Definir esse valor como 0 impede que o tempo limite de suspensão ocorra.</span><span class="sxs-lookup"><span data-stu-id="06d14-230">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="06d14-231">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="06d14-231">kioskAppDisplayName</span></span>|<span data-ttu-id="06d14-232">String</span><span class="sxs-lookup"><span data-stu-id="06d14-232">String</span></span>|<span data-ttu-id="06d14-233">Especifica o texto de exibição para a conta mostrada na tela de entrada que inicializa o aplicativo especificado por SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="06d14-233">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="06d14-234">Aplicável somente quando KioskAppUserModelId está definido.</span><span class="sxs-lookup"><span data-stu-id="06d14-234">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="06d14-235">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="06d14-235">kioskAppUserModelId</span></span>|<span data-ttu-id="06d14-236">String</span><span class="sxs-lookup"><span data-stu-id="06d14-236">String</span></span>|<span data-ttu-id="06d14-237">Especifica a ID do modelo de usuário do aplicativo para uso com acesso atribuído.</span><span class="sxs-lookup"><span data-stu-id="06d14-237">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="06d14-238">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="06d14-238">maintenanceStartTime</span></span>|<span data-ttu-id="06d14-239">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="06d14-239">TimeOfDay</span></span>|<span data-ttu-id="06d14-240">Especifica o horário de início diário da hora de manutenção.</span><span class="sxs-lookup"><span data-stu-id="06d14-240">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="06d14-241">fastFirstSignIn</span><span class="sxs-lookup"><span data-stu-id="06d14-241">fastFirstSignIn</span></span>|[<span data-ttu-id="06d14-242">habilitação</span><span class="sxs-lookup"><span data-stu-id="06d14-242">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="06d14-243">Especifica se a conexão automática de novas contas não administrativas do Azure AD para contas locais de candidatos pré-configuradas.</span><span class="sxs-lookup"><span data-stu-id="06d14-243">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="06d14-244">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="06d14-244">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="06d14-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="06d14-245">Response</span></span>
<span data-ttu-id="06d14-246">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06d14-246">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06d14-247">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06d14-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="06d14-248">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06d14-248">Request</span></span>
<span data-ttu-id="06d14-249">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06d14-249">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="06d14-250">Resposta</span><span class="sxs-lookup"><span data-stu-id="06d14-250">Response</span></span>
<span data-ttu-id="06d14-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06d14-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





