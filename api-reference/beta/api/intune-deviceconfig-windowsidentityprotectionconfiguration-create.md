---
title: Criar windowsIdentityProtectionConfiguration
description: Criar um novo objeto windowsIdentityProtectionConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 07357f72954378ac9190f0a5845e382fc7f3ccaa
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42735272"
---
# <a name="create-windowsidentityprotectionconfiguration"></a><span data-ttu-id="a5b92-103">Criar windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="a5b92-103">Create windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="a5b92-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a5b92-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5b92-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a5b92-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5b92-106">Criar um novo objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a5b92-106">Create a new [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5b92-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a5b92-107">Prerequisites</span></span>
<span data-ttu-id="a5b92-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5b92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5b92-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5b92-110">Permission type</span></span>|<span data-ttu-id="a5b92-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a5b92-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5b92-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5b92-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5b92-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5b92-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a5b92-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5b92-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5b92-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5b92-115">Not supported.</span></span>|
|<span data-ttu-id="a5b92-116">Application</span><span class="sxs-lookup"><span data-stu-id="a5b92-116">Application</span></span>|<span data-ttu-id="a5b92-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5b92-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5b92-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5b92-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a5b92-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5b92-119">Request headers</span></span>
|<span data-ttu-id="a5b92-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5b92-120">Header</span></span>|<span data-ttu-id="a5b92-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a5b92-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5b92-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5b92-122">Authorization</span></span>|<span data-ttu-id="a5b92-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5b92-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5b92-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a5b92-124">Accept</span></span>|<span data-ttu-id="a5b92-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5b92-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5b92-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5b92-126">Request body</span></span>
<span data-ttu-id="a5b92-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsIdentityProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a5b92-127">In the request body, supply a JSON representation for the windowsIdentityProtectionConfiguration object.</span></span>

<span data-ttu-id="a5b92-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsIdentityProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a5b92-128">The following table shows the properties that are required when you create the windowsIdentityProtectionConfiguration.</span></span>

|<span data-ttu-id="a5b92-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5b92-129">Property</span></span>|<span data-ttu-id="a5b92-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5b92-130">Type</span></span>|<span data-ttu-id="a5b92-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5b92-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5b92-132">id</span><span class="sxs-lookup"><span data-stu-id="a5b92-132">id</span></span>|<span data-ttu-id="a5b92-133">String</span><span class="sxs-lookup"><span data-stu-id="a5b92-133">String</span></span>|<span data-ttu-id="a5b92-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a5b92-134">Key of the entity.</span></span> <span data-ttu-id="a5b92-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5b92-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5b92-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5b92-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a5b92-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5b92-137">DateTimeOffset</span></span>|<span data-ttu-id="a5b92-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a5b92-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a5b92-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5b92-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5b92-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a5b92-140">roleScopeTagIds</span></span>|<span data-ttu-id="a5b92-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5b92-141">String collection</span></span>|<span data-ttu-id="a5b92-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a5b92-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a5b92-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5b92-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5b92-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a5b92-144">supportsScopeTags</span></span>|<span data-ttu-id="a5b92-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5b92-145">Boolean</span></span>|<span data-ttu-id="a5b92-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a5b92-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a5b92-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a5b92-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a5b92-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a5b92-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a5b92-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a5b92-149">This property is read-only.</span></span> <span data-ttu-id="a5b92-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5b92-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5b92-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a5b92-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a5b92-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a5b92-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a5b92-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="a5b92-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a5b92-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5b92-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5b92-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a5b92-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a5b92-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a5b92-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a5b92-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="a5b92-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a5b92-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5b92-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5b92-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a5b92-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a5b92-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a5b92-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a5b92-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="a5b92-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a5b92-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5b92-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5b92-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a5b92-163">createdDateTime</span></span>|<span data-ttu-id="a5b92-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5b92-164">DateTimeOffset</span></span>|<span data-ttu-id="a5b92-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a5b92-165">DateTime the object was created.</span></span> <span data-ttu-id="a5b92-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5b92-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5b92-167">description</span><span class="sxs-lookup"><span data-stu-id="a5b92-167">description</span></span>|<span data-ttu-id="a5b92-168">String</span><span class="sxs-lookup"><span data-stu-id="a5b92-168">String</span></span>|<span data-ttu-id="a5b92-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a5b92-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a5b92-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5b92-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5b92-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a5b92-171">displayName</span></span>|<span data-ttu-id="a5b92-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5b92-172">String</span></span>|<span data-ttu-id="a5b92-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a5b92-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a5b92-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5b92-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5b92-175">versão</span><span class="sxs-lookup"><span data-stu-id="a5b92-175">version</span></span>|<span data-ttu-id="a5b92-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a5b92-176">Int32</span></span>|<span data-ttu-id="a5b92-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a5b92-177">Version of the device configuration.</span></span> <span data-ttu-id="a5b92-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5b92-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5b92-179">useSecurityKeyForSignin</span><span class="sxs-lookup"><span data-stu-id="a5b92-179">useSecurityKeyForSignin</span></span>|<span data-ttu-id="a5b92-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5b92-180">Boolean</span></span>|<span data-ttu-id="a5b92-181">Valor booliano usado para habilitar a chave de segurança do Windows Hello como uma credencial de logon.</span><span class="sxs-lookup"><span data-stu-id="a5b92-181">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="a5b92-182">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="a5b92-182">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="a5b92-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5b92-183">Boolean</span></span>|<span data-ttu-id="a5b92-184">Valor booliano usado para habilitar a antifalsificação avançada para reconhecimento de recurso facial na autenticação facial do Windows Hello.</span><span class="sxs-lookup"><span data-stu-id="a5b92-184">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="a5b92-185">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a5b92-185">pinMinimumLength</span></span>|<span data-ttu-id="a5b92-186">Int32</span><span class="sxs-lookup"><span data-stu-id="a5b92-186">Int32</span></span>|<span data-ttu-id="a5b92-187">Valor inteiro que define o número mínimo de caracteres necessários para o PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="a5b92-187">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="a5b92-188">Os valores válidos são 4 a 127 inclusive e menores ou iguais ao valor definido para o PIN máximo.</span><span class="sxs-lookup"><span data-stu-id="a5b92-188">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="a5b92-189">Valores válidos de 4 a 127</span><span class="sxs-lookup"><span data-stu-id="a5b92-189">Valid values 4 to 127</span></span>|
|<span data-ttu-id="a5b92-190">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="a5b92-190">pinMaximumLength</span></span>|<span data-ttu-id="a5b92-191">Int32</span><span class="sxs-lookup"><span data-stu-id="a5b92-191">Int32</span></span>|<span data-ttu-id="a5b92-192">Valor inteiro que define o número máximo de caracteres permitidos para o PIN de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a5b92-192">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="a5b92-193">Os valores válidos são 4 a 127 inclusive e maiores ou iguais ao valor definido para o PIN mínimo.</span><span class="sxs-lookup"><span data-stu-id="a5b92-193">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="a5b92-194">Valores válidos de 4 a 127</span><span class="sxs-lookup"><span data-stu-id="a5b92-194">Valid values 4 to 127</span></span>|
|<span data-ttu-id="a5b92-195">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a5b92-195">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="a5b92-196">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="a5b92-196">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="a5b92-197">Este valor configura o uso de caracteres maiúsculos no PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="a5b92-197">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="a5b92-198">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="a5b92-198">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="a5b92-199">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a5b92-199">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="a5b92-200">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="a5b92-200">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="a5b92-201">Esse valor configura o uso de caracteres minúsculos no PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="a5b92-201">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="a5b92-202">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="a5b92-202">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="a5b92-203">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a5b92-203">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="a5b92-204">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="a5b92-204">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="a5b92-205">Controla a capacidade de usar caracteres especiais no PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="a5b92-205">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="a5b92-206">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="a5b92-206">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="a5b92-207">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="a5b92-207">pinExpirationInDays</span></span>|<span data-ttu-id="a5b92-208">Int32</span><span class="sxs-lookup"><span data-stu-id="a5b92-208">Int32</span></span>|<span data-ttu-id="a5b92-209">Valor inteiro especifica o período (em dias) que um PIN pode ser usado antes que o sistema exija que o usuário o altere.</span><span class="sxs-lookup"><span data-stu-id="a5b92-209">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="a5b92-210">Os valores válidos são de 0 a 730 inclusive.</span><span class="sxs-lookup"><span data-stu-id="a5b92-210">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="a5b92-211">Valores válidos de 0 a 730</span><span class="sxs-lookup"><span data-stu-id="a5b92-211">Valid values 0 to 730</span></span>|
|<span data-ttu-id="a5b92-212">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="a5b92-212">pinPreviousBlockCount</span></span>|<span data-ttu-id="a5b92-213">Int32</span><span class="sxs-lookup"><span data-stu-id="a5b92-213">Int32</span></span>|<span data-ttu-id="a5b92-214">Controla a capacidade de impedir que os usuários usem PINs passados.</span><span class="sxs-lookup"><span data-stu-id="a5b92-214">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="a5b92-215">Isso deve ser definido entre 0 e 50, inclusive, e o PIN atual do usuário é incluído nessa contagem.</span><span class="sxs-lookup"><span data-stu-id="a5b92-215">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="a5b92-216">Se for definido como 0, os PINs anteriores não serão armazenados.</span><span class="sxs-lookup"><span data-stu-id="a5b92-216">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="a5b92-217">O histórico de PIN não é preservado por meio de uma redefinição de PIN.</span><span class="sxs-lookup"><span data-stu-id="a5b92-217">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="a5b92-218">Valores válidos de 0 a 50</span><span class="sxs-lookup"><span data-stu-id="a5b92-218">Valid values 0 to 50</span></span>|
|<span data-ttu-id="a5b92-219">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="a5b92-219">pinRecoveryEnabled</span></span>|<span data-ttu-id="a5b92-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5b92-220">Boolean</span></span>|<span data-ttu-id="a5b92-221">Valor booliano que permite que um usuário altere o PIN usando o serviço de recuperação de PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="a5b92-221">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="a5b92-222">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="a5b92-222">securityDeviceRequired</span></span>|<span data-ttu-id="a5b92-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5b92-223">Boolean</span></span>|<span data-ttu-id="a5b92-224">Controla se é necessário exigir um TPM (Trusted Platform Module) para provisionar o Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="a5b92-224">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="a5b92-225">Um TPM oferece um benefício de segurança adicional nos dados armazenados nele que não podem ser usados em outros dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a5b92-225">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="a5b92-226">Se for definido como false, todos os dispositivos poderão provisionar o Windows Hello para empresas mesmo se não houver um TPM utilizável.</span><span class="sxs-lookup"><span data-stu-id="a5b92-226">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="a5b92-227">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="a5b92-227">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="a5b92-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5b92-228">Boolean</span></span>|<span data-ttu-id="a5b92-229">Controla o uso de gestos biométricos, como face e impressão digital, como uma alternativa para o PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="a5b92-229">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="a5b92-230">Se for definido como false, os gestos biométricos não serão permitidos.</span><span class="sxs-lookup"><span data-stu-id="a5b92-230">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="a5b92-231">Os usuários ainda devem configurar um PIN como um backup em caso de falhas.</span><span class="sxs-lookup"><span data-stu-id="a5b92-231">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="a5b92-232">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="a5b92-232">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="a5b92-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5b92-233">Boolean</span></span>|<span data-ttu-id="a5b92-234">Valor booliano que permite ao Windows Hello para empresas usar certificados para autenticar recursos locais.</span><span class="sxs-lookup"><span data-stu-id="a5b92-234">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="a5b92-235">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="a5b92-235">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="a5b92-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5b92-236">Boolean</span></span>|<span data-ttu-id="a5b92-237">Valor booliano que bloqueia o Windows Hello para empresas como um método para entrar no Windows.</span><span class="sxs-lookup"><span data-stu-id="a5b92-237">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="a5b92-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5b92-238">Response</span></span>
<span data-ttu-id="a5b92-239">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5b92-239">If successful, this method returns a `201 Created` response code and a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5b92-240">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5b92-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5b92-241">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5b92-241">Request</span></span>
<span data-ttu-id="a5b92-242">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5b92-242">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a5b92-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5b92-243">Response</span></span>
<span data-ttu-id="a5b92-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5b92-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




