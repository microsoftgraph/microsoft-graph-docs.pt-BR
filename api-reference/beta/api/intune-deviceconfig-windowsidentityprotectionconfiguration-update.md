---
title: Atualizar windowsIdentityProtectionConfiguration
description: Atualiza as propriedades de um objeto windowsIdentityProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75a79520f045fcd78ffb86e5ce5c152a3e3c7f60
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946753"
---
# <a name="update-windowsidentityprotectionconfiguration"></a><span data-ttu-id="145ee-103">Atualizar windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="145ee-103">Update windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="145ee-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="145ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="145ee-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="145ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="145ee-106">Atualiza as propriedades de um objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="145ee-106">Update the properties of a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="145ee-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="145ee-107">Prerequisites</span></span>
<span data-ttu-id="145ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="145ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="145ee-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="145ee-110">Permission type</span></span>|<span data-ttu-id="145ee-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="145ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="145ee-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="145ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="145ee-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="145ee-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="145ee-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="145ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="145ee-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="145ee-115">Not supported.</span></span>|
|<span data-ttu-id="145ee-116">Application</span><span class="sxs-lookup"><span data-stu-id="145ee-116">Application</span></span>|<span data-ttu-id="145ee-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="145ee-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="145ee-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="145ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="145ee-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="145ee-119">Request headers</span></span>
|<span data-ttu-id="145ee-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="145ee-120">Header</span></span>|<span data-ttu-id="145ee-121">Valor</span><span class="sxs-lookup"><span data-stu-id="145ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="145ee-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="145ee-122">Authorization</span></span>|<span data-ttu-id="145ee-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="145ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="145ee-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="145ee-124">Accept</span></span>|<span data-ttu-id="145ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="145ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="145ee-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="145ee-126">Request body</span></span>
<span data-ttu-id="145ee-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="145ee-127">In the request body, supply a JSON representation for the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="145ee-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="145ee-128">The following table shows the properties that are required when you create the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).</span></span>

|<span data-ttu-id="145ee-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="145ee-129">Property</span></span>|<span data-ttu-id="145ee-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="145ee-130">Type</span></span>|<span data-ttu-id="145ee-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="145ee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="145ee-132">id</span><span class="sxs-lookup"><span data-stu-id="145ee-132">id</span></span>|<span data-ttu-id="145ee-133">String</span><span class="sxs-lookup"><span data-stu-id="145ee-133">String</span></span>|<span data-ttu-id="145ee-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="145ee-134">Key of the entity.</span></span> <span data-ttu-id="145ee-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="145ee-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="145ee-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="145ee-136">lastModifiedDateTime</span></span>|<span data-ttu-id="145ee-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="145ee-137">DateTimeOffset</span></span>|<span data-ttu-id="145ee-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="145ee-138">DateTime the object was last modified.</span></span> <span data-ttu-id="145ee-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="145ee-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="145ee-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="145ee-140">roleScopeTagIds</span></span>|<span data-ttu-id="145ee-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="145ee-141">String collection</span></span>|<span data-ttu-id="145ee-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="145ee-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="145ee-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="145ee-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="145ee-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="145ee-144">supportsScopeTags</span></span>|<span data-ttu-id="145ee-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="145ee-145">Boolean</span></span>|<span data-ttu-id="145ee-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="145ee-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="145ee-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="145ee-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="145ee-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="145ee-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="145ee-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="145ee-149">This property is read-only.</span></span> <span data-ttu-id="145ee-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="145ee-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="145ee-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="145ee-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="145ee-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="145ee-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="145ee-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="145ee-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="145ee-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="145ee-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="145ee-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="145ee-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="145ee-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="145ee-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="145ee-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="145ee-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="145ee-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="145ee-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="145ee-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="145ee-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="145ee-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="145ee-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="145ee-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="145ee-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="145ee-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="145ee-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="145ee-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="145ee-163">createdDateTime</span></span>|<span data-ttu-id="145ee-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="145ee-164">DateTimeOffset</span></span>|<span data-ttu-id="145ee-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="145ee-165">DateTime the object was created.</span></span> <span data-ttu-id="145ee-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="145ee-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="145ee-167">description</span><span class="sxs-lookup"><span data-stu-id="145ee-167">description</span></span>|<span data-ttu-id="145ee-168">String</span><span class="sxs-lookup"><span data-stu-id="145ee-168">String</span></span>|<span data-ttu-id="145ee-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="145ee-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="145ee-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="145ee-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="145ee-171">displayName</span><span class="sxs-lookup"><span data-stu-id="145ee-171">displayName</span></span>|<span data-ttu-id="145ee-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="145ee-172">String</span></span>|<span data-ttu-id="145ee-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="145ee-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="145ee-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="145ee-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="145ee-175">versão</span><span class="sxs-lookup"><span data-stu-id="145ee-175">version</span></span>|<span data-ttu-id="145ee-176">Int32</span><span class="sxs-lookup"><span data-stu-id="145ee-176">Int32</span></span>|<span data-ttu-id="145ee-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="145ee-177">Version of the device configuration.</span></span> <span data-ttu-id="145ee-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="145ee-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="145ee-179">useSecurityKeyForSignin</span><span class="sxs-lookup"><span data-stu-id="145ee-179">useSecurityKeyForSignin</span></span>|<span data-ttu-id="145ee-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="145ee-180">Boolean</span></span>|<span data-ttu-id="145ee-181">Valor booliano usado para habilitar a chave de segurança do Windows Hello como uma credencial de logon.</span><span class="sxs-lookup"><span data-stu-id="145ee-181">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="145ee-182">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="145ee-182">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="145ee-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="145ee-183">Boolean</span></span>|<span data-ttu-id="145ee-184">Valor booliano usado para habilitar a antifalsificação avançada para reconhecimento de recurso facial na autenticação facial do Windows Hello.</span><span class="sxs-lookup"><span data-stu-id="145ee-184">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="145ee-185">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="145ee-185">pinMinimumLength</span></span>|<span data-ttu-id="145ee-186">Int32</span><span class="sxs-lookup"><span data-stu-id="145ee-186">Int32</span></span>|<span data-ttu-id="145ee-187">Valor inteiro que define o número mínimo de caracteres necessários para o PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="145ee-187">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="145ee-188">Os valores válidos são 4 a 127 inclusive e menores ou iguais ao valor definido para o PIN máximo.</span><span class="sxs-lookup"><span data-stu-id="145ee-188">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="145ee-189">Valores válidos de 4 a 127</span><span class="sxs-lookup"><span data-stu-id="145ee-189">Valid values 4 to 127</span></span>|
|<span data-ttu-id="145ee-190">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="145ee-190">pinMaximumLength</span></span>|<span data-ttu-id="145ee-191">Int32</span><span class="sxs-lookup"><span data-stu-id="145ee-191">Int32</span></span>|<span data-ttu-id="145ee-192">Valor inteiro que define o número máximo de caracteres permitidos para o PIN de trabalho.</span><span class="sxs-lookup"><span data-stu-id="145ee-192">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="145ee-193">Os valores válidos são 4 a 127 inclusive e maiores ou iguais ao valor definido para o PIN mínimo.</span><span class="sxs-lookup"><span data-stu-id="145ee-193">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="145ee-194">Valores válidos de 4 a 127</span><span class="sxs-lookup"><span data-stu-id="145ee-194">Valid values 4 to 127</span></span>|
|<span data-ttu-id="145ee-195">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="145ee-195">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="145ee-196">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="145ee-196">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="145ee-197">Este valor configura o uso de caracteres maiúsculos no PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="145ee-197">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="145ee-198">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="145ee-198">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="145ee-199">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="145ee-199">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="145ee-200">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="145ee-200">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="145ee-201">Esse valor configura o uso de caracteres minúsculos no PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="145ee-201">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="145ee-202">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="145ee-202">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="145ee-203">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="145ee-203">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="145ee-204">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="145ee-204">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="145ee-205">Controla a capacidade de usar caracteres especiais no PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="145ee-205">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="145ee-206">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="145ee-206">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="145ee-207">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="145ee-207">pinExpirationInDays</span></span>|<span data-ttu-id="145ee-208">Int32</span><span class="sxs-lookup"><span data-stu-id="145ee-208">Int32</span></span>|<span data-ttu-id="145ee-209">Valor inteiro especifica o período (em dias) que um PIN pode ser usado antes que o sistema exija que o usuário o altere.</span><span class="sxs-lookup"><span data-stu-id="145ee-209">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="145ee-210">Os valores válidos são de 0 a 730 inclusive.</span><span class="sxs-lookup"><span data-stu-id="145ee-210">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="145ee-211">Valores válidos de 0 a 730</span><span class="sxs-lookup"><span data-stu-id="145ee-211">Valid values 0 to 730</span></span>|
|<span data-ttu-id="145ee-212">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="145ee-212">pinPreviousBlockCount</span></span>|<span data-ttu-id="145ee-213">Int32</span><span class="sxs-lookup"><span data-stu-id="145ee-213">Int32</span></span>|<span data-ttu-id="145ee-214">Controla a capacidade de impedir que os usuários usem PINs passados.</span><span class="sxs-lookup"><span data-stu-id="145ee-214">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="145ee-215">Isso deve ser definido entre 0 e 50, inclusive, e o PIN atual do usuário é incluído nessa contagem.</span><span class="sxs-lookup"><span data-stu-id="145ee-215">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="145ee-216">Se for definido como 0, os PINs anteriores não serão armazenados.</span><span class="sxs-lookup"><span data-stu-id="145ee-216">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="145ee-217">O histórico de PIN não é preservado por meio de uma redefinição de PIN.</span><span class="sxs-lookup"><span data-stu-id="145ee-217">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="145ee-218">Valores válidos de 0 a 50</span><span class="sxs-lookup"><span data-stu-id="145ee-218">Valid values 0 to 50</span></span>|
|<span data-ttu-id="145ee-219">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="145ee-219">pinRecoveryEnabled</span></span>|<span data-ttu-id="145ee-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="145ee-220">Boolean</span></span>|<span data-ttu-id="145ee-221">Valor booliano que permite que um usuário altere o PIN usando o serviço de recuperação de PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="145ee-221">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="145ee-222">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="145ee-222">securityDeviceRequired</span></span>|<span data-ttu-id="145ee-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="145ee-223">Boolean</span></span>|<span data-ttu-id="145ee-224">Controla se é necessário exigir um TPM (Trusted Platform Module) para provisionar o Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="145ee-224">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="145ee-225">Um TPM oferece um benefício de segurança adicional nos dados armazenados nele que não podem ser usados em outros dispositivos.</span><span class="sxs-lookup"><span data-stu-id="145ee-225">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="145ee-226">Se for definido como false, todos os dispositivos poderão provisionar o Windows Hello para empresas mesmo se não houver um TPM utilizável.</span><span class="sxs-lookup"><span data-stu-id="145ee-226">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="145ee-227">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="145ee-227">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="145ee-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="145ee-228">Boolean</span></span>|<span data-ttu-id="145ee-229">Controla o uso de gestos biométricos, como face e impressão digital, como uma alternativa para o PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="145ee-229">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="145ee-230">Se for definido como false, os gestos biométricos não serão permitidos.</span><span class="sxs-lookup"><span data-stu-id="145ee-230">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="145ee-231">Os usuários ainda devem configurar um PIN como um backup em caso de falhas.</span><span class="sxs-lookup"><span data-stu-id="145ee-231">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="145ee-232">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="145ee-232">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="145ee-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="145ee-233">Boolean</span></span>|<span data-ttu-id="145ee-234">Valor booliano que permite ao Windows Hello para empresas usar certificados para autenticar recursos locais.</span><span class="sxs-lookup"><span data-stu-id="145ee-234">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="145ee-235">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="145ee-235">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="145ee-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="145ee-236">Boolean</span></span>|<span data-ttu-id="145ee-237">Valor booliano que bloqueia o Windows Hello para empresas como um método para entrar no Windows.</span><span class="sxs-lookup"><span data-stu-id="145ee-237">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="145ee-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="145ee-238">Response</span></span>
<span data-ttu-id="145ee-239">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="145ee-239">If successful, this method returns a `200 OK` response code and an updated [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="145ee-240">Exemplo</span><span class="sxs-lookup"><span data-stu-id="145ee-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="145ee-241">Solicitação</span><span class="sxs-lookup"><span data-stu-id="145ee-241">Request</span></span>
<span data-ttu-id="145ee-242">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="145ee-242">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="145ee-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="145ee-243">Response</span></span>
<span data-ttu-id="145ee-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="145ee-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





