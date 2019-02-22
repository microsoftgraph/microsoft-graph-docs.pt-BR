---
title: Atualizar windowsIdentityProtectionConfiguration
description: Atualiza as propriedades de um objeto windowsIdentityProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 14b8a94c8a27ec06187b342af5619433c48ccce9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141290"
---
# <a name="update-windowsidentityprotectionconfiguration"></a><span data-ttu-id="013c5-103">Atualizar windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="013c5-103">Update windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="013c5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="013c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="013c5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="013c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="013c5-106">Atualiza as propriedades de um objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="013c5-106">Update the properties of a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="013c5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="013c5-107">Prerequisites</span></span>
<span data-ttu-id="013c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="013c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="013c5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="013c5-110">Permission type</span></span>|<span data-ttu-id="013c5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="013c5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="013c5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="013c5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="013c5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="013c5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="013c5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="013c5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="013c5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="013c5-115">Not supported.</span></span>|
|<span data-ttu-id="013c5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="013c5-116">Application</span></span>|<span data-ttu-id="013c5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="013c5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="013c5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="013c5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="013c5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="013c5-119">Request headers</span></span>
|<span data-ttu-id="013c5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="013c5-120">Header</span></span>|<span data-ttu-id="013c5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="013c5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="013c5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="013c5-122">Authorization</span></span>|<span data-ttu-id="013c5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="013c5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="013c5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="013c5-124">Accept</span></span>|<span data-ttu-id="013c5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="013c5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="013c5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="013c5-126">Request body</span></span>
<span data-ttu-id="013c5-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="013c5-127">In the request body, supply a JSON representation for the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="013c5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="013c5-128">The following table shows the properties that are required when you create the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).</span></span>

|<span data-ttu-id="013c5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="013c5-129">Property</span></span>|<span data-ttu-id="013c5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="013c5-130">Type</span></span>|<span data-ttu-id="013c5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="013c5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="013c5-132">id</span><span class="sxs-lookup"><span data-stu-id="013c5-132">id</span></span>|<span data-ttu-id="013c5-133">String</span><span class="sxs-lookup"><span data-stu-id="013c5-133">String</span></span>|<span data-ttu-id="013c5-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="013c5-134">Key of the entity.</span></span> <span data-ttu-id="013c5-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="013c5-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="013c5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="013c5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="013c5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="013c5-137">DateTimeOffset</span></span>|<span data-ttu-id="013c5-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="013c5-138">DateTime the object was last modified.</span></span> <span data-ttu-id="013c5-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="013c5-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="013c5-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="013c5-140">roleScopeTagIds</span></span>|<span data-ttu-id="013c5-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="013c5-141">String collection</span></span>|<span data-ttu-id="013c5-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="013c5-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="013c5-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="013c5-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="013c5-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="013c5-144">supportsScopeTags</span></span>|<span data-ttu-id="013c5-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="013c5-145">Boolean</span></span>|<span data-ttu-id="013c5-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="013c5-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="013c5-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="013c5-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="013c5-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="013c5-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="013c5-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="013c5-149">This property is read-only.</span></span> <span data-ttu-id="013c5-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="013c5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="013c5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="013c5-151">createdDateTime</span></span>|<span data-ttu-id="013c5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="013c5-152">DateTimeOffset</span></span>|<span data-ttu-id="013c5-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="013c5-153">DateTime the object was created.</span></span> <span data-ttu-id="013c5-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="013c5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="013c5-155">description</span><span class="sxs-lookup"><span data-stu-id="013c5-155">description</span></span>|<span data-ttu-id="013c5-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="013c5-156">String</span></span>|<span data-ttu-id="013c5-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="013c5-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="013c5-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="013c5-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="013c5-159">displayName</span><span class="sxs-lookup"><span data-stu-id="013c5-159">displayName</span></span>|<span data-ttu-id="013c5-160">String</span><span class="sxs-lookup"><span data-stu-id="013c5-160">String</span></span>|<span data-ttu-id="013c5-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="013c5-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="013c5-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="013c5-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="013c5-163">version</span><span class="sxs-lookup"><span data-stu-id="013c5-163">version</span></span>|<span data-ttu-id="013c5-164">Int32</span><span class="sxs-lookup"><span data-stu-id="013c5-164">Int32</span></span>|<span data-ttu-id="013c5-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="013c5-165">Version of the device configuration.</span></span> <span data-ttu-id="013c5-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="013c5-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="013c5-167">useSecurityKeyForSignin</span><span class="sxs-lookup"><span data-stu-id="013c5-167">useSecurityKeyForSignin</span></span>|<span data-ttu-id="013c5-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="013c5-168">Boolean</span></span>|<span data-ttu-id="013c5-169">Valor booliano usado para habilitar a chave de segurança do Windows Hello como uma credencial de logon.</span><span class="sxs-lookup"><span data-stu-id="013c5-169">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="013c5-170">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="013c5-170">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="013c5-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="013c5-171">Boolean</span></span>|<span data-ttu-id="013c5-172">Valor booliano usado para habilitar a antifalsificação avançada para reconhecimento de recurso facial na autenticação facial do Windows Hello.</span><span class="sxs-lookup"><span data-stu-id="013c5-172">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="013c5-173">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="013c5-173">pinMinimumLength</span></span>|<span data-ttu-id="013c5-174">Int32</span><span class="sxs-lookup"><span data-stu-id="013c5-174">Int32</span></span>|<span data-ttu-id="013c5-175">Valor inteiro que define o número mínimo de caracteres necessários para o PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="013c5-175">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="013c5-176">Os valores válidos são 4 a 127 inclusive e menores ou iguais ao valor definido para o PIN máximo.</span><span class="sxs-lookup"><span data-stu-id="013c5-176">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="013c5-177">Valores válidos de 4 a 127</span><span class="sxs-lookup"><span data-stu-id="013c5-177">Valid values 4 to 127</span></span>|
|<span data-ttu-id="013c5-178">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="013c5-178">pinMaximumLength</span></span>|<span data-ttu-id="013c5-179">Int32</span><span class="sxs-lookup"><span data-stu-id="013c5-179">Int32</span></span>|<span data-ttu-id="013c5-180">Valor inteiro que define o número máximo de caracteres permitidos para o PIN de trabalho.</span><span class="sxs-lookup"><span data-stu-id="013c5-180">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="013c5-181">Os valores válidos são 4 a 127 inclusive e maiores ou iguais ao valor definido para o PIN mínimo.</span><span class="sxs-lookup"><span data-stu-id="013c5-181">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="013c5-182">Valores válidos de 4 a 127</span><span class="sxs-lookup"><span data-stu-id="013c5-182">Valid values 4 to 127</span></span>|
|<span data-ttu-id="013c5-183">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="013c5-183">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="013c5-184">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="013c5-184">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="013c5-185">Este valor configura o uso de caracteres maiúsculos no PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="013c5-185">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="013c5-186">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="013c5-186">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="013c5-187">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="013c5-187">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="013c5-188">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="013c5-188">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="013c5-189">Esse valor configura o uso de caracteres minúsculos no PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="013c5-189">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="013c5-190">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="013c5-190">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="013c5-191">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="013c5-191">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="013c5-192">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="013c5-192">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="013c5-193">Controla a capacidade de usar caracteres especiais no PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="013c5-193">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="013c5-194">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="013c5-194">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="013c5-195">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="013c5-195">pinExpirationInDays</span></span>|<span data-ttu-id="013c5-196">Int32</span><span class="sxs-lookup"><span data-stu-id="013c5-196">Int32</span></span>|<span data-ttu-id="013c5-197">Valor inteiro especifica o período (em dias) que um PIN pode ser usado antes que o sistema exija que o usuário o altere.</span><span class="sxs-lookup"><span data-stu-id="013c5-197">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="013c5-198">Os valores válidos são de 0 a 730 inclusive.</span><span class="sxs-lookup"><span data-stu-id="013c5-198">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="013c5-199">Valores válidos de 0 a 730</span><span class="sxs-lookup"><span data-stu-id="013c5-199">Valid values 0 to 730</span></span>|
|<span data-ttu-id="013c5-200">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="013c5-200">pinPreviousBlockCount</span></span>|<span data-ttu-id="013c5-201">Int32</span><span class="sxs-lookup"><span data-stu-id="013c5-201">Int32</span></span>|<span data-ttu-id="013c5-202">Controla a capacidade de impedir que os usuários usem PINs passados.</span><span class="sxs-lookup"><span data-stu-id="013c5-202">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="013c5-203">Isso deve ser definido entre 0 e 50, inclusive, e o PIN atual do usuário é incluído nessa contagem.</span><span class="sxs-lookup"><span data-stu-id="013c5-203">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="013c5-204">Se for definido como 0, os PINs anteriores não serão armazenados.</span><span class="sxs-lookup"><span data-stu-id="013c5-204">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="013c5-205">O histórico de PIN não é preservado por meio de uma redefinição de PIN.</span><span class="sxs-lookup"><span data-stu-id="013c5-205">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="013c5-206">Valores válidos de 0 a 50</span><span class="sxs-lookup"><span data-stu-id="013c5-206">Valid values 0 to 50</span></span>|
|<span data-ttu-id="013c5-207">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="013c5-207">pinRecoveryEnabled</span></span>|<span data-ttu-id="013c5-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="013c5-208">Boolean</span></span>|<span data-ttu-id="013c5-209">Valor booliano que permite que um usuário altere o PIN usando o serviço de recuperação de PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="013c5-209">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="013c5-210">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="013c5-210">securityDeviceRequired</span></span>|<span data-ttu-id="013c5-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="013c5-211">Boolean</span></span>|<span data-ttu-id="013c5-212">Controla se é necessário exigir um TPM (Trusted Platform Module) para provisionar o Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="013c5-212">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="013c5-213">Um TPM oferece um benefício de segurança adicional nos dados armazenados nele que não podem ser usados em outros dispositivos.</span><span class="sxs-lookup"><span data-stu-id="013c5-213">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="013c5-214">Se for definido como false, todos os dispositivos poderão provisionar o Windows Hello para empresas mesmo se não houver um TPM utilizável.</span><span class="sxs-lookup"><span data-stu-id="013c5-214">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="013c5-215">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="013c5-215">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="013c5-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="013c5-216">Boolean</span></span>|<span data-ttu-id="013c5-217">Controla o uso de gestos biométricos, como face e impressão digital, como uma alternativa para o PIN do Windows Hello para empresas.</span><span class="sxs-lookup"><span data-stu-id="013c5-217">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="013c5-218">Se for definido como false, os gestos biométricos não serão permitidos.</span><span class="sxs-lookup"><span data-stu-id="013c5-218">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="013c5-219">Os usuários ainda devem configurar um PIN como um backup em caso de falhas.</span><span class="sxs-lookup"><span data-stu-id="013c5-219">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="013c5-220">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="013c5-220">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="013c5-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="013c5-221">Boolean</span></span>|<span data-ttu-id="013c5-222">Valor booliano que permite ao Windows Hello para empresas usar certificados para autenticar recursos locais.</span><span class="sxs-lookup"><span data-stu-id="013c5-222">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="013c5-223">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="013c5-223">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="013c5-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="013c5-224">Boolean</span></span>|<span data-ttu-id="013c5-225">Valor booliano que bloqueia o Windows Hello para empresas como um método para entrar no Windows.</span><span class="sxs-lookup"><span data-stu-id="013c5-225">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="013c5-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="013c5-226">Response</span></span>
<span data-ttu-id="013c5-227">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="013c5-227">If successful, this method returns a `200 OK` response code and an updated [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="013c5-228">Exemplo</span><span class="sxs-lookup"><span data-stu-id="013c5-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="013c5-229">Solicitação</span><span class="sxs-lookup"><span data-stu-id="013c5-229">Request</span></span>
<span data-ttu-id="013c5-230">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="013c5-230">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 810

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="013c5-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="013c5-231">Response</span></span>
<span data-ttu-id="013c5-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="013c5-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 982

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




