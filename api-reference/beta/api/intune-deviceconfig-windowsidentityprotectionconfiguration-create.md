---
title: Criar windowsIdentityProtectionConfiguration
description: Crie um novo objeto de windowsIdentityProtectionConfiguration.
ms.openlocfilehash: 30700a08517e5762068078de46369e892218c8f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037187"
---
# <a name="create-windowsidentityprotectionconfiguration"></a><span data-ttu-id="82c41-103">Criar windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="82c41-103">Create windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="82c41-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="82c41-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82c41-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="82c41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82c41-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="82c41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82c41-107">Crie um novo objeto de [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="82c41-107">Create a new [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="82c41-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="82c41-108">Prerequisites</span></span>
<span data-ttu-id="82c41-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82c41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82c41-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82c41-111">Permission type</span></span>|<span data-ttu-id="82c41-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="82c41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82c41-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82c41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82c41-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82c41-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82c41-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82c41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82c41-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82c41-116">Not supported.</span></span>|
|<span data-ttu-id="82c41-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82c41-117">Application</span></span>|<span data-ttu-id="82c41-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82c41-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82c41-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82c41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="82c41-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82c41-120">Request headers</span></span>
|<span data-ttu-id="82c41-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="82c41-121">Header</span></span>|<span data-ttu-id="82c41-122">Valor</span><span class="sxs-lookup"><span data-stu-id="82c41-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82c41-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="82c41-123">Authorization</span></span>|<span data-ttu-id="82c41-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82c41-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82c41-125">Accept</span><span class="sxs-lookup"><span data-stu-id="82c41-125">Accept</span></span>|<span data-ttu-id="82c41-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82c41-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82c41-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82c41-127">Request body</span></span>
<span data-ttu-id="82c41-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsIdentityProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="82c41-128">In the request body, supply a JSON representation for the windowsIdentityProtectionConfiguration object.</span></span>

<span data-ttu-id="82c41-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsIdentityProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="82c41-129">The following table shows the properties that are required when you create the windowsIdentityProtectionConfiguration.</span></span>

|<span data-ttu-id="82c41-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82c41-130">Property</span></span>|<span data-ttu-id="82c41-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="82c41-131">Type</span></span>|<span data-ttu-id="82c41-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="82c41-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82c41-133">id</span><span class="sxs-lookup"><span data-stu-id="82c41-133">id</span></span>|<span data-ttu-id="82c41-134">String</span><span class="sxs-lookup"><span data-stu-id="82c41-134">String</span></span>|<span data-ttu-id="82c41-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="82c41-135">Key of the entity.</span></span> <span data-ttu-id="82c41-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82c41-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82c41-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82c41-137">lastModifiedDateTime</span></span>|<span data-ttu-id="82c41-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82c41-138">DateTimeOffset</span></span>|<span data-ttu-id="82c41-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="82c41-139">DateTime the object was last modified.</span></span> <span data-ttu-id="82c41-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82c41-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82c41-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="82c41-141">roleScopeTagIds</span></span>|<span data-ttu-id="82c41-142">String collection</span><span class="sxs-lookup"><span data-stu-id="82c41-142">String collection</span></span>|<span data-ttu-id="82c41-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="82c41-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="82c41-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82c41-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82c41-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="82c41-145">supportsScopeTags</span></span>|<span data-ttu-id="82c41-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c41-146">Boolean</span></span>|<span data-ttu-id="82c41-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="82c41-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="82c41-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="82c41-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="82c41-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="82c41-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="82c41-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="82c41-150">This property is read-only.</span></span> <span data-ttu-id="82c41-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82c41-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82c41-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82c41-152">createdDateTime</span></span>|<span data-ttu-id="82c41-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82c41-153">DateTimeOffset</span></span>|<span data-ttu-id="82c41-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="82c41-154">DateTime the object was created.</span></span> <span data-ttu-id="82c41-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82c41-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82c41-156">description</span><span class="sxs-lookup"><span data-stu-id="82c41-156">description</span></span>|<span data-ttu-id="82c41-157">String</span><span class="sxs-lookup"><span data-stu-id="82c41-157">String</span></span>|<span data-ttu-id="82c41-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="82c41-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="82c41-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82c41-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82c41-160">displayName</span><span class="sxs-lookup"><span data-stu-id="82c41-160">displayName</span></span>|<span data-ttu-id="82c41-161">String</span><span class="sxs-lookup"><span data-stu-id="82c41-161">String</span></span>|<span data-ttu-id="82c41-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="82c41-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="82c41-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82c41-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82c41-164">version</span><span class="sxs-lookup"><span data-stu-id="82c41-164">version</span></span>|<span data-ttu-id="82c41-165">Int32</span><span class="sxs-lookup"><span data-stu-id="82c41-165">Int32</span></span>|<span data-ttu-id="82c41-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="82c41-166">Version of the device configuration.</span></span> <span data-ttu-id="82c41-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82c41-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82c41-168">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="82c41-168">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="82c41-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c41-169">Boolean</span></span>|<span data-ttu-id="82c41-170">Valor booleano usado para habilitar avançada antifalsificação para reconhecimento de recurso faciais na autenticação do Windows Olá face padrão.</span><span class="sxs-lookup"><span data-stu-id="82c41-170">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="82c41-171">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="82c41-171">pinMinimumLength</span></span>|<span data-ttu-id="82c41-172">Int32</span><span class="sxs-lookup"><span data-stu-id="82c41-172">Int32</span></span>|<span data-ttu-id="82c41-173">Valor inteiro que define o número mínimo de caracteres necessários para o Windows Olá PIN de negócios.</span><span class="sxs-lookup"><span data-stu-id="82c41-173">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="82c41-174">Os valores válidos são de 4 a 127 inclusive e menor ou igual ao valor definido para o PIN máximo.</span><span class="sxs-lookup"><span data-stu-id="82c41-174">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="82c41-175">Valores válidos 4 a 127</span><span class="sxs-lookup"><span data-stu-id="82c41-175">Valid values 4 to 127</span></span>|
|<span data-ttu-id="82c41-176">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="82c41-176">pinMaximumLength</span></span>|<span data-ttu-id="82c41-177">Int32</span><span class="sxs-lookup"><span data-stu-id="82c41-177">Int32</span></span>|<span data-ttu-id="82c41-178">Valor inteiro que define o número máximo de caracteres permitido para o trabalho PIN.</span><span class="sxs-lookup"><span data-stu-id="82c41-178">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="82c41-179">Valores válidos são de 4 a 127 inclusive e maior ou igual ao valor definido para o PIN mínimo.</span><span class="sxs-lookup"><span data-stu-id="82c41-179">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="82c41-180">Valores válidos 4 a 127</span><span class="sxs-lookup"><span data-stu-id="82c41-180">Valid values 4 to 127</span></span>|
|<span data-ttu-id="82c41-181">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="82c41-181">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="82c41-182">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="82c41-182">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="82c41-183">Esse valor configura o uso de caracteres maiusculos no Windows Olá PIN de negócios.</span><span class="sxs-lookup"><span data-stu-id="82c41-183">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="82c41-184">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="82c41-184">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="82c41-185">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="82c41-185">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="82c41-186">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="82c41-186">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="82c41-187">Esse valor configura o uso de caracteres minúsculos no Windows Olá PIN de negócios.</span><span class="sxs-lookup"><span data-stu-id="82c41-187">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="82c41-188">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="82c41-188">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="82c41-189">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="82c41-189">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="82c41-190">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="82c41-190">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="82c41-191">Controla a capacidade de usar caracteres especiais no Windows Olá PIN de negócios.</span><span class="sxs-lookup"><span data-stu-id="82c41-191">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="82c41-192">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="82c41-192">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="82c41-193">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="82c41-193">pinExpirationInDays</span></span>|<span data-ttu-id="82c41-194">Int32</span><span class="sxs-lookup"><span data-stu-id="82c41-194">Int32</span></span>|<span data-ttu-id="82c41-195">Valor inteiro Especifica o período (em dias) que um PIN pode ser usado antes que o sistema exige que o usuário alterá-la.</span><span class="sxs-lookup"><span data-stu-id="82c41-195">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="82c41-196">Valores válidos são 0 para 730 inclusive.</span><span class="sxs-lookup"><span data-stu-id="82c41-196">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="82c41-197">Valores válidos de 0 a 730</span><span class="sxs-lookup"><span data-stu-id="82c41-197">Valid values 0 to 730</span></span>|
|<span data-ttu-id="82c41-198">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="82c41-198">pinPreviousBlockCount</span></span>|<span data-ttu-id="82c41-199">Int32</span><span class="sxs-lookup"><span data-stu-id="82c41-199">Int32</span></span>|<span data-ttu-id="82c41-200">Controla a capacidade de impedir que os usuários utilizem antigas PINs.</span><span class="sxs-lookup"><span data-stu-id="82c41-200">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="82c41-201">Isso deve ser definido entre 0 e 50, inclusive, e o PIN atual do usuário está incluído nessa contagem.</span><span class="sxs-lookup"><span data-stu-id="82c41-201">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="82c41-202">Se definido como 0, anterior PINs não são armazenadas.</span><span class="sxs-lookup"><span data-stu-id="82c41-202">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="82c41-203">Histórico PIN não é preservado por meio de um PIN redefinir.</span><span class="sxs-lookup"><span data-stu-id="82c41-203">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="82c41-204">Valores válidos de 0 a 50</span><span class="sxs-lookup"><span data-stu-id="82c41-204">Valid values 0 to 50</span></span>|
|<span data-ttu-id="82c41-205">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="82c41-205">pinRecoveryEnabled</span></span>|<span data-ttu-id="82c41-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c41-206">Boolean</span></span>|<span data-ttu-id="82c41-207">Valor booleano que permite que um usuário alterar seus PINs usando o Windows Hello para o serviço de recuperação de PIN de negócios.</span><span class="sxs-lookup"><span data-stu-id="82c41-207">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="82c41-208">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="82c41-208">securityDeviceRequired</span></span>|<span data-ttu-id="82c41-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c41-209">Boolean</span></span>|<span data-ttu-id="82c41-210">Controla se será exigido um Trusted Platform Module (TPM) para provisionamento Windows Olá for Business.</span><span class="sxs-lookup"><span data-stu-id="82c41-210">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="82c41-211">Um TPM fornece um benefício de segurança adicionais em que os dados armazenados nela não podem ser usados em outros dispositivos.</span><span class="sxs-lookup"><span data-stu-id="82c41-211">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="82c41-212">Se definido como False, todos os dispositivos podem provisionar Windows Olá for Business, mesmo se não houver um TPM utilizável.</span><span class="sxs-lookup"><span data-stu-id="82c41-212">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="82c41-213">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="82c41-213">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="82c41-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c41-214">Boolean</span></span>|<span data-ttu-id="82c41-215">Controla o uso de gestos biométricos, como nominal e a impressão digital, como uma alternativa para o Windows Olá PIN de negócios.</span><span class="sxs-lookup"><span data-stu-id="82c41-215">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="82c41-216">Se definido como False, biométricos gestos não é permitido.</span><span class="sxs-lookup"><span data-stu-id="82c41-216">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="82c41-217">Os usuários ainda devem configurar um PIN como um backup em caso de falhas.</span><span class="sxs-lookup"><span data-stu-id="82c41-217">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="82c41-218">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="82c41-218">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="82c41-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c41-219">Boolean</span></span>|<span data-ttu-id="82c41-220">Valor Boolean que permite Windows Olá for Business usar certificados para autenticar os recursos no local.</span><span class="sxs-lookup"><span data-stu-id="82c41-220">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="82c41-221">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="82c41-221">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="82c41-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c41-222">Boolean</span></span>|<span data-ttu-id="82c41-223">Valor Boolean que bloqueia Windows Olá para negócios como um método para fazer o login no Windows.</span><span class="sxs-lookup"><span data-stu-id="82c41-223">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="82c41-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="82c41-224">Response</span></span>
<span data-ttu-id="82c41-225">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82c41-225">If successful, this method returns a `201 Created` response code and a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82c41-226">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82c41-226">Example</span></span>
### <a name="request"></a><span data-ttu-id="82c41-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82c41-227">Request</span></span>
<span data-ttu-id="82c41-228">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82c41-228">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 838

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
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

### <a name="response"></a><span data-ttu-id="82c41-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="82c41-229">Response</span></span>
<span data-ttu-id="82c41-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82c41-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 946

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





