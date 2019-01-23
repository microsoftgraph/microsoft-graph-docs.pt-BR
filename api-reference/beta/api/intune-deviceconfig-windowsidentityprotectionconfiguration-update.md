---
title: Atualizar windowsIdentityProtectionConfiguration
description: Atualize as propriedades de um objeto windowsIdentityProtectionConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 130e4cda84be5b6e79245c2964acc5580fd5ad79
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418509"
---
# <a name="update-windowsidentityprotectionconfiguration"></a><span data-ttu-id="975d0-103">Atualizar windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="975d0-103">Update windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="975d0-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="975d0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="975d0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="975d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="975d0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="975d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="975d0-107">Atualize as propriedades de um objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="975d0-107">Update the properties of a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="975d0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="975d0-108">Prerequisites</span></span>
<span data-ttu-id="975d0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="975d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="975d0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="975d0-111">Permission type</span></span>|<span data-ttu-id="975d0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="975d0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="975d0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="975d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="975d0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="975d0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="975d0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="975d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="975d0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="975d0-116">Not supported.</span></span>|
|<span data-ttu-id="975d0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="975d0-117">Application</span></span>|<span data-ttu-id="975d0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="975d0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="975d0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="975d0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="975d0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="975d0-120">Request headers</span></span>
|<span data-ttu-id="975d0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="975d0-121">Header</span></span>|<span data-ttu-id="975d0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="975d0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="975d0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="975d0-123">Authorization</span></span>|<span data-ttu-id="975d0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="975d0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="975d0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="975d0-125">Accept</span></span>|<span data-ttu-id="975d0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="975d0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="975d0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="975d0-127">Request body</span></span>
<span data-ttu-id="975d0-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="975d0-128">In the request body, supply a JSON representation for the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="975d0-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="975d0-129">The following table shows the properties that are required when you create the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).</span></span>

|<span data-ttu-id="975d0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="975d0-130">Property</span></span>|<span data-ttu-id="975d0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="975d0-131">Type</span></span>|<span data-ttu-id="975d0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="975d0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="975d0-133">id</span><span class="sxs-lookup"><span data-stu-id="975d0-133">id</span></span>|<span data-ttu-id="975d0-134">String</span><span class="sxs-lookup"><span data-stu-id="975d0-134">String</span></span>|<span data-ttu-id="975d0-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="975d0-135">Key of the entity.</span></span> <span data-ttu-id="975d0-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="975d0-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="975d0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="975d0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="975d0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="975d0-138">DateTimeOffset</span></span>|<span data-ttu-id="975d0-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="975d0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="975d0-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="975d0-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="975d0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="975d0-141">roleScopeTagIds</span></span>|<span data-ttu-id="975d0-142">String collection</span><span class="sxs-lookup"><span data-stu-id="975d0-142">String collection</span></span>|<span data-ttu-id="975d0-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="975d0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="975d0-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="975d0-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="975d0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="975d0-145">supportsScopeTags</span></span>|<span data-ttu-id="975d0-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="975d0-146">Boolean</span></span>|<span data-ttu-id="975d0-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="975d0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="975d0-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="975d0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="975d0-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="975d0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="975d0-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="975d0-150">This property is read-only.</span></span> <span data-ttu-id="975d0-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="975d0-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="975d0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="975d0-152">createdDateTime</span></span>|<span data-ttu-id="975d0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="975d0-153">DateTimeOffset</span></span>|<span data-ttu-id="975d0-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="975d0-154">DateTime the object was created.</span></span> <span data-ttu-id="975d0-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="975d0-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="975d0-156">description</span><span class="sxs-lookup"><span data-stu-id="975d0-156">description</span></span>|<span data-ttu-id="975d0-157">String</span><span class="sxs-lookup"><span data-stu-id="975d0-157">String</span></span>|<span data-ttu-id="975d0-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="975d0-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="975d0-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="975d0-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="975d0-160">displayName</span><span class="sxs-lookup"><span data-stu-id="975d0-160">displayName</span></span>|<span data-ttu-id="975d0-161">String</span><span class="sxs-lookup"><span data-stu-id="975d0-161">String</span></span>|<span data-ttu-id="975d0-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="975d0-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="975d0-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="975d0-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="975d0-164">version</span><span class="sxs-lookup"><span data-stu-id="975d0-164">version</span></span>|<span data-ttu-id="975d0-165">Int32</span><span class="sxs-lookup"><span data-stu-id="975d0-165">Int32</span></span>|<span data-ttu-id="975d0-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="975d0-166">Version of the device configuration.</span></span> <span data-ttu-id="975d0-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="975d0-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="975d0-168">useSecurityKeyForSignin</span><span class="sxs-lookup"><span data-stu-id="975d0-168">useSecurityKeyForSignin</span></span>|<span data-ttu-id="975d0-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="975d0-169">Boolean</span></span>|<span data-ttu-id="975d0-170">Valor booleano usado para ativar a chave de segurança Olá do Windows como uma credencial de logon.</span><span class="sxs-lookup"><span data-stu-id="975d0-170">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="975d0-171">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="975d0-171">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="975d0-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="975d0-172">Boolean</span></span>|<span data-ttu-id="975d0-173">Valor booleano usado para habilitar avançada antifalsificação para reconhecimento de recurso faciais na autenticação do Windows Olá face padrão.</span><span class="sxs-lookup"><span data-stu-id="975d0-173">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="975d0-174">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="975d0-174">pinMinimumLength</span></span>|<span data-ttu-id="975d0-175">Int32</span><span class="sxs-lookup"><span data-stu-id="975d0-175">Int32</span></span>|<span data-ttu-id="975d0-176">Valor inteiro que define o número mínimo de caracteres necessários para o Windows Olá PIN de negócios.</span><span class="sxs-lookup"><span data-stu-id="975d0-176">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="975d0-177">Os valores válidos são de 4 a 127 inclusive e menor ou igual ao valor definido para o PIN máximo.</span><span class="sxs-lookup"><span data-stu-id="975d0-177">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="975d0-178">Valores válidos 4 a 127</span><span class="sxs-lookup"><span data-stu-id="975d0-178">Valid values 4 to 127</span></span>|
|<span data-ttu-id="975d0-179">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="975d0-179">pinMaximumLength</span></span>|<span data-ttu-id="975d0-180">Int32</span><span class="sxs-lookup"><span data-stu-id="975d0-180">Int32</span></span>|<span data-ttu-id="975d0-181">Valor inteiro que define o número máximo de caracteres permitido para o trabalho PIN.</span><span class="sxs-lookup"><span data-stu-id="975d0-181">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="975d0-182">Valores válidos são de 4 a 127 inclusive e maior ou igual ao valor definido para o PIN mínimo.</span><span class="sxs-lookup"><span data-stu-id="975d0-182">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="975d0-183">Valores válidos 4 a 127</span><span class="sxs-lookup"><span data-stu-id="975d0-183">Valid values 4 to 127</span></span>|
|<span data-ttu-id="975d0-184">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="975d0-184">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="975d0-185">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="975d0-185">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="975d0-186">Esse valor configura o uso de caracteres maiusculos no Windows Olá PIN de negócios.</span><span class="sxs-lookup"><span data-stu-id="975d0-186">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="975d0-187">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="975d0-187">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="975d0-188">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="975d0-188">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="975d0-189">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="975d0-189">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="975d0-190">Esse valor configura o uso de caracteres minúsculos no Windows Olá PIN de negócios.</span><span class="sxs-lookup"><span data-stu-id="975d0-190">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="975d0-191">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="975d0-191">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="975d0-192">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="975d0-192">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="975d0-193">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="975d0-193">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="975d0-194">Controla a capacidade de usar caracteres especiais no Windows Olá PIN de negócios.</span><span class="sxs-lookup"><span data-stu-id="975d0-194">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="975d0-195">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="975d0-195">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="975d0-196">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="975d0-196">pinExpirationInDays</span></span>|<span data-ttu-id="975d0-197">Int32</span><span class="sxs-lookup"><span data-stu-id="975d0-197">Int32</span></span>|<span data-ttu-id="975d0-198">Valor inteiro Especifica o período (em dias) que um PIN pode ser usado antes que o sistema exige que o usuário alterá-la.</span><span class="sxs-lookup"><span data-stu-id="975d0-198">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="975d0-199">Valores válidos são 0 para 730 inclusive.</span><span class="sxs-lookup"><span data-stu-id="975d0-199">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="975d0-200">Valores válidos de 0 a 730</span><span class="sxs-lookup"><span data-stu-id="975d0-200">Valid values 0 to 730</span></span>|
|<span data-ttu-id="975d0-201">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="975d0-201">pinPreviousBlockCount</span></span>|<span data-ttu-id="975d0-202">Int32</span><span class="sxs-lookup"><span data-stu-id="975d0-202">Int32</span></span>|<span data-ttu-id="975d0-203">Controla a capacidade de impedir que os usuários utilizem antigas PINs.</span><span class="sxs-lookup"><span data-stu-id="975d0-203">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="975d0-204">Isso deve ser definido entre 0 e 50, inclusive, e o PIN atual do usuário está incluído nessa contagem.</span><span class="sxs-lookup"><span data-stu-id="975d0-204">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="975d0-205">Se definido como 0, anterior PINs não são armazenadas.</span><span class="sxs-lookup"><span data-stu-id="975d0-205">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="975d0-206">Histórico PIN não é preservado por meio de um PIN redefinir.</span><span class="sxs-lookup"><span data-stu-id="975d0-206">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="975d0-207">Valores válidos de 0 a 50</span><span class="sxs-lookup"><span data-stu-id="975d0-207">Valid values 0 to 50</span></span>|
|<span data-ttu-id="975d0-208">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="975d0-208">pinRecoveryEnabled</span></span>|<span data-ttu-id="975d0-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="975d0-209">Boolean</span></span>|<span data-ttu-id="975d0-210">Valor booleano que permite que um usuário alterar seus PINs usando o Windows Hello para o serviço de recuperação de PIN de negócios.</span><span class="sxs-lookup"><span data-stu-id="975d0-210">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="975d0-211">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="975d0-211">securityDeviceRequired</span></span>|<span data-ttu-id="975d0-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="975d0-212">Boolean</span></span>|<span data-ttu-id="975d0-213">Controla se será exigido um Trusted Platform Module (TPM) para provisionamento Windows Olá for Business.</span><span class="sxs-lookup"><span data-stu-id="975d0-213">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="975d0-214">Um TPM fornece um benefício de segurança adicionais em que os dados armazenados nela não podem ser usados em outros dispositivos.</span><span class="sxs-lookup"><span data-stu-id="975d0-214">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="975d0-215">Se definido como False, todos os dispositivos podem provisionar Windows Olá for Business, mesmo se não houver um TPM utilizável.</span><span class="sxs-lookup"><span data-stu-id="975d0-215">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="975d0-216">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="975d0-216">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="975d0-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="975d0-217">Boolean</span></span>|<span data-ttu-id="975d0-218">Controla o uso de gestos biométricos, como nominal e a impressão digital, como uma alternativa para o Windows Olá PIN de negócios.</span><span class="sxs-lookup"><span data-stu-id="975d0-218">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="975d0-219">Se definido como False, biométricos gestos não é permitido.</span><span class="sxs-lookup"><span data-stu-id="975d0-219">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="975d0-220">Os usuários ainda devem configurar um PIN como um backup em caso de falhas.</span><span class="sxs-lookup"><span data-stu-id="975d0-220">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="975d0-221">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="975d0-221">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="975d0-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="975d0-222">Boolean</span></span>|<span data-ttu-id="975d0-223">Valor Boolean que permite Windows Olá for Business usar certificados para autenticar os recursos no local.</span><span class="sxs-lookup"><span data-stu-id="975d0-223">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="975d0-224">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="975d0-224">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="975d0-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="975d0-225">Boolean</span></span>|<span data-ttu-id="975d0-226">Valor Boolean que bloqueia Windows Olá para negócios como um método para fazer o login no Windows.</span><span class="sxs-lookup"><span data-stu-id="975d0-226">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="975d0-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="975d0-227">Response</span></span>
<span data-ttu-id="975d0-228">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="975d0-228">If successful, this method returns a `200 OK` response code and an updated [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="975d0-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="975d0-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="975d0-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="975d0-230">Request</span></span>
<span data-ttu-id="975d0-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="975d0-231">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="975d0-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="975d0-232">Response</span></span>
<span data-ttu-id="975d0-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="975d0-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




