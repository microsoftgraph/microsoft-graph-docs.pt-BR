---
title: Atualizar sharedPCConfiguration
description: Atualiza as propriedades de um objeto sharedPCConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f85f4896448a0fab47c1771f661cc84d085bead8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34962795"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="4d7c3-103">Atualizar sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="4d7c3-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="4d7c3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d7c3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d7c3-106">Atualiza as propriedades de um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4d7c3-106">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d7c3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4d7c3-107">Prerequisites</span></span>
<span data-ttu-id="4d7c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d7c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d7c3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d7c3-110">Permission type</span></span>|<span data-ttu-id="4d7c3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4d7c3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d7c3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d7c3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4d7c3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d7c3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4d7c3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d7c3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d7c3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-115">Not supported.</span></span>|
|<span data-ttu-id="4d7c3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d7c3-116">Application</span></span>|<span data-ttu-id="4d7c3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d7c3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d7c3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4d7c3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d7c3-119">Request headers</span></span>
|<span data-ttu-id="4d7c3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4d7c3-120">Header</span></span>|<span data-ttu-id="4d7c3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4d7c3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d7c3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d7c3-122">Authorization</span></span>|<span data-ttu-id="4d7c3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d7c3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4d7c3-124">Accept</span></span>|<span data-ttu-id="4d7c3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4d7c3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d7c3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d7c3-126">Request body</span></span>
<span data-ttu-id="4d7c3-127">No corpo da solicitação, forneça uma representação JSON do objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4d7c3-127">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="4d7c3-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4d7c3-128">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="4d7c3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d7c3-129">Property</span></span>|<span data-ttu-id="4d7c3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d7c3-130">Type</span></span>|<span data-ttu-id="4d7c3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d7c3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d7c3-132">id</span><span class="sxs-lookup"><span data-stu-id="4d7c3-132">id</span></span>|<span data-ttu-id="4d7c3-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d7c3-133">String</span></span>|<span data-ttu-id="4d7c3-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-134">Key of the entity.</span></span> <span data-ttu-id="4d7c3-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d7c3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d7c3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d7c3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4d7c3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d7c3-137">DateTimeOffset</span></span>|<span data-ttu-id="4d7c3-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4d7c3-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d7c3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d7c3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4d7c3-140">roleScopeTagIds</span></span>|<span data-ttu-id="4d7c3-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d7c3-141">String collection</span></span>|<span data-ttu-id="4d7c3-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4d7c3-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d7c3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d7c3-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4d7c3-144">supportsScopeTags</span></span>|<span data-ttu-id="4d7c3-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="4d7c3-145">Boolean</span></span>|<span data-ttu-id="4d7c3-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4d7c3-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4d7c3-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4d7c3-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-149">This property is read-only.</span></span> <span data-ttu-id="4d7c3-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d7c3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d7c3-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4d7c3-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4d7c3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4d7c3-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4d7c3-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4d7c3-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d7c3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d7c3-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4d7c3-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4d7c3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4d7c3-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4d7c3-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4d7c3-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d7c3-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d7c3-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4d7c3-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4d7c3-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4d7c3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4d7c3-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4d7c3-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d7c3-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d7c3-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4d7c3-163">createdDateTime</span></span>|<span data-ttu-id="4d7c3-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d7c3-164">DateTimeOffset</span></span>|<span data-ttu-id="4d7c3-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-165">DateTime the object was created.</span></span> <span data-ttu-id="4d7c3-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d7c3-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d7c3-167">descrição</span><span class="sxs-lookup"><span data-stu-id="4d7c3-167">description</span></span>|<span data-ttu-id="4d7c3-168">String</span><span class="sxs-lookup"><span data-stu-id="4d7c3-168">String</span></span>|<span data-ttu-id="4d7c3-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4d7c3-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d7c3-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d7c3-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4d7c3-171">displayName</span></span>|<span data-ttu-id="4d7c3-172">String</span><span class="sxs-lookup"><span data-stu-id="4d7c3-172">String</span></span>|<span data-ttu-id="4d7c3-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4d7c3-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d7c3-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d7c3-175">versão</span><span class="sxs-lookup"><span data-stu-id="4d7c3-175">version</span></span>|<span data-ttu-id="4d7c3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4d7c3-176">Int32</span></span>|<span data-ttu-id="4d7c3-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-177">Version of the device configuration.</span></span> <span data-ttu-id="4d7c3-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d7c3-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d7c3-179">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="4d7c3-179">accountManagerPolicy</span></span>|[<span data-ttu-id="4d7c3-180">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="4d7c3-180">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="4d7c3-181">Especifica como as contas são gerenciadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-181">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="4d7c3-182">Aplica-se somente quando disableAccountManager é false.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-182">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="4d7c3-183">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="4d7c3-183">allowedAccounts</span></span>|[<span data-ttu-id="4d7c3-184">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="4d7c3-184">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="4d7c3-185">Indica que tipos de contas podem ser usadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-185">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="4d7c3-186">Os valores possíveis são: `notConfigured`, `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-186">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="4d7c3-187">localStorage</span><span class="sxs-lookup"><span data-stu-id="4d7c3-187">localStorage</span></span>|[<span data-ttu-id="4d7c3-188">habilitação</span><span class="sxs-lookup"><span data-stu-id="4d7c3-188">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4d7c3-189">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-189">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="4d7c3-190">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-190">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4d7c3-191">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="4d7c3-191">allowLocalStorage</span></span>|<span data-ttu-id="4d7c3-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="4d7c3-192">Boolean</span></span>|<span data-ttu-id="4d7c3-193">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-193">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="4d7c3-194">setaccountmanager</span><span class="sxs-lookup"><span data-stu-id="4d7c3-194">setAccountManager</span></span>|[<span data-ttu-id="4d7c3-195">habilitação</span><span class="sxs-lookup"><span data-stu-id="4d7c3-195">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4d7c3-196">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-196">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="4d7c3-197">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-197">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4d7c3-198">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="4d7c3-198">disableAccountManager</span></span>|<span data-ttu-id="4d7c3-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="4d7c3-199">Boolean</span></span>|<span data-ttu-id="4d7c3-200">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-200">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="4d7c3-201">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="4d7c3-201">setEduPolicies</span></span>|[<span data-ttu-id="4d7c3-202">habilitação</span><span class="sxs-lookup"><span data-stu-id="4d7c3-202">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4d7c3-203">Especifica se as políticas de ambiente de educação de computador compartilhado padrão devem ser habilitadas/desabilitadas/não configuradas.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-203">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="4d7c3-204">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-204">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="4d7c3-205">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-205">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4d7c3-206">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="4d7c3-206">disableEduPolicies</span></span>|<span data-ttu-id="4d7c3-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="4d7c3-207">Boolean</span></span>|<span data-ttu-id="4d7c3-208">Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-208">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="4d7c3-209">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-209">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="4d7c3-210">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="4d7c3-210">setPowerPolicies</span></span>|[<span data-ttu-id="4d7c3-211">habilitação</span><span class="sxs-lookup"><span data-stu-id="4d7c3-211">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4d7c3-212">Especifica se as políticas de energia padrão do computador compartilhado devem ser ativadas/desativadas.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-212">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="4d7c3-213">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-213">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4d7c3-214">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="4d7c3-214">disablePowerPolicies</span></span>|<span data-ttu-id="4d7c3-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="4d7c3-215">Boolean</span></span>|<span data-ttu-id="4d7c3-216">Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-216">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="4d7c3-217">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="4d7c3-217">signInOnResume</span></span>|[<span data-ttu-id="4d7c3-218">habilitação</span><span class="sxs-lookup"><span data-stu-id="4d7c3-218">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4d7c3-219">Especifica o requisito para entrar sempre que o dispositivo é ativado do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-219">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="4d7c3-220">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-220">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4d7c3-221">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="4d7c3-221">disableSignInOnResume</span></span>|<span data-ttu-id="4d7c3-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="4d7c3-222">Boolean</span></span>|<span data-ttu-id="4d7c3-223">Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-223">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="4d7c3-224">enabled</span><span class="sxs-lookup"><span data-stu-id="4d7c3-224">enabled</span></span>|<span data-ttu-id="4d7c3-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d7c3-225">Boolean</span></span>|<span data-ttu-id="4d7c3-226">Habilita o modo de PC compartilhado e aplica as políticas de PC compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-226">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="4d7c3-227">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="4d7c3-227">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="4d7c3-228">Int32</span><span class="sxs-lookup"><span data-stu-id="4d7c3-228">Int32</span></span>|<span data-ttu-id="4d7c3-229">Especifica o tempo em segundos que um dispositivo deve ficar ocioso antes de o PC entrar em suspensão.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-229">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="4d7c3-230">Definir esse valor como 0 impede que o tempo limite de suspensão ocorra.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-230">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="4d7c3-231">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="4d7c3-231">kioskAppDisplayName</span></span>|<span data-ttu-id="4d7c3-232">String</span><span class="sxs-lookup"><span data-stu-id="4d7c3-232">String</span></span>|<span data-ttu-id="4d7c3-233">Especifica o texto de exibição para a conta mostrada na tela de entrada que inicializa o aplicativo especificado por SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-233">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="4d7c3-234">Aplicável somente quando KioskAppUserModelId está definido.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-234">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="4d7c3-235">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="4d7c3-235">kioskAppUserModelId</span></span>|<span data-ttu-id="4d7c3-236">String</span><span class="sxs-lookup"><span data-stu-id="4d7c3-236">String</span></span>|<span data-ttu-id="4d7c3-237">Especifica a ID do modelo de usuário do aplicativo para uso com acesso atribuído.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-237">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="4d7c3-238">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="4d7c3-238">maintenanceStartTime</span></span>|<span data-ttu-id="4d7c3-239">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4d7c3-239">TimeOfDay</span></span>|<span data-ttu-id="4d7c3-240">Especifica o horário de início diário da hora de manutenção.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-240">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="4d7c3-241">fastFirstSignIn</span><span class="sxs-lookup"><span data-stu-id="4d7c3-241">fastFirstSignIn</span></span>|[<span data-ttu-id="4d7c3-242">habilitação</span><span class="sxs-lookup"><span data-stu-id="4d7c3-242">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4d7c3-243">Especifica se a conexão automática de novas contas não administrativas do Azure AD para contas locais de candidatos pré-configuradas.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-243">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="4d7c3-244">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-244">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="4d7c3-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d7c3-245">Response</span></span>
<span data-ttu-id="4d7c3-246">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-246">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d7c3-247">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d7c3-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d7c3-248">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d7c3-248">Request</span></span>
<span data-ttu-id="4d7c3-249">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-249">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4d7c3-250">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d7c3-250">Response</span></span>
<span data-ttu-id="4d7c3-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d7c3-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





