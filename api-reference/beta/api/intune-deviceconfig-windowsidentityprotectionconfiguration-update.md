---
title: Atualizar windowsIdentityProtectionConfiguration
description: Atualiza as propriedades de um objeto windowsIdentityProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 18b9ceb8b410baf9ea006bf76c8a86188ff96498
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42475800"
---
# <a name="update-windowsidentityprotectionconfiguration"></a><span data-ttu-id="5d500-103">Atualizar windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="5d500-103">Update windowsIdentityProtectionConfiguration</span></span>

<span data-ttu-id="5d500-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5d500-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d500-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5d500-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d500-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5d500-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d500-107">Atualiza as propriedades de um objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5d500-107">Update the properties of a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d500-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5d500-108">Prerequisites</span></span>
<span data-ttu-id="5d500-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d500-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d500-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d500-111">Permission type</span></span>|<span data-ttu-id="5d500-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5d500-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d500-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d500-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5d500-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d500-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5d500-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d500-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d500-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d500-116">Not supported.</span></span>|
|<span data-ttu-id="5d500-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d500-117">Application</span></span>|<span data-ttu-id="5d500-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d500-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d500-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d500-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5d500-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d500-120">Request headers</span></span>
|<span data-ttu-id="5d500-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5d500-121">Header</span></span>|<span data-ttu-id="5d500-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5d500-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d500-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d500-123">Authorization</span></span>|<span data-ttu-id="5d500-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d500-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d500-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5d500-125">Accept</span></span>|<span data-ttu-id="5d500-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5d500-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d500-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d500-127">Request body</span></span>
<span data-ttu-id="5d500-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5d500-128">In the request body, supply a JSON representation for the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="5d500-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5d500-129">The following table shows the properties that are required when you create the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).</span></span>

|<span data-ttu-id="5d500-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d500-130">Property</span></span>|<span data-ttu-id="5d500-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d500-131">Type</span></span>|<span data-ttu-id="5d500-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d500-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d500-133">id</span><span class="sxs-lookup"><span data-stu-id="5d500-133">id</span></span>|<span data-ttu-id="5d500-134">String</span><span class="sxs-lookup"><span data-stu-id="5d500-134">String</span></span>|<span data-ttu-id="5d500-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5d500-135">Key of the entity.</span></span> <span data-ttu-id="5d500-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d500-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d500-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5d500-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5d500-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d500-138">DateTimeOffset</span></span>|<span data-ttu-id="5d500-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5d500-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5d500-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d500-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d500-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5d500-141">roleScopeTagIds</span></span>|<span data-ttu-id="5d500-142">String collection</span><span class="sxs-lookup"><span data-stu-id="5d500-142">String collection</span></span>|<span data-ttu-id="5d500-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="5d500-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5d500-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d500-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d500-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5d500-145">supportsScopeTags</span></span>|<span data-ttu-id="5d500-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d500-146">Boolean</span></span>|<span data-ttu-id="5d500-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="5d500-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5d500-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="5d500-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5d500-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="5d500-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5d500-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5d500-150">This property is read-only.</span></span> <span data-ttu-id="5d500-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d500-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d500-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5d500-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5d500-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5d500-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5d500-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="5d500-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5d500-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d500-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d500-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5d500-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5d500-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5d500-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5d500-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="5d500-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5d500-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d500-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d500-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5d500-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5d500-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5d500-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5d500-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="5d500-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5d500-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d500-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d500-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5d500-164">createdDateTime</span></span>|<span data-ttu-id="5d500-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d500-165">DateTimeOffset</span></span>|<span data-ttu-id="5d500-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5d500-166">DateTime the object was created.</span></span> <span data-ttu-id="5d500-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d500-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d500-168">description</span><span class="sxs-lookup"><span data-stu-id="5d500-168">description</span></span>|<span data-ttu-id="5d500-169">String</span><span class="sxs-lookup"><span data-stu-id="5d500-169">String</span></span>|<span data-ttu-id="5d500-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5d500-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5d500-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d500-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d500-172">displayName</span><span class="sxs-lookup"><span data-stu-id="5d500-172">displayName</span></span>|<span data-ttu-id="5d500-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5d500-173">String</span></span>|<span data-ttu-id="5d500-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5d500-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5d500-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d500-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d500-176">versão</span><span class="sxs-lookup"><span data-stu-id="5d500-176">version</span></span>|<span data-ttu-id="5d500-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5d500-177">Int32</span></span>|<span data-ttu-id="5d500-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5d500-178">Version of the device configuration.</span></span> <span data-ttu-id="5d500-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d500-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d500-180">useSecurityKeyForSignin</span><span class="sxs-lookup"><span data-stu-id="5d500-180">useSecurityKeyForSignin</span></span>|<span data-ttu-id="5d500-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d500-181">Boolean</span></span>|<span data-ttu-id="5d500-182">Valor booliano usado para habilitar a chave de segurança do Windows Hello como uma credencial de logon.</span><span class="sxs-lookup"><span data-stu-id="5d500-182">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="5d500-183">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="5d500-183">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="5d500-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d500-184">Boolean</span></span>|<span data-ttu-id="5d500-185">Valor booliano usado para habilitar a antifalsificação avançada para reconhecimento de recurso facial na autenticação facial do Windows Hello.</span><span class="sxs-lookup"><span data-stu-id="5d500-185">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="5d500-186">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5d500-186">pinMinimumLength</span></span>|<span data-ttu-id="5d500-187">Int32</span><span class="sxs-lookup"><span data-stu-id="5d500-187">Int32</span></span>|<span data-ttu-id="5d500-188">Valor inteiro que define o número mínimo de caracteres necessários para o PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="5d500-188">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="5d500-189">Os valores válidos são 4 a 127 inclusive e menores ou iguais ao valor definido para o PIN máximo.</span><span class="sxs-lookup"><span data-stu-id="5d500-189">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="5d500-190">Valores válidos de 4 a 127</span><span class="sxs-lookup"><span data-stu-id="5d500-190">Valid values 4 to 127</span></span>|
|<span data-ttu-id="5d500-191">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="5d500-191">pinMaximumLength</span></span>|<span data-ttu-id="5d500-192">Int32</span><span class="sxs-lookup"><span data-stu-id="5d500-192">Int32</span></span>|<span data-ttu-id="5d500-193">Valor inteiro que define o número máximo de caracteres permitidos para o PIN de trabalho.</span><span class="sxs-lookup"><span data-stu-id="5d500-193">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="5d500-194">Os valores válidos são 4 a 127 inclusive e maiores ou iguais ao valor definido para o PIN mínimo.</span><span class="sxs-lookup"><span data-stu-id="5d500-194">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="5d500-195">Valores válidos de 4 a 127</span><span class="sxs-lookup"><span data-stu-id="5d500-195">Valid values 4 to 127</span></span>|
|<span data-ttu-id="5d500-196">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="5d500-196">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="5d500-197">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="5d500-197">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="5d500-198">Este valor configura o uso de caracteres maiúsculos no PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="5d500-198">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="5d500-199">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="5d500-199">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="5d500-200">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="5d500-200">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="5d500-201">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="5d500-201">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="5d500-202">Esse valor configura o uso de caracteres minúsculos no PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="5d500-202">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="5d500-203">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="5d500-203">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="5d500-204">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="5d500-204">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="5d500-205">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="5d500-205">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="5d500-206">Controla a capacidade de usar caracteres especiais no PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="5d500-206">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="5d500-207">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="5d500-207">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="5d500-208">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="5d500-208">pinExpirationInDays</span></span>|<span data-ttu-id="5d500-209">Int32</span><span class="sxs-lookup"><span data-stu-id="5d500-209">Int32</span></span>|<span data-ttu-id="5d500-210">Valor inteiro especifica o período (em dias) que um PIN pode ser usado antes que o sistema exija que o usuário o altere.</span><span class="sxs-lookup"><span data-stu-id="5d500-210">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="5d500-211">Os valores válidos são de 0 a 730 inclusive.</span><span class="sxs-lookup"><span data-stu-id="5d500-211">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="5d500-212">Valores válidos de 0 a 730</span><span class="sxs-lookup"><span data-stu-id="5d500-212">Valid values 0 to 730</span></span>|
|<span data-ttu-id="5d500-213">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="5d500-213">pinPreviousBlockCount</span></span>|<span data-ttu-id="5d500-214">Int32</span><span class="sxs-lookup"><span data-stu-id="5d500-214">Int32</span></span>|<span data-ttu-id="5d500-215">Controla a capacidade de impedir que os usuários usem PINs passados.</span><span class="sxs-lookup"><span data-stu-id="5d500-215">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="5d500-216">Isso deve ser definido entre 0 e 50, inclusive, e o PIN atual do usuário é incluído nessa contagem.</span><span class="sxs-lookup"><span data-stu-id="5d500-216">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="5d500-217">Se for definido como 0, os PINs anteriores não serão armazenados.</span><span class="sxs-lookup"><span data-stu-id="5d500-217">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="5d500-218">O histórico de PIN não é preservado por meio de uma redefinição de PIN.</span><span class="sxs-lookup"><span data-stu-id="5d500-218">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="5d500-219">Valores válidos de 0 a 50</span><span class="sxs-lookup"><span data-stu-id="5d500-219">Valid values 0 to 50</span></span>|
|<span data-ttu-id="5d500-220">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="5d500-220">pinRecoveryEnabled</span></span>|<span data-ttu-id="5d500-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d500-221">Boolean</span></span>|<span data-ttu-id="5d500-222">Valor booliano que permite que um usuário altere o PIN usando o serviço de recuperação de PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="5d500-222">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="5d500-223">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="5d500-223">securityDeviceRequired</span></span>|<span data-ttu-id="5d500-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="5d500-224">Boolean</span></span>|<span data-ttu-id="5d500-225">Controla se é necessário exigir um TPM (Trusted Platform Module) para provisionar o Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="5d500-225">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="5d500-226">Um TPM oferece um benefício de segurança adicional nos dados armazenados nele que não podem ser usados em outros dispositivos.</span><span class="sxs-lookup"><span data-stu-id="5d500-226">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="5d500-227">Se for definido como false, todos os dispositivos poderão provisionar o Windows Hello para empresas mesmo se não houver um TPM utilizável.</span><span class="sxs-lookup"><span data-stu-id="5d500-227">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="5d500-228">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="5d500-228">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="5d500-229">Booliano</span><span class="sxs-lookup"><span data-stu-id="5d500-229">Boolean</span></span>|<span data-ttu-id="5d500-230">Controla o uso de gestos biométricos, como face e impressão digital, como uma alternativa para o PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="5d500-230">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="5d500-231">Se for definido como false, os gestos biométricos não serão permitidos.</span><span class="sxs-lookup"><span data-stu-id="5d500-231">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="5d500-232">Os usuários ainda devem configurar um PIN como um backup em caso de falhas.</span><span class="sxs-lookup"><span data-stu-id="5d500-232">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="5d500-233">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="5d500-233">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="5d500-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d500-234">Boolean</span></span>|<span data-ttu-id="5d500-235">Valor booliano que permite ao Windows Hello para empresas usar certificados para autenticar recursos locais.</span><span class="sxs-lookup"><span data-stu-id="5d500-235">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="5d500-236">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="5d500-236">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="5d500-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d500-237">Boolean</span></span>|<span data-ttu-id="5d500-238">Valor booliano que bloqueia o Windows Hello para empresas como um método para entrar no Windows.</span><span class="sxs-lookup"><span data-stu-id="5d500-238">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="5d500-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d500-239">Response</span></span>
<span data-ttu-id="5d500-240">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d500-240">If successful, this method returns a `200 OK` response code and an updated [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d500-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d500-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d500-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d500-242">Request</span></span>
<span data-ttu-id="5d500-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d500-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1583

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
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
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="5d500-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d500-244">Response</span></span>
<span data-ttu-id="5d500-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d500-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1755

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
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
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```





