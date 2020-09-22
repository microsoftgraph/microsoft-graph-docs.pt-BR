---
title: Criar sharedPCConfiguration
description: Cria um novo objeto sharedPCConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 15fc74514587190f2ead79bd2b5af6546ac2047e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028032"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="75cf1-103">Criar sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="75cf1-103">Create sharedPCConfiguration</span></span>

<span data-ttu-id="75cf1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75cf1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75cf1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75cf1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75cf1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75cf1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75cf1-107">Cria um novo objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="75cf1-107">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75cf1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="75cf1-108">Prerequisites</span></span>
<span data-ttu-id="75cf1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75cf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75cf1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75cf1-111">Permission type</span></span>|<span data-ttu-id="75cf1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="75cf1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75cf1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75cf1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75cf1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75cf1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75cf1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75cf1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75cf1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75cf1-116">Not supported.</span></span>|
|<span data-ttu-id="75cf1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75cf1-117">Application</span></span>|<span data-ttu-id="75cf1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75cf1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75cf1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75cf1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="75cf1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75cf1-120">Request headers</span></span>
|<span data-ttu-id="75cf1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75cf1-121">Header</span></span>|<span data-ttu-id="75cf1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="75cf1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75cf1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="75cf1-123">Authorization</span></span>|<span data-ttu-id="75cf1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75cf1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75cf1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="75cf1-125">Accept</span></span>|<span data-ttu-id="75cf1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75cf1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75cf1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75cf1-127">Request body</span></span>
<span data-ttu-id="75cf1-128">No corpo da solicitação, forneça uma representação JSON do objeto sharedPCConfiguration.</span><span class="sxs-lookup"><span data-stu-id="75cf1-128">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="75cf1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar sharedPCConfiguration.</span><span class="sxs-lookup"><span data-stu-id="75cf1-129">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="75cf1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75cf1-130">Property</span></span>|<span data-ttu-id="75cf1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="75cf1-131">Type</span></span>|<span data-ttu-id="75cf1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="75cf1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75cf1-133">id</span><span class="sxs-lookup"><span data-stu-id="75cf1-133">id</span></span>|<span data-ttu-id="75cf1-134">String</span><span class="sxs-lookup"><span data-stu-id="75cf1-134">String</span></span>|<span data-ttu-id="75cf1-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="75cf1-135">Key of the entity.</span></span> <span data-ttu-id="75cf1-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75cf1-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75cf1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75cf1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="75cf1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75cf1-138">DateTimeOffset</span></span>|<span data-ttu-id="75cf1-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="75cf1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="75cf1-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75cf1-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75cf1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="75cf1-141">roleScopeTagIds</span></span>|<span data-ttu-id="75cf1-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="75cf1-142">String collection</span></span>|<span data-ttu-id="75cf1-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="75cf1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="75cf1-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75cf1-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75cf1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="75cf1-145">supportsScopeTags</span></span>|<span data-ttu-id="75cf1-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="75cf1-146">Boolean</span></span>|<span data-ttu-id="75cf1-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="75cf1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="75cf1-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="75cf1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="75cf1-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="75cf1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="75cf1-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="75cf1-150">This property is read-only.</span></span> <span data-ttu-id="75cf1-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75cf1-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75cf1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="75cf1-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="75cf1-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="75cf1-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="75cf1-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="75cf1-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="75cf1-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75cf1-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75cf1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="75cf1-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="75cf1-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="75cf1-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="75cf1-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="75cf1-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="75cf1-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75cf1-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75cf1-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="75cf1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="75cf1-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="75cf1-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="75cf1-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="75cf1-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="75cf1-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75cf1-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75cf1-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75cf1-164">createdDateTime</span></span>|<span data-ttu-id="75cf1-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75cf1-165">DateTimeOffset</span></span>|<span data-ttu-id="75cf1-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="75cf1-166">DateTime the object was created.</span></span> <span data-ttu-id="75cf1-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75cf1-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75cf1-168">description</span><span class="sxs-lookup"><span data-stu-id="75cf1-168">description</span></span>|<span data-ttu-id="75cf1-169">String</span><span class="sxs-lookup"><span data-stu-id="75cf1-169">String</span></span>|<span data-ttu-id="75cf1-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75cf1-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="75cf1-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75cf1-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75cf1-172">displayName</span><span class="sxs-lookup"><span data-stu-id="75cf1-172">displayName</span></span>|<span data-ttu-id="75cf1-173">String</span><span class="sxs-lookup"><span data-stu-id="75cf1-173">String</span></span>|<span data-ttu-id="75cf1-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75cf1-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="75cf1-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75cf1-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75cf1-176">versão</span><span class="sxs-lookup"><span data-stu-id="75cf1-176">version</span></span>|<span data-ttu-id="75cf1-177">Int32</span><span class="sxs-lookup"><span data-stu-id="75cf1-177">Int32</span></span>|<span data-ttu-id="75cf1-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75cf1-178">Version of the device configuration.</span></span> <span data-ttu-id="75cf1-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75cf1-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75cf1-180">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="75cf1-180">accountManagerPolicy</span></span>|[<span data-ttu-id="75cf1-181">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="75cf1-181">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="75cf1-182">Especifica como as contas são gerenciadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="75cf1-182">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="75cf1-183">Aplica-se somente quando disableAccountManager é false.</span><span class="sxs-lookup"><span data-stu-id="75cf1-183">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="75cf1-184">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="75cf1-184">allowedAccounts</span></span>|[<span data-ttu-id="75cf1-185">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="75cf1-185">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="75cf1-186">Indica que tipos de contas podem ser usadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="75cf1-186">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="75cf1-187">Os valores possíveis são: `notConfigured`, `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="75cf1-187">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="75cf1-188">localStorage</span><span class="sxs-lookup"><span data-stu-id="75cf1-188">localStorage</span></span>|[<span data-ttu-id="75cf1-189">habilitação</span><span class="sxs-lookup"><span data-stu-id="75cf1-189">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="75cf1-190">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="75cf1-190">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="75cf1-191">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="75cf1-191">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="75cf1-192">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="75cf1-192">allowLocalStorage</span></span>|<span data-ttu-id="75cf1-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="75cf1-193">Boolean</span></span>|<span data-ttu-id="75cf1-194">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="75cf1-194">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="75cf1-195">setaccountmanager</span><span class="sxs-lookup"><span data-stu-id="75cf1-195">setAccountManager</span></span>|[<span data-ttu-id="75cf1-196">habilitação</span><span class="sxs-lookup"><span data-stu-id="75cf1-196">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="75cf1-197">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="75cf1-197">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="75cf1-198">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="75cf1-198">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="75cf1-199">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="75cf1-199">disableAccountManager</span></span>|<span data-ttu-id="75cf1-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="75cf1-200">Boolean</span></span>|<span data-ttu-id="75cf1-201">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="75cf1-201">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="75cf1-202">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="75cf1-202">setEduPolicies</span></span>|[<span data-ttu-id="75cf1-203">habilitação</span><span class="sxs-lookup"><span data-stu-id="75cf1-203">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="75cf1-204">Especifica se as políticas de ambiente de educação de computador compartilhado padrão devem ser habilitadas/desabilitadas/não configuradas.</span><span class="sxs-lookup"><span data-stu-id="75cf1-204">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="75cf1-205">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="75cf1-205">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="75cf1-206">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="75cf1-206">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="75cf1-207">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="75cf1-207">disableEduPolicies</span></span>|<span data-ttu-id="75cf1-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="75cf1-208">Boolean</span></span>|<span data-ttu-id="75cf1-209">Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="75cf1-209">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="75cf1-210">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="75cf1-210">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="75cf1-211">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="75cf1-211">setPowerPolicies</span></span>|[<span data-ttu-id="75cf1-212">habilitação</span><span class="sxs-lookup"><span data-stu-id="75cf1-212">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="75cf1-213">Especifica se as políticas de energia padrão do computador compartilhado devem ser ativadas/desativadas.</span><span class="sxs-lookup"><span data-stu-id="75cf1-213">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="75cf1-214">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="75cf1-214">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="75cf1-215">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="75cf1-215">disablePowerPolicies</span></span>|<span data-ttu-id="75cf1-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="75cf1-216">Boolean</span></span>|<span data-ttu-id="75cf1-217">Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="75cf1-217">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="75cf1-218">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="75cf1-218">signInOnResume</span></span>|[<span data-ttu-id="75cf1-219">habilitação</span><span class="sxs-lookup"><span data-stu-id="75cf1-219">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="75cf1-220">Especifica o requisito para entrar sempre que o dispositivo é ativado do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="75cf1-220">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="75cf1-221">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="75cf1-221">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="75cf1-222">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="75cf1-222">disableSignInOnResume</span></span>|<span data-ttu-id="75cf1-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="75cf1-223">Boolean</span></span>|<span data-ttu-id="75cf1-224">Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="75cf1-224">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="75cf1-225">enabled</span><span class="sxs-lookup"><span data-stu-id="75cf1-225">enabled</span></span>|<span data-ttu-id="75cf1-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="75cf1-226">Boolean</span></span>|<span data-ttu-id="75cf1-227">Habilita o modo de PC compartilhado e aplica as políticas de PC compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="75cf1-227">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="75cf1-228">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="75cf1-228">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="75cf1-229">Int32</span><span class="sxs-lookup"><span data-stu-id="75cf1-229">Int32</span></span>|<span data-ttu-id="75cf1-230">Especifica o tempo em segundos que um dispositivo deve ficar ocioso antes de o PC entrar em suspensão.</span><span class="sxs-lookup"><span data-stu-id="75cf1-230">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="75cf1-231">Definir esse valor como 0 impede que o tempo limite de suspensão ocorra.</span><span class="sxs-lookup"><span data-stu-id="75cf1-231">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="75cf1-232">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="75cf1-232">kioskAppDisplayName</span></span>|<span data-ttu-id="75cf1-233">String</span><span class="sxs-lookup"><span data-stu-id="75cf1-233">String</span></span>|<span data-ttu-id="75cf1-234">Especifica o texto de exibição para a conta mostrada na tela de entrada que inicializa o aplicativo especificado por SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="75cf1-234">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="75cf1-235">Aplicável somente quando KioskAppUserModelId está definido.</span><span class="sxs-lookup"><span data-stu-id="75cf1-235">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="75cf1-236">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="75cf1-236">kioskAppUserModelId</span></span>|<span data-ttu-id="75cf1-237">String</span><span class="sxs-lookup"><span data-stu-id="75cf1-237">String</span></span>|<span data-ttu-id="75cf1-238">Especifica a ID do modelo de usuário do aplicativo para uso com acesso atribuído.</span><span class="sxs-lookup"><span data-stu-id="75cf1-238">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="75cf1-239">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="75cf1-239">maintenanceStartTime</span></span>|<span data-ttu-id="75cf1-240">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="75cf1-240">TimeOfDay</span></span>|<span data-ttu-id="75cf1-241">Especifica o horário de início diário da hora de manutenção.</span><span class="sxs-lookup"><span data-stu-id="75cf1-241">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="75cf1-242">fastFirstSignIn</span><span class="sxs-lookup"><span data-stu-id="75cf1-242">fastFirstSignIn</span></span>|[<span data-ttu-id="75cf1-243">habilitação</span><span class="sxs-lookup"><span data-stu-id="75cf1-243">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="75cf1-244">Especifica se a conexão automática de novas contas não administrativas do Azure AD para contas locais de candidatos pré-configuradas.</span><span class="sxs-lookup"><span data-stu-id="75cf1-244">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="75cf1-245">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="75cf1-245">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="75cf1-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="75cf1-246">Response</span></span>
<span data-ttu-id="75cf1-247">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75cf1-247">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75cf1-248">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75cf1-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="75cf1-249">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75cf1-249">Request</span></span>
<span data-ttu-id="75cf1-250">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75cf1-250">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="75cf1-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="75cf1-251">Response</span></span>
<span data-ttu-id="75cf1-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75cf1-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






