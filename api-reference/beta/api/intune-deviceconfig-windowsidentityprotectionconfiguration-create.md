---
title: Criar windowsIdentityProtectionConfiguration
description: Criar um novo objeto windowsIdentityProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b42301b2ce46ac3d07f028997bc74ebd2abf8e26
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49204156"
---
# <a name="create-windowsidentityprotectionconfiguration"></a><span data-ttu-id="da0d8-103">Criar windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="da0d8-103">Create windowsIdentityProtectionConfiguration</span></span>

<span data-ttu-id="da0d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da0d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da0d8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="da0d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da0d8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="da0d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da0d8-107">Criar um novo objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="da0d8-107">Create a new [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da0d8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="da0d8-108">Prerequisites</span></span>
<span data-ttu-id="da0d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da0d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da0d8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da0d8-111">Permission type</span></span>|<span data-ttu-id="da0d8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="da0d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da0d8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da0d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da0d8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da0d8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da0d8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da0d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da0d8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da0d8-116">Not supported.</span></span>|
|<span data-ttu-id="da0d8-117">Application</span><span class="sxs-lookup"><span data-stu-id="da0d8-117">Application</span></span>|<span data-ttu-id="da0d8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da0d8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da0d8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da0d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="da0d8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da0d8-120">Request headers</span></span>
|<span data-ttu-id="da0d8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da0d8-121">Header</span></span>|<span data-ttu-id="da0d8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="da0d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da0d8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="da0d8-123">Authorization</span></span>|<span data-ttu-id="da0d8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da0d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da0d8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="da0d8-125">Accept</span></span>|<span data-ttu-id="da0d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da0d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da0d8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da0d8-127">Request body</span></span>
<span data-ttu-id="da0d8-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsIdentityProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="da0d8-128">In the request body, supply a JSON representation for the windowsIdentityProtectionConfiguration object.</span></span>

<span data-ttu-id="da0d8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsIdentityProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="da0d8-129">The following table shows the properties that are required when you create the windowsIdentityProtectionConfiguration.</span></span>

|<span data-ttu-id="da0d8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da0d8-130">Property</span></span>|<span data-ttu-id="da0d8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="da0d8-131">Type</span></span>|<span data-ttu-id="da0d8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="da0d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da0d8-133">id</span><span class="sxs-lookup"><span data-stu-id="da0d8-133">id</span></span>|<span data-ttu-id="da0d8-134">String</span><span class="sxs-lookup"><span data-stu-id="da0d8-134">String</span></span>|<span data-ttu-id="da0d8-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="da0d8-135">Key of the entity.</span></span> <span data-ttu-id="da0d8-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da0d8-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da0d8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da0d8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="da0d8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da0d8-138">DateTimeOffset</span></span>|<span data-ttu-id="da0d8-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="da0d8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="da0d8-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da0d8-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da0d8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="da0d8-141">roleScopeTagIds</span></span>|<span data-ttu-id="da0d8-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="da0d8-142">String collection</span></span>|<span data-ttu-id="da0d8-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="da0d8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="da0d8-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da0d8-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da0d8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="da0d8-145">supportsScopeTags</span></span>|<span data-ttu-id="da0d8-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="da0d8-146">Boolean</span></span>|<span data-ttu-id="da0d8-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="da0d8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="da0d8-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="da0d8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="da0d8-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="da0d8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="da0d8-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="da0d8-150">This property is read-only.</span></span> <span data-ttu-id="da0d8-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da0d8-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da0d8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="da0d8-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="da0d8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="da0d8-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="da0d8-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="da0d8-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="da0d8-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da0d8-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da0d8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="da0d8-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="da0d8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="da0d8-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="da0d8-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="da0d8-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="da0d8-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da0d8-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da0d8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="da0d8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="da0d8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="da0d8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="da0d8-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="da0d8-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="da0d8-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da0d8-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da0d8-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da0d8-164">createdDateTime</span></span>|<span data-ttu-id="da0d8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da0d8-165">DateTimeOffset</span></span>|<span data-ttu-id="da0d8-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="da0d8-166">DateTime the object was created.</span></span> <span data-ttu-id="da0d8-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da0d8-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da0d8-168">description</span><span class="sxs-lookup"><span data-stu-id="da0d8-168">description</span></span>|<span data-ttu-id="da0d8-169">String</span><span class="sxs-lookup"><span data-stu-id="da0d8-169">String</span></span>|<span data-ttu-id="da0d8-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="da0d8-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="da0d8-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da0d8-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da0d8-172">displayName</span><span class="sxs-lookup"><span data-stu-id="da0d8-172">displayName</span></span>|<span data-ttu-id="da0d8-173">String</span><span class="sxs-lookup"><span data-stu-id="da0d8-173">String</span></span>|<span data-ttu-id="da0d8-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="da0d8-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="da0d8-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da0d8-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da0d8-176">versão</span><span class="sxs-lookup"><span data-stu-id="da0d8-176">version</span></span>|<span data-ttu-id="da0d8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="da0d8-177">Int32</span></span>|<span data-ttu-id="da0d8-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="da0d8-178">Version of the device configuration.</span></span> <span data-ttu-id="da0d8-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da0d8-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da0d8-180">useSecurityKeyForSignin</span><span class="sxs-lookup"><span data-stu-id="da0d8-180">useSecurityKeyForSignin</span></span>|<span data-ttu-id="da0d8-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="da0d8-181">Boolean</span></span>|<span data-ttu-id="da0d8-182">Valor booliano usado para habilitar a chave de segurança do Windows Hello como uma credencial de logon.</span><span class="sxs-lookup"><span data-stu-id="da0d8-182">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="da0d8-183">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="da0d8-183">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="da0d8-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="da0d8-184">Boolean</span></span>|<span data-ttu-id="da0d8-185">Valor booliano usado para habilitar a antifalsificação avançada para reconhecimento de recurso facial na autenticação facial do Windows Hello.</span><span class="sxs-lookup"><span data-stu-id="da0d8-185">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="da0d8-186">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="da0d8-186">pinMinimumLength</span></span>|<span data-ttu-id="da0d8-187">Int32</span><span class="sxs-lookup"><span data-stu-id="da0d8-187">Int32</span></span>|<span data-ttu-id="da0d8-188">Valor inteiro que define o número mínimo de caracteres necessários para o PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="da0d8-188">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="da0d8-189">Os valores válidos são 4 a 127 inclusive e menores ou iguais ao valor definido para o PIN máximo.</span><span class="sxs-lookup"><span data-stu-id="da0d8-189">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="da0d8-190">Valores válidos de 4 a 127</span><span class="sxs-lookup"><span data-stu-id="da0d8-190">Valid values 4 to 127</span></span>|
|<span data-ttu-id="da0d8-191">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="da0d8-191">pinMaximumLength</span></span>|<span data-ttu-id="da0d8-192">Int32</span><span class="sxs-lookup"><span data-stu-id="da0d8-192">Int32</span></span>|<span data-ttu-id="da0d8-193">Valor inteiro que define o número máximo de caracteres permitidos para o PIN de trabalho.</span><span class="sxs-lookup"><span data-stu-id="da0d8-193">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="da0d8-194">Os valores válidos são 4 a 127 inclusive e maiores ou iguais ao valor definido para o PIN mínimo.</span><span class="sxs-lookup"><span data-stu-id="da0d8-194">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="da0d8-195">Valores válidos de 4 a 127</span><span class="sxs-lookup"><span data-stu-id="da0d8-195">Valid values 4 to 127</span></span>|
|<span data-ttu-id="da0d8-196">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="da0d8-196">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="da0d8-197">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="da0d8-197">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="da0d8-198">Este valor configura o uso de caracteres maiúsculos no PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="da0d8-198">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="da0d8-199">Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="da0d8-199">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="da0d8-200">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="da0d8-200">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="da0d8-201">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="da0d8-201">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="da0d8-202">Esse valor configura o uso de caracteres minúsculos no PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="da0d8-202">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="da0d8-203">Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="da0d8-203">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="da0d8-204">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="da0d8-204">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="da0d8-205">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="da0d8-205">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="da0d8-206">Controla a capacidade de usar caracteres especiais no PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="da0d8-206">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="da0d8-207">Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="da0d8-207">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="da0d8-208">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="da0d8-208">pinExpirationInDays</span></span>|<span data-ttu-id="da0d8-209">Int32</span><span class="sxs-lookup"><span data-stu-id="da0d8-209">Int32</span></span>|<span data-ttu-id="da0d8-210">Valor inteiro especifica o período (em dias) que um PIN pode ser usado antes que o sistema exija que o usuário o altere.</span><span class="sxs-lookup"><span data-stu-id="da0d8-210">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="da0d8-211">Os valores válidos são de 0 a 730 inclusive.</span><span class="sxs-lookup"><span data-stu-id="da0d8-211">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="da0d8-212">Valores válidos de 0 a 730</span><span class="sxs-lookup"><span data-stu-id="da0d8-212">Valid values 0 to 730</span></span>|
|<span data-ttu-id="da0d8-213">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="da0d8-213">pinPreviousBlockCount</span></span>|<span data-ttu-id="da0d8-214">Int32</span><span class="sxs-lookup"><span data-stu-id="da0d8-214">Int32</span></span>|<span data-ttu-id="da0d8-215">Controla a capacidade de impedir que os usuários usem PINs passados.</span><span class="sxs-lookup"><span data-stu-id="da0d8-215">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="da0d8-216">Isso deve ser definido entre 0 e 50, inclusive, e o PIN atual do usuário é incluído nessa contagem.</span><span class="sxs-lookup"><span data-stu-id="da0d8-216">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="da0d8-217">Se for definido como 0, os PINs anteriores não serão armazenados.</span><span class="sxs-lookup"><span data-stu-id="da0d8-217">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="da0d8-218">O histórico de PIN não é preservado por meio de uma redefinição de PIN.</span><span class="sxs-lookup"><span data-stu-id="da0d8-218">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="da0d8-219">Valores válidos de 0 a 50</span><span class="sxs-lookup"><span data-stu-id="da0d8-219">Valid values 0 to 50</span></span>|
|<span data-ttu-id="da0d8-220">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="da0d8-220">pinRecoveryEnabled</span></span>|<span data-ttu-id="da0d8-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="da0d8-221">Boolean</span></span>|<span data-ttu-id="da0d8-222">Valor booliano que permite que um usuário altere o PIN usando o serviço de recuperação de PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="da0d8-222">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="da0d8-223">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="da0d8-223">securityDeviceRequired</span></span>|<span data-ttu-id="da0d8-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="da0d8-224">Boolean</span></span>|<span data-ttu-id="da0d8-225">Controla se é necessário exigir um TPM (Trusted Platform Module) para provisionar o Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="da0d8-225">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="da0d8-226">Um TPM oferece um benefício de segurança adicional nos dados armazenados nele que não podem ser usados em outros dispositivos.</span><span class="sxs-lookup"><span data-stu-id="da0d8-226">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="da0d8-227">Se for definido como false, todos os dispositivos poderão provisionar o Windows Hello para empresas mesmo se não houver um TPM utilizável.</span><span class="sxs-lookup"><span data-stu-id="da0d8-227">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="da0d8-228">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="da0d8-228">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="da0d8-229">Booliano</span><span class="sxs-lookup"><span data-stu-id="da0d8-229">Boolean</span></span>|<span data-ttu-id="da0d8-230">Controla o uso de gestos biométricos, como face e impressão digital, como uma alternativa para o PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="da0d8-230">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="da0d8-231">Se for definido como false, os gestos biométricos não serão permitidos.</span><span class="sxs-lookup"><span data-stu-id="da0d8-231">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="da0d8-232">Os usuários ainda devem configurar um PIN como um backup em caso de falhas.</span><span class="sxs-lookup"><span data-stu-id="da0d8-232">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="da0d8-233">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="da0d8-233">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="da0d8-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="da0d8-234">Boolean</span></span>|<span data-ttu-id="da0d8-235">Valor booliano que permite ao Windows Hello para empresas usar certificados para autenticar recursos locais.</span><span class="sxs-lookup"><span data-stu-id="da0d8-235">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="da0d8-236">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="da0d8-236">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="da0d8-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="da0d8-237">Boolean</span></span>|<span data-ttu-id="da0d8-238">Valor booliano que bloqueia o Windows Hello para empresas como um método para entrar no Windows.</span><span class="sxs-lookup"><span data-stu-id="da0d8-238">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="da0d8-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="da0d8-239">Response</span></span>
<span data-ttu-id="da0d8-240">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da0d8-240">If successful, this method returns a `201 Created` response code and a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da0d8-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da0d8-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="da0d8-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da0d8-242">Request</span></span>
<span data-ttu-id="da0d8-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da0d8-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="da0d8-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="da0d8-244">Response</span></span>
<span data-ttu-id="da0d8-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da0d8-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




