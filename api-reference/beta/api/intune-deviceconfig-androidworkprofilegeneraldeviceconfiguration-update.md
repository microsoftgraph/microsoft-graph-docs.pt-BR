---
title: Atualizar Entidadeandroidforworkprofiledeviceconfiguration
description: Atualiza as propriedades de um objeto Entidadeandroidforworkprofiledeviceconfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 282584140243b8142ffe6a1919657efef5126a2f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443479"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="b126c-103">Atualizar Entidadeandroidforworkprofiledeviceconfiguration</span><span class="sxs-lookup"><span data-stu-id="b126c-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="b126c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b126c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b126c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b126c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b126c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b126c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b126c-107">Atualiza as propriedades de um objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b126c-107">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b126c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b126c-108">Prerequisites</span></span>
<span data-ttu-id="b126c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b126c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b126c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b126c-111">Permission type</span></span>|<span data-ttu-id="b126c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b126c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b126c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b126c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b126c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b126c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b126c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b126c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b126c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b126c-116">Not supported.</span></span>|
|<span data-ttu-id="b126c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b126c-117">Application</span></span>|<span data-ttu-id="b126c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b126c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b126c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b126c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b126c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b126c-120">Request headers</span></span>
|<span data-ttu-id="b126c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b126c-121">Header</span></span>|<span data-ttu-id="b126c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b126c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b126c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b126c-123">Authorization</span></span>|<span data-ttu-id="b126c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b126c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b126c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b126c-125">Accept</span></span>|<span data-ttu-id="b126c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b126c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b126c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b126c-127">Request body</span></span>
<span data-ttu-id="b126c-128">No corpo da solicitação, forneça uma representação JSON do objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b126c-128">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="b126c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b126c-129">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="b126c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b126c-130">Property</span></span>|<span data-ttu-id="b126c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b126c-131">Type</span></span>|<span data-ttu-id="b126c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b126c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b126c-133">id</span><span class="sxs-lookup"><span data-stu-id="b126c-133">id</span></span>|<span data-ttu-id="b126c-134">String</span><span class="sxs-lookup"><span data-stu-id="b126c-134">String</span></span>|<span data-ttu-id="b126c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b126c-135">Key of the entity.</span></span> <span data-ttu-id="b126c-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b126c-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b126c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b126c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b126c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b126c-138">DateTimeOffset</span></span>|<span data-ttu-id="b126c-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b126c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b126c-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b126c-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b126c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b126c-141">roleScopeTagIds</span></span>|<span data-ttu-id="b126c-142">String collection</span><span class="sxs-lookup"><span data-stu-id="b126c-142">String collection</span></span>|<span data-ttu-id="b126c-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="b126c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b126c-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b126c-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b126c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b126c-145">supportsScopeTags</span></span>|<span data-ttu-id="b126c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b126c-146">Boolean</span></span>|<span data-ttu-id="b126c-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b126c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b126c-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b126c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b126c-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b126c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b126c-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b126c-150">This property is read-only.</span></span> <span data-ttu-id="b126c-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b126c-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b126c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b126c-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b126c-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b126c-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b126c-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="b126c-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b126c-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b126c-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b126c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b126c-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b126c-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b126c-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b126c-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="b126c-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b126c-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b126c-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b126c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b126c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b126c-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b126c-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b126c-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="b126c-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b126c-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b126c-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b126c-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b126c-164">createdDateTime</span></span>|<span data-ttu-id="b126c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b126c-165">DateTimeOffset</span></span>|<span data-ttu-id="b126c-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b126c-166">DateTime the object was created.</span></span> <span data-ttu-id="b126c-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b126c-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b126c-168">description</span><span class="sxs-lookup"><span data-stu-id="b126c-168">description</span></span>|<span data-ttu-id="b126c-169">String</span><span class="sxs-lookup"><span data-stu-id="b126c-169">String</span></span>|<span data-ttu-id="b126c-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b126c-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b126c-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b126c-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b126c-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b126c-172">displayName</span></span>|<span data-ttu-id="b126c-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b126c-173">String</span></span>|<span data-ttu-id="b126c-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b126c-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b126c-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b126c-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b126c-176">versão</span><span class="sxs-lookup"><span data-stu-id="b126c-176">version</span></span>|<span data-ttu-id="b126c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b126c-177">Int32</span></span>|<span data-ttu-id="b126c-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b126c-178">Version of the device configuration.</span></span> <span data-ttu-id="b126c-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b126c-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b126c-180">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="b126c-180">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="b126c-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="b126c-181">Boolean</span></span>|<span data-ttu-id="b126c-182">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b126c-182">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="b126c-183">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="b126c-183">passwordBlockTrustAgents</span></span>|<span data-ttu-id="b126c-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="b126c-184">Boolean</span></span>|<span data-ttu-id="b126c-185">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="b126c-185">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="b126c-186">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b126c-186">passwordExpirationDays</span></span>|<span data-ttu-id="b126c-187">Int32</span><span class="sxs-lookup"><span data-stu-id="b126c-187">Int32</span></span>|<span data-ttu-id="b126c-188">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="b126c-188">Number of days before the password expires.</span></span> <span data-ttu-id="b126c-189">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="b126c-189">Valid values 1 to 365</span></span>|
|<span data-ttu-id="b126c-190">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b126c-190">passwordMinimumLength</span></span>|<span data-ttu-id="b126c-191">Int32</span><span class="sxs-lookup"><span data-stu-id="b126c-191">Int32</span></span>|<span data-ttu-id="b126c-192">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="b126c-192">Minimum length of passwords.</span></span> <span data-ttu-id="b126c-193">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="b126c-193">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b126c-194">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b126c-194">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b126c-195">Int32</span><span class="sxs-lookup"><span data-stu-id="b126c-195">Int32</span></span>|<span data-ttu-id="b126c-196">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="b126c-196">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b126c-197">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b126c-197">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b126c-198">Int32</span><span class="sxs-lookup"><span data-stu-id="b126c-198">Int32</span></span>|<span data-ttu-id="b126c-199">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="b126c-199">Number of previous passwords to block.</span></span> <span data-ttu-id="b126c-200">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="b126c-200">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b126c-201">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b126c-201">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b126c-202">Int32</span><span class="sxs-lookup"><span data-stu-id="b126c-202">Int32</span></span>|<span data-ttu-id="b126c-203">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="b126c-203">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="b126c-204">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="b126c-204">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b126c-205">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b126c-205">passwordRequiredType</span></span>|[<span data-ttu-id="b126c-206">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b126c-206">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="b126c-207">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="b126c-207">Type of password that is required.</span></span> <span data-ttu-id="b126c-208">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="b126c-208">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="b126c-209">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="b126c-209">workProfileDataSharingType</span></span>|[<span data-ttu-id="b126c-210">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="b126c-210">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="b126c-211">Tipo de compartilhamento de dados permitido.</span><span class="sxs-lookup"><span data-stu-id="b126c-211">Type of data sharing that is allowed.</span></span> <span data-ttu-id="b126c-212">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="b126c-212">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="b126c-213">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="b126c-213">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="b126c-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="b126c-214">Boolean</span></span>|<span data-ttu-id="b126c-215">Indica se as notificações devem ou não ser bloqueadas enquanto o dispositivo estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b126c-215">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="b126c-216">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="b126c-216">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="b126c-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="b126c-217">Boolean</span></span>|<span data-ttu-id="b126c-218">Impedir que os usuários adicionem/removam contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="b126c-218">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="b126c-219">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="b126c-219">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="b126c-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="b126c-220">Boolean</span></span>|<span data-ttu-id="b126c-221">Permitir que dispositivos Bluetooth acessem contatos da empresa.</span><span class="sxs-lookup"><span data-stu-id="b126c-221">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="b126c-222">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="b126c-222">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="b126c-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="b126c-223">Boolean</span></span>|<span data-ttu-id="b126c-224">Bloquear captura de tela em perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="b126c-224">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="b126c-225">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="b126c-225">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="b126c-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="b126c-226">Boolean</span></span>|<span data-ttu-id="b126c-227">Bloquear exibir ID de chamadas de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="b126c-227">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="b126c-228">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="b126c-228">workProfileBlockCamera</span></span>|<span data-ttu-id="b126c-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="b126c-229">Boolean</span></span>|<span data-ttu-id="b126c-230">Bloquear câmera de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="b126c-230">Block work profile camera.</span></span>|
|<span data-ttu-id="b126c-231">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="b126c-231">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="b126c-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="b126c-232">Boolean</span></span>|<span data-ttu-id="b126c-233">Bloquear disponibilidade de contatos de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="b126c-233">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="b126c-234">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="b126c-234">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="b126c-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="b126c-235">Boolean</span></span>|<span data-ttu-id="b126c-236">Booliano que indica se a configuração de desautorizar a cópia/colagem entre perfis está habilitada.</span><span class="sxs-lookup"><span data-stu-id="b126c-236">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="b126c-237">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="b126c-237">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="b126c-238">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="b126c-238">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="b126c-239">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="b126c-239">Type of password that is required.</span></span> <span data-ttu-id="b126c-240">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="b126c-240">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="b126c-241">Propriedades workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="b126c-241">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="b126c-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="b126c-242">Boolean</span></span>|<span data-ttu-id="b126c-243">Indica se o desbloqueio de impressão digital para o perfil de trabalho deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b126c-243">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="b126c-244">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="b126c-244">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="b126c-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="b126c-245">Boolean</span></span>|<span data-ttu-id="b126c-246">Indica se o bloqueio inteligente e outros agentes de confiança devem ou não ser bloqueados para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="b126c-246">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="b126c-247">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b126c-247">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="b126c-248">Int32</span><span class="sxs-lookup"><span data-stu-id="b126c-248">Int32</span></span>|<span data-ttu-id="b126c-249">Número de dias antes da senha do perfil de trabalho expirar.</span><span class="sxs-lookup"><span data-stu-id="b126c-249">Number of days before the work profile password expires.</span></span> <span data-ttu-id="b126c-250">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="b126c-250">Valid values 1 to 365</span></span>|
|<span data-ttu-id="b126c-251">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b126c-251">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="b126c-252">Int32</span><span class="sxs-lookup"><span data-stu-id="b126c-252">Int32</span></span>|<span data-ttu-id="b126c-253">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="b126c-253">Minimum length of work profile password.</span></span> <span data-ttu-id="b126c-254">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="b126c-254">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b126c-255">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="b126c-255">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="b126c-256">Int32</span><span class="sxs-lookup"><span data-stu-id="b126c-256">Int32</span></span>|<span data-ttu-id="b126c-257">Mínimo de caracteres numéricos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="b126c-257">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="b126c-258">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="b126c-258">Valid values 1 to 10</span></span>|
|<span data-ttu-id="b126c-259">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="b126c-259">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="b126c-260">Int32</span><span class="sxs-lookup"><span data-stu-id="b126c-260">Int32</span></span>|<span data-ttu-id="b126c-261">Número mínimo de caracteres não carta necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="b126c-261">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="b126c-262">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="b126c-262">Valid values 1 to 10</span></span>|
|<span data-ttu-id="b126c-263">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="b126c-263">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="b126c-264">Int32</span><span class="sxs-lookup"><span data-stu-id="b126c-264">Int32</span></span>|<span data-ttu-id="b126c-265">Número mínimo de caracteres de letras necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="b126c-265">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="b126c-266">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="b126c-266">Valid values 1 to 10</span></span>|
|<span data-ttu-id="b126c-267">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="b126c-267">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="b126c-268">Int32</span><span class="sxs-lookup"><span data-stu-id="b126c-268">Int32</span></span>|<span data-ttu-id="b126c-269">Número mínimo de caracteres em minúsculas exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="b126c-269">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="b126c-270">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="b126c-270">Valid values 1 to 10</span></span>|
|<span data-ttu-id="b126c-271">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="b126c-271">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="b126c-272">Int32</span><span class="sxs-lookup"><span data-stu-id="b126c-272">Int32</span></span>|<span data-ttu-id="b126c-273">Número mínimo de caracteres em maiúsculas obrigatórios na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="b126c-273">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="b126c-274">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="b126c-274">Valid values 1 to 10</span></span>|
|<span data-ttu-id="b126c-275">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="b126c-275">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="b126c-276">Int32</span><span class="sxs-lookup"><span data-stu-id="b126c-276">Int32</span></span>|<span data-ttu-id="b126c-277">Número mínimo de símbolos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="b126c-277">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="b126c-278">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="b126c-278">Valid values 1 to 10</span></span>|
|<span data-ttu-id="b126c-279">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b126c-279">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b126c-280">Int32</span><span class="sxs-lookup"><span data-stu-id="b126c-280">Int32</span></span>|<span data-ttu-id="b126c-281">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="b126c-281">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b126c-282">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b126c-282">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b126c-283">Int32</span><span class="sxs-lookup"><span data-stu-id="b126c-283">Int32</span></span>|<span data-ttu-id="b126c-284">Número de senhas de perfil de trabalho anteriores a serem bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="b126c-284">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="b126c-285">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="b126c-285">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b126c-286">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b126c-286">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b126c-287">Int32</span><span class="sxs-lookup"><span data-stu-id="b126c-287">Int32</span></span>|<span data-ttu-id="b126c-288">Número de falhas de entrada permitidas antes que o perfil de trabalho seja removido e todos os dados corporativos excluídos.</span><span class="sxs-lookup"><span data-stu-id="b126c-288">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="b126c-289">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="b126c-289">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b126c-290">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b126c-290">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="b126c-291">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b126c-291">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="b126c-292">Tipo de senha de perfil de trabalho necessário.</span><span class="sxs-lookup"><span data-stu-id="b126c-292">Type of work profile password that is required.</span></span> <span data-ttu-id="b126c-293">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="b126c-293">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="b126c-294">Workprofilerequirepassword foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="b126c-294">workProfileRequirePassword</span></span>|<span data-ttu-id="b126c-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="b126c-295">Boolean</span></span>|<span data-ttu-id="b126c-296">A senha é obrigatória ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="b126c-296">Password is required or not for work profile</span></span>|
|<span data-ttu-id="b126c-297">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="b126c-297">securityRequireVerifyApps</span></span>|<span data-ttu-id="b126c-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="b126c-298">Boolean</span></span>|<span data-ttu-id="b126c-299">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="b126c-299">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="b126c-300">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="b126c-300">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="b126c-301">String</span><span class="sxs-lookup"><span data-stu-id="b126c-301">String</span></span>|<span data-ttu-id="b126c-302">Habilitar o modo de bloqueio para VPN Always-on.</span><span class="sxs-lookup"><span data-stu-id="b126c-302">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="b126c-303">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="b126c-303">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="b126c-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="b126c-304">Boolean</span></span>|<span data-ttu-id="b126c-305">Habilitar o modo de bloqueio para VPN Always-on.</span><span class="sxs-lookup"><span data-stu-id="b126c-305">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="b126c-306">workProfileAllowWidgets</span><span class="sxs-lookup"><span data-stu-id="b126c-306">workProfileAllowWidgets</span></span>|<span data-ttu-id="b126c-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="b126c-307">Boolean</span></span>|<span data-ttu-id="b126c-308">Permitir widgets de aplicativos de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="b126c-308">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="b126c-309">workProfileBlockPersonalAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="b126c-309">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="b126c-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="b126c-310">Boolean</span></span>|<span data-ttu-id="b126c-311">Impedir instalações de aplicativos de fontes desconhecidas no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="b126c-311">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="b126c-312">Resposta</span><span class="sxs-lookup"><span data-stu-id="b126c-312">Response</span></span>
<span data-ttu-id="b126c-313">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b126c-313">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b126c-314">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b126c-314">Example</span></span>

### <a name="request"></a><span data-ttu-id="b126c-315">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b126c-315">Request</span></span>
<span data-ttu-id="b126c-316">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b126c-316">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2917

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
  "workProfileAllowWidgets": true,
  "workProfileBlockPersonalAppInstallsFromUnknownSources": true
}
```

### <a name="response"></a><span data-ttu-id="b126c-317">Resposta</span><span class="sxs-lookup"><span data-stu-id="b126c-317">Response</span></span>
<span data-ttu-id="b126c-p131">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b126c-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3089

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
  "workProfileAllowWidgets": true,
  "workProfileBlockPersonalAppInstallsFromUnknownSources": true
}
```





