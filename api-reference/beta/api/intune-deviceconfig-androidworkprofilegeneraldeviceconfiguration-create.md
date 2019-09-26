---
title: Criar Entidadeandroidforworkprofiledeviceconfiguration
description: Criar um novo objeto Entidadeandroidforworkprofiledeviceconfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bad851a899f316470ba43c24df236f979e273dcb
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37168737"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="2d33a-103">Criar Entidadeandroidforworkprofiledeviceconfiguration</span><span class="sxs-lookup"><span data-stu-id="2d33a-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="2d33a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2d33a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d33a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d33a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d33a-106">Criar um novo objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2d33a-106">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d33a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2d33a-107">Prerequisites</span></span>
<span data-ttu-id="2d33a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d33a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d33a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d33a-110">Permission type</span></span>|<span data-ttu-id="2d33a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2d33a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d33a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d33a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d33a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d33a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d33a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d33a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d33a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d33a-115">Not supported.</span></span>|
|<span data-ttu-id="2d33a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d33a-116">Application</span></span>|<span data-ttu-id="2d33a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d33a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d33a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d33a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2d33a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d33a-119">Request headers</span></span>
|<span data-ttu-id="2d33a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2d33a-120">Header</span></span>|<span data-ttu-id="2d33a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2d33a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d33a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d33a-122">Authorization</span></span>|<span data-ttu-id="2d33a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d33a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d33a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2d33a-124">Accept</span></span>|<span data-ttu-id="2d33a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d33a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d33a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d33a-126">Request body</span></span>
<span data-ttu-id="2d33a-127">No corpo da solicitação, forneça uma representação JSON do objeto Entidadeandroidforworkprofiledeviceconfiguration.</span><span class="sxs-lookup"><span data-stu-id="2d33a-127">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="2d33a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar Entidadeandroidforworkprofiledeviceconfiguration.</span><span class="sxs-lookup"><span data-stu-id="2d33a-128">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="2d33a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d33a-129">Property</span></span>|<span data-ttu-id="2d33a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d33a-130">Type</span></span>|<span data-ttu-id="2d33a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d33a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d33a-132">id</span><span class="sxs-lookup"><span data-stu-id="2d33a-132">id</span></span>|<span data-ttu-id="2d33a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d33a-133">String</span></span>|<span data-ttu-id="2d33a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2d33a-134">Key of the entity.</span></span> <span data-ttu-id="2d33a-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d33a-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d33a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d33a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2d33a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d33a-137">DateTimeOffset</span></span>|<span data-ttu-id="2d33a-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2d33a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2d33a-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d33a-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d33a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2d33a-140">roleScopeTagIds</span></span>|<span data-ttu-id="2d33a-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d33a-141">String collection</span></span>|<span data-ttu-id="2d33a-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="2d33a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2d33a-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d33a-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d33a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2d33a-144">supportsScopeTags</span></span>|<span data-ttu-id="2d33a-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d33a-145">Boolean</span></span>|<span data-ttu-id="2d33a-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="2d33a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2d33a-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="2d33a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2d33a-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="2d33a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2d33a-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2d33a-149">This property is read-only.</span></span> <span data-ttu-id="2d33a-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d33a-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d33a-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2d33a-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2d33a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2d33a-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2d33a-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="2d33a-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2d33a-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d33a-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d33a-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2d33a-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2d33a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2d33a-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2d33a-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="2d33a-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2d33a-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d33a-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d33a-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2d33a-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2d33a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2d33a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2d33a-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="2d33a-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2d33a-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d33a-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d33a-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2d33a-163">createdDateTime</span></span>|<span data-ttu-id="2d33a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d33a-164">DateTimeOffset</span></span>|<span data-ttu-id="2d33a-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2d33a-165">DateTime the object was created.</span></span> <span data-ttu-id="2d33a-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d33a-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d33a-167">descrição</span><span class="sxs-lookup"><span data-stu-id="2d33a-167">description</span></span>|<span data-ttu-id="2d33a-168">String</span><span class="sxs-lookup"><span data-stu-id="2d33a-168">String</span></span>|<span data-ttu-id="2d33a-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2d33a-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2d33a-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d33a-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d33a-171">displayName</span><span class="sxs-lookup"><span data-stu-id="2d33a-171">displayName</span></span>|<span data-ttu-id="2d33a-172">String</span><span class="sxs-lookup"><span data-stu-id="2d33a-172">String</span></span>|<span data-ttu-id="2d33a-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2d33a-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2d33a-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d33a-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d33a-175">versão</span><span class="sxs-lookup"><span data-stu-id="2d33a-175">version</span></span>|<span data-ttu-id="2d33a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2d33a-176">Int32</span></span>|<span data-ttu-id="2d33a-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2d33a-177">Version of the device configuration.</span></span> <span data-ttu-id="2d33a-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d33a-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d33a-179">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="2d33a-179">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="2d33a-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d33a-180">Boolean</span></span>|<span data-ttu-id="2d33a-181">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="2d33a-181">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="2d33a-182">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="2d33a-182">passwordBlockTrustAgents</span></span>|<span data-ttu-id="2d33a-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d33a-183">Boolean</span></span>|<span data-ttu-id="2d33a-184">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="2d33a-184">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="2d33a-185">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2d33a-185">passwordExpirationDays</span></span>|<span data-ttu-id="2d33a-186">Int32</span><span class="sxs-lookup"><span data-stu-id="2d33a-186">Int32</span></span>|<span data-ttu-id="2d33a-187">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="2d33a-187">Number of days before the password expires.</span></span> <span data-ttu-id="2d33a-188">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="2d33a-188">Valid values 1 to 365</span></span>|
|<span data-ttu-id="2d33a-189">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2d33a-189">passwordMinimumLength</span></span>|<span data-ttu-id="2d33a-190">Int32</span><span class="sxs-lookup"><span data-stu-id="2d33a-190">Int32</span></span>|<span data-ttu-id="2d33a-191">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="2d33a-191">Minimum length of passwords.</span></span> <span data-ttu-id="2d33a-192">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="2d33a-192">Valid values 4 to 16</span></span>|
|<span data-ttu-id="2d33a-193">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="2d33a-193">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="2d33a-194">Int32</span><span class="sxs-lookup"><span data-stu-id="2d33a-194">Int32</span></span>|<span data-ttu-id="2d33a-195">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="2d33a-195">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="2d33a-196">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2d33a-196">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2d33a-197">Int32</span><span class="sxs-lookup"><span data-stu-id="2d33a-197">Int32</span></span>|<span data-ttu-id="2d33a-198">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="2d33a-198">Number of previous passwords to block.</span></span> <span data-ttu-id="2d33a-199">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="2d33a-199">Valid values 0 to 24</span></span>|
|<span data-ttu-id="2d33a-200">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="2d33a-200">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="2d33a-201">Int32</span><span class="sxs-lookup"><span data-stu-id="2d33a-201">Int32</span></span>|<span data-ttu-id="2d33a-202">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="2d33a-202">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="2d33a-203">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="2d33a-203">Valid values 1 to 16</span></span>|
|<span data-ttu-id="2d33a-204">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2d33a-204">passwordRequiredType</span></span>|[<span data-ttu-id="2d33a-205">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2d33a-205">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="2d33a-206">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="2d33a-206">Type of password that is required.</span></span> <span data-ttu-id="2d33a-207">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="2d33a-207">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="2d33a-208">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="2d33a-208">workProfileDataSharingType</span></span>|[<span data-ttu-id="2d33a-209">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="2d33a-209">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="2d33a-210">Tipo de compartilhamento de dados permitido.</span><span class="sxs-lookup"><span data-stu-id="2d33a-210">Type of data sharing that is allowed.</span></span> <span data-ttu-id="2d33a-211">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="2d33a-211">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="2d33a-212">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="2d33a-212">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="2d33a-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d33a-213">Boolean</span></span>|<span data-ttu-id="2d33a-214">Indica se as notificações devem ou não ser bloqueadas enquanto o dispositivo estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="2d33a-214">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="2d33a-215">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="2d33a-215">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="2d33a-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d33a-216">Boolean</span></span>|<span data-ttu-id="2d33a-217">Impedir que os usuários adicionem/removam contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2d33a-217">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="2d33a-218">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="2d33a-218">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="2d33a-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d33a-219">Boolean</span></span>|<span data-ttu-id="2d33a-220">Permitir que dispositivos Bluetooth acessem contatos da empresa.</span><span class="sxs-lookup"><span data-stu-id="2d33a-220">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="2d33a-221">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="2d33a-221">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="2d33a-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d33a-222">Boolean</span></span>|<span data-ttu-id="2d33a-223">Bloquear captura de tela em perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2d33a-223">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="2d33a-224">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="2d33a-224">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="2d33a-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d33a-225">Boolean</span></span>|<span data-ttu-id="2d33a-226">Bloquear exibir ID de chamadas de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="2d33a-226">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="2d33a-227">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="2d33a-227">workProfileBlockCamera</span></span>|<span data-ttu-id="2d33a-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d33a-228">Boolean</span></span>|<span data-ttu-id="2d33a-229">Bloquear câmera de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2d33a-229">Block work profile camera.</span></span>|
|<span data-ttu-id="2d33a-230">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="2d33a-230">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="2d33a-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d33a-231">Boolean</span></span>|<span data-ttu-id="2d33a-232">Bloquear disponibilidade de contatos de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="2d33a-232">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="2d33a-233">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="2d33a-233">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="2d33a-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d33a-234">Boolean</span></span>|<span data-ttu-id="2d33a-235">Booliano que indica se a configuração de desautorizar a cópia/colagem entre perfis está habilitada.</span><span class="sxs-lookup"><span data-stu-id="2d33a-235">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="2d33a-236">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="2d33a-236">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="2d33a-237">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="2d33a-237">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="2d33a-238">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="2d33a-238">Type of password that is required.</span></span> <span data-ttu-id="2d33a-239">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="2d33a-239">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="2d33a-240">Propriedades workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="2d33a-240">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="2d33a-241">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d33a-241">Boolean</span></span>|<span data-ttu-id="2d33a-242">Indica se o desbloqueio de impressão digital para o perfil de trabalho deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="2d33a-242">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="2d33a-243">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="2d33a-243">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="2d33a-244">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d33a-244">Boolean</span></span>|<span data-ttu-id="2d33a-245">Indica se o bloqueio inteligente e outros agentes de confiança devem ou não ser bloqueados para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2d33a-245">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="2d33a-246">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2d33a-246">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="2d33a-247">Int32</span><span class="sxs-lookup"><span data-stu-id="2d33a-247">Int32</span></span>|<span data-ttu-id="2d33a-248">Número de dias antes da senha do perfil de trabalho expirar.</span><span class="sxs-lookup"><span data-stu-id="2d33a-248">Number of days before the work profile password expires.</span></span> <span data-ttu-id="2d33a-249">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="2d33a-249">Valid values 1 to 365</span></span>|
|<span data-ttu-id="2d33a-250">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2d33a-250">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="2d33a-251">Int32</span><span class="sxs-lookup"><span data-stu-id="2d33a-251">Int32</span></span>|<span data-ttu-id="2d33a-252">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2d33a-252">Minimum length of work profile password.</span></span> <span data-ttu-id="2d33a-253">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="2d33a-253">Valid values 4 to 16</span></span>|
|<span data-ttu-id="2d33a-254">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="2d33a-254">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="2d33a-255">Int32</span><span class="sxs-lookup"><span data-stu-id="2d33a-255">Int32</span></span>|<span data-ttu-id="2d33a-256">Mínimo de caracteres numéricos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2d33a-256">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="2d33a-257">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="2d33a-257">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2d33a-258">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="2d33a-258">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="2d33a-259">Int32</span><span class="sxs-lookup"><span data-stu-id="2d33a-259">Int32</span></span>|<span data-ttu-id="2d33a-260">Número mínimo de caracteres não carta necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2d33a-260">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="2d33a-261">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="2d33a-261">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2d33a-262">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="2d33a-262">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="2d33a-263">Int32</span><span class="sxs-lookup"><span data-stu-id="2d33a-263">Int32</span></span>|<span data-ttu-id="2d33a-264">Número mínimo de caracteres de letras necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2d33a-264">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="2d33a-265">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="2d33a-265">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2d33a-266">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="2d33a-266">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="2d33a-267">Int32</span><span class="sxs-lookup"><span data-stu-id="2d33a-267">Int32</span></span>|<span data-ttu-id="2d33a-268">Número mínimo de caracteres em minúsculas exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2d33a-268">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="2d33a-269">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="2d33a-269">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2d33a-270">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="2d33a-270">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="2d33a-271">Int32</span><span class="sxs-lookup"><span data-stu-id="2d33a-271">Int32</span></span>|<span data-ttu-id="2d33a-272">Número mínimo de caracteres em maiúsculas obrigatórios na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2d33a-272">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="2d33a-273">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="2d33a-273">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2d33a-274">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="2d33a-274">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="2d33a-275">Int32</span><span class="sxs-lookup"><span data-stu-id="2d33a-275">Int32</span></span>|<span data-ttu-id="2d33a-276">Número mínimo de símbolos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2d33a-276">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="2d33a-277">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="2d33a-277">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2d33a-278">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="2d33a-278">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="2d33a-279">Int32</span><span class="sxs-lookup"><span data-stu-id="2d33a-279">Int32</span></span>|<span data-ttu-id="2d33a-280">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="2d33a-280">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="2d33a-281">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2d33a-281">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2d33a-282">Int32</span><span class="sxs-lookup"><span data-stu-id="2d33a-282">Int32</span></span>|<span data-ttu-id="2d33a-283">Número de senhas de perfil de trabalho anteriores a serem bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="2d33a-283">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="2d33a-284">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="2d33a-284">Valid values 0 to 24</span></span>|
|<span data-ttu-id="2d33a-285">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="2d33a-285">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="2d33a-286">Int32</span><span class="sxs-lookup"><span data-stu-id="2d33a-286">Int32</span></span>|<span data-ttu-id="2d33a-287">Número de falhas de entrada permitidas antes que o perfil de trabalho seja removido e todos os dados corporativos excluídos.</span><span class="sxs-lookup"><span data-stu-id="2d33a-287">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="2d33a-288">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="2d33a-288">Valid values 1 to 16</span></span>|
|<span data-ttu-id="2d33a-289">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2d33a-289">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="2d33a-290">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2d33a-290">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="2d33a-291">Tipo de senha de perfil de trabalho necessário.</span><span class="sxs-lookup"><span data-stu-id="2d33a-291">Type of work profile password that is required.</span></span> <span data-ttu-id="2d33a-292">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="2d33a-292">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="2d33a-293">Workprofilerequirepassword foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="2d33a-293">workProfileRequirePassword</span></span>|<span data-ttu-id="2d33a-294">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d33a-294">Boolean</span></span>|<span data-ttu-id="2d33a-295">A senha é obrigatória ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="2d33a-295">Password is required or not for work profile</span></span>|
|<span data-ttu-id="2d33a-296">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="2d33a-296">securityRequireVerifyApps</span></span>|<span data-ttu-id="2d33a-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d33a-297">Boolean</span></span>|<span data-ttu-id="2d33a-298">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="2d33a-298">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="2d33a-299">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="2d33a-299">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="2d33a-300">String</span><span class="sxs-lookup"><span data-stu-id="2d33a-300">String</span></span>|<span data-ttu-id="2d33a-301">Habilitar o modo de bloqueio para VPN Always-on.</span><span class="sxs-lookup"><span data-stu-id="2d33a-301">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="2d33a-302">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="2d33a-302">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="2d33a-303">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d33a-303">Boolean</span></span>|<span data-ttu-id="2d33a-304">Habilitar o modo de bloqueio para VPN Always-on.</span><span class="sxs-lookup"><span data-stu-id="2d33a-304">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="2d33a-305">workProfileAllowWidgets</span><span class="sxs-lookup"><span data-stu-id="2d33a-305">workProfileAllowWidgets</span></span>|<span data-ttu-id="2d33a-306">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d33a-306">Boolean</span></span>|<span data-ttu-id="2d33a-307">Permitir widgets de aplicativos de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2d33a-307">Allow widgets from work profile apps.</span></span>|



## <a name="response"></a><span data-ttu-id="2d33a-308">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d33a-308">Response</span></span>
<span data-ttu-id="2d33a-309">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d33a-309">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d33a-310">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d33a-310">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d33a-311">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d33a-311">Request</span></span>
<span data-ttu-id="2d33a-312">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d33a-312">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2851

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
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
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true,
  "workProfileAllowWidgets": true
}
```

### <a name="response"></a><span data-ttu-id="2d33a-313">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d33a-313">Response</span></span>
<span data-ttu-id="2d33a-p131">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d33a-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3023

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
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
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true,
  "workProfileAllowWidgets": true
}
```




