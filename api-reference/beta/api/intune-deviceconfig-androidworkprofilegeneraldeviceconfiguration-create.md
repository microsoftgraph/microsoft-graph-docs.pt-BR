---
title: Criar Entidadeandroidforworkprofiledeviceconfiguration
description: Criar um novo objeto Entidadeandroidforworkprofiledeviceconfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3fdf7096b59fe908dbb310fd27608b59f6a09b22
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36340741"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="d7542-103">Criar Entidadeandroidforworkprofiledeviceconfiguration</span><span class="sxs-lookup"><span data-stu-id="d7542-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="d7542-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d7542-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7542-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d7542-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7542-106">Criar um novo objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d7542-106">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7542-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d7542-107">Prerequisites</span></span>
<span data-ttu-id="d7542-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7542-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7542-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7542-110">Permission type</span></span>|<span data-ttu-id="d7542-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d7542-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7542-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7542-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7542-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7542-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7542-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7542-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7542-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7542-115">Not supported.</span></span>|
|<span data-ttu-id="d7542-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7542-116">Application</span></span>|<span data-ttu-id="d7542-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7542-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7542-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7542-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d7542-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7542-119">Request headers</span></span>
|<span data-ttu-id="d7542-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d7542-120">Header</span></span>|<span data-ttu-id="d7542-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d7542-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7542-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7542-122">Authorization</span></span>|<span data-ttu-id="d7542-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7542-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7542-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d7542-124">Accept</span></span>|<span data-ttu-id="d7542-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7542-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7542-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7542-126">Request body</span></span>
<span data-ttu-id="d7542-127">No corpo da solicitação, forneça uma representação JSON do objeto Entidadeandroidforworkprofiledeviceconfiguration.</span><span class="sxs-lookup"><span data-stu-id="d7542-127">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="d7542-128">A tabela a seguir mostra as propriedades que são necessárias ao criar Entidadeandroidforworkprofiledeviceconfiguration.</span><span class="sxs-lookup"><span data-stu-id="d7542-128">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="d7542-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7542-129">Property</span></span>|<span data-ttu-id="d7542-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7542-130">Type</span></span>|<span data-ttu-id="d7542-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7542-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7542-132">id</span><span class="sxs-lookup"><span data-stu-id="d7542-132">id</span></span>|<span data-ttu-id="d7542-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7542-133">String</span></span>|<span data-ttu-id="d7542-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d7542-134">Key of the entity.</span></span> <span data-ttu-id="d7542-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7542-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7542-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7542-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d7542-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7542-137">DateTimeOffset</span></span>|<span data-ttu-id="d7542-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d7542-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d7542-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7542-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7542-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d7542-140">roleScopeTagIds</span></span>|<span data-ttu-id="d7542-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7542-141">String collection</span></span>|<span data-ttu-id="d7542-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d7542-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d7542-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7542-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7542-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d7542-144">supportsScopeTags</span></span>|<span data-ttu-id="d7542-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="d7542-145">Boolean</span></span>|<span data-ttu-id="d7542-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d7542-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d7542-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d7542-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d7542-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d7542-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d7542-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d7542-149">This property is read-only.</span></span> <span data-ttu-id="d7542-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7542-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7542-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d7542-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d7542-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d7542-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d7542-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="d7542-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d7542-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7542-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7542-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d7542-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d7542-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d7542-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d7542-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="d7542-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d7542-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7542-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7542-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d7542-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d7542-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d7542-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d7542-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="d7542-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d7542-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7542-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7542-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7542-163">createdDateTime</span></span>|<span data-ttu-id="d7542-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7542-164">DateTimeOffset</span></span>|<span data-ttu-id="d7542-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d7542-165">DateTime the object was created.</span></span> <span data-ttu-id="d7542-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7542-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7542-167">descrição</span><span class="sxs-lookup"><span data-stu-id="d7542-167">description</span></span>|<span data-ttu-id="d7542-168">String</span><span class="sxs-lookup"><span data-stu-id="d7542-168">String</span></span>|<span data-ttu-id="d7542-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d7542-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d7542-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7542-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7542-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d7542-171">displayName</span></span>|<span data-ttu-id="d7542-172">String</span><span class="sxs-lookup"><span data-stu-id="d7542-172">String</span></span>|<span data-ttu-id="d7542-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d7542-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d7542-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7542-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7542-175">versão</span><span class="sxs-lookup"><span data-stu-id="d7542-175">version</span></span>|<span data-ttu-id="d7542-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d7542-176">Int32</span></span>|<span data-ttu-id="d7542-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d7542-177">Version of the device configuration.</span></span> <span data-ttu-id="d7542-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7542-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7542-179">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="d7542-179">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="d7542-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="d7542-180">Boolean</span></span>|<span data-ttu-id="d7542-181">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d7542-181">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="d7542-182">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="d7542-182">passwordBlockTrustAgents</span></span>|<span data-ttu-id="d7542-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7542-183">Boolean</span></span>|<span data-ttu-id="d7542-184">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="d7542-184">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="d7542-185">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d7542-185">passwordExpirationDays</span></span>|<span data-ttu-id="d7542-186">Int32</span><span class="sxs-lookup"><span data-stu-id="d7542-186">Int32</span></span>|<span data-ttu-id="d7542-187">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="d7542-187">Number of days before the password expires.</span></span> <span data-ttu-id="d7542-188">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="d7542-188">Valid values 1 to 365</span></span>|
|<span data-ttu-id="d7542-189">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d7542-189">passwordMinimumLength</span></span>|<span data-ttu-id="d7542-190">Int32</span><span class="sxs-lookup"><span data-stu-id="d7542-190">Int32</span></span>|<span data-ttu-id="d7542-191">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="d7542-191">Minimum length of passwords.</span></span> <span data-ttu-id="d7542-192">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="d7542-192">Valid values 4 to 16</span></span>|
|<span data-ttu-id="d7542-193">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d7542-193">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d7542-194">Int32</span><span class="sxs-lookup"><span data-stu-id="d7542-194">Int32</span></span>|<span data-ttu-id="d7542-195">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="d7542-195">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="d7542-196">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d7542-196">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d7542-197">Int32</span><span class="sxs-lookup"><span data-stu-id="d7542-197">Int32</span></span>|<span data-ttu-id="d7542-198">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="d7542-198">Number of previous passwords to block.</span></span> <span data-ttu-id="d7542-199">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="d7542-199">Valid values 0 to 24</span></span>|
|<span data-ttu-id="d7542-200">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="d7542-200">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="d7542-201">Int32</span><span class="sxs-lookup"><span data-stu-id="d7542-201">Int32</span></span>|<span data-ttu-id="d7542-202">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="d7542-202">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="d7542-203">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="d7542-203">Valid values 1 to 16</span></span>|
|<span data-ttu-id="d7542-204">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d7542-204">passwordRequiredType</span></span>|[<span data-ttu-id="d7542-205">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d7542-205">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="d7542-206">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="d7542-206">Type of password that is required.</span></span> <span data-ttu-id="d7542-207">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="d7542-207">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="d7542-208">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="d7542-208">workProfileDataSharingType</span></span>|[<span data-ttu-id="d7542-209">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="d7542-209">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="d7542-210">Tipo de compartilhamento de dados permitido.</span><span class="sxs-lookup"><span data-stu-id="d7542-210">Type of data sharing that is allowed.</span></span> <span data-ttu-id="d7542-211">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="d7542-211">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="d7542-212">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="d7542-212">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="d7542-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="d7542-213">Boolean</span></span>|<span data-ttu-id="d7542-214">Indica se as notificações devem ou não ser bloqueadas enquanto o dispositivo estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d7542-214">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="d7542-215">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="d7542-215">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="d7542-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="d7542-216">Boolean</span></span>|<span data-ttu-id="d7542-217">Impedir que os usuários adicionem/removam contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d7542-217">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="d7542-218">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="d7542-218">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="d7542-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="d7542-219">Boolean</span></span>|<span data-ttu-id="d7542-220">Permitir que dispositivos Bluetooth acessem contatos da empresa.</span><span class="sxs-lookup"><span data-stu-id="d7542-220">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="d7542-221">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="d7542-221">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="d7542-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="d7542-222">Boolean</span></span>|<span data-ttu-id="d7542-223">Bloquear captura de tela em perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d7542-223">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="d7542-224">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="d7542-224">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="d7542-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="d7542-225">Boolean</span></span>|<span data-ttu-id="d7542-226">Bloquear exibir ID de chamadas de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="d7542-226">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="d7542-227">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="d7542-227">workProfileBlockCamera</span></span>|<span data-ttu-id="d7542-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="d7542-228">Boolean</span></span>|<span data-ttu-id="d7542-229">Bloquear câmera de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d7542-229">Block work profile camera.</span></span>|
|<span data-ttu-id="d7542-230">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="d7542-230">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="d7542-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="d7542-231">Boolean</span></span>|<span data-ttu-id="d7542-232">Bloquear disponibilidade de contatos de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="d7542-232">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="d7542-233">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="d7542-233">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="d7542-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="d7542-234">Boolean</span></span>|<span data-ttu-id="d7542-235">Booliano que indica se a configuração de desautorizar a cópia/colagem entre perfis está habilitada.</span><span class="sxs-lookup"><span data-stu-id="d7542-235">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="d7542-236">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="d7542-236">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="d7542-237">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="d7542-237">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="d7542-238">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="d7542-238">Type of password that is required.</span></span> <span data-ttu-id="d7542-239">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="d7542-239">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="d7542-240">Propriedades workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="d7542-240">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="d7542-241">Booliano</span><span class="sxs-lookup"><span data-stu-id="d7542-241">Boolean</span></span>|<span data-ttu-id="d7542-242">Indica se o desbloqueio de impressão digital para o perfil de trabalho deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d7542-242">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="d7542-243">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="d7542-243">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="d7542-244">Booliano</span><span class="sxs-lookup"><span data-stu-id="d7542-244">Boolean</span></span>|<span data-ttu-id="d7542-245">Indica se o bloqueio inteligente e outros agentes de confiança devem ou não ser bloqueados para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d7542-245">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="d7542-246">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d7542-246">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="d7542-247">Int32</span><span class="sxs-lookup"><span data-stu-id="d7542-247">Int32</span></span>|<span data-ttu-id="d7542-248">Número de dias antes da senha do perfil de trabalho expirar.</span><span class="sxs-lookup"><span data-stu-id="d7542-248">Number of days before the work profile password expires.</span></span> <span data-ttu-id="d7542-249">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="d7542-249">Valid values 1 to 365</span></span>|
|<span data-ttu-id="d7542-250">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d7542-250">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="d7542-251">Int32</span><span class="sxs-lookup"><span data-stu-id="d7542-251">Int32</span></span>|<span data-ttu-id="d7542-252">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d7542-252">Minimum length of work profile password.</span></span> <span data-ttu-id="d7542-253">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="d7542-253">Valid values 4 to 16</span></span>|
|<span data-ttu-id="d7542-254">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="d7542-254">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="d7542-255">Int32</span><span class="sxs-lookup"><span data-stu-id="d7542-255">Int32</span></span>|<span data-ttu-id="d7542-256">Mínimo de caracteres numéricos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d7542-256">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="d7542-257">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="d7542-257">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d7542-258">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="d7542-258">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="d7542-259">Int32</span><span class="sxs-lookup"><span data-stu-id="d7542-259">Int32</span></span>|<span data-ttu-id="d7542-260">Número mínimo de caracteres não carta necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d7542-260">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="d7542-261">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="d7542-261">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d7542-262">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="d7542-262">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="d7542-263">Int32</span><span class="sxs-lookup"><span data-stu-id="d7542-263">Int32</span></span>|<span data-ttu-id="d7542-264">Número mínimo de caracteres de letras necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d7542-264">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="d7542-265">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="d7542-265">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d7542-266">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="d7542-266">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="d7542-267">Int32</span><span class="sxs-lookup"><span data-stu-id="d7542-267">Int32</span></span>|<span data-ttu-id="d7542-268">Número mínimo de caracteres em minúsculas exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d7542-268">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="d7542-269">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="d7542-269">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d7542-270">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="d7542-270">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="d7542-271">Int32</span><span class="sxs-lookup"><span data-stu-id="d7542-271">Int32</span></span>|<span data-ttu-id="d7542-272">Número mínimo de caracteres em maiúsculas obrigatórios na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d7542-272">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="d7542-273">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="d7542-273">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d7542-274">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="d7542-274">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="d7542-275">Int32</span><span class="sxs-lookup"><span data-stu-id="d7542-275">Int32</span></span>|<span data-ttu-id="d7542-276">Número mínimo de símbolos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d7542-276">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="d7542-277">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="d7542-277">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d7542-278">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d7542-278">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d7542-279">Int32</span><span class="sxs-lookup"><span data-stu-id="d7542-279">Int32</span></span>|<span data-ttu-id="d7542-280">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="d7542-280">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="d7542-281">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d7542-281">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d7542-282">Int32</span><span class="sxs-lookup"><span data-stu-id="d7542-282">Int32</span></span>|<span data-ttu-id="d7542-283">Número de senhas de perfil de trabalho anteriores a serem bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="d7542-283">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="d7542-284">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="d7542-284">Valid values 0 to 24</span></span>|
|<span data-ttu-id="d7542-285">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="d7542-285">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="d7542-286">Int32</span><span class="sxs-lookup"><span data-stu-id="d7542-286">Int32</span></span>|<span data-ttu-id="d7542-287">Número de falhas de entrada permitidas antes que o perfil de trabalho seja removido e todos os dados corporativos excluídos.</span><span class="sxs-lookup"><span data-stu-id="d7542-287">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="d7542-288">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="d7542-288">Valid values 1 to 16</span></span>|
|<span data-ttu-id="d7542-289">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d7542-289">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="d7542-290">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d7542-290">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="d7542-291">Tipo de senha de perfil de trabalho necessário.</span><span class="sxs-lookup"><span data-stu-id="d7542-291">Type of work profile password that is required.</span></span> <span data-ttu-id="d7542-292">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="d7542-292">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="d7542-293">Workprofilerequirepassword foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="d7542-293">workProfileRequirePassword</span></span>|<span data-ttu-id="d7542-294">Booliano</span><span class="sxs-lookup"><span data-stu-id="d7542-294">Boolean</span></span>|<span data-ttu-id="d7542-295">A senha é obrigatória ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="d7542-295">Password is required or not for work profile</span></span>|
|<span data-ttu-id="d7542-296">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="d7542-296">securityRequireVerifyApps</span></span>|<span data-ttu-id="d7542-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7542-297">Boolean</span></span>|<span data-ttu-id="d7542-298">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="d7542-298">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="d7542-299">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="d7542-299">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="d7542-300">String</span><span class="sxs-lookup"><span data-stu-id="d7542-300">String</span></span>|<span data-ttu-id="d7542-301">Habilitar o modo de bloqueio para VPN Always-on.</span><span class="sxs-lookup"><span data-stu-id="d7542-301">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="d7542-302">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="d7542-302">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="d7542-303">Booliano</span><span class="sxs-lookup"><span data-stu-id="d7542-303">Boolean</span></span>|<span data-ttu-id="d7542-304">Habilitar o modo de bloqueio para VPN Always-on.</span><span class="sxs-lookup"><span data-stu-id="d7542-304">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="d7542-305">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7542-305">Response</span></span>
<span data-ttu-id="d7542-306">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7542-306">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7542-307">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7542-307">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7542-308">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7542-308">Request</span></span>
<span data-ttu-id="d7542-309">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7542-309">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2815

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
  "vpnEnableAlwaysOnLockdownMode": true
}
```

### <a name="response"></a><span data-ttu-id="d7542-310">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7542-310">Response</span></span>
<span data-ttu-id="d7542-p131">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7542-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2987

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
  "vpnEnableAlwaysOnLockdownMode": true
}
```






