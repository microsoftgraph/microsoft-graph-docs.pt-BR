---
title: Atualizar androidForWorkGeneralDeviceConfiguration
description: Atualiza as propriedades de um objeto androidForWorkGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2cd7bd5071c38d3921707259bcfb4a434b4776ec
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790872"
---
# <a name="update-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="6cf73-103">Atualizar androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="6cf73-103">Update androidForWorkGeneralDeviceConfiguration</span></span>

<span data-ttu-id="6cf73-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cf73-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6cf73-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6cf73-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cf73-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6cf73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cf73-107">Atualiza as propriedades de um objeto [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6cf73-107">Update the properties of a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cf73-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6cf73-108">Prerequisites</span></span>
<span data-ttu-id="6cf73-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cf73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cf73-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cf73-111">Permission type</span></span>|<span data-ttu-id="6cf73-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6cf73-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cf73-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cf73-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6cf73-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cf73-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6cf73-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cf73-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cf73-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cf73-116">Not supported.</span></span>|
|<span data-ttu-id="6cf73-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cf73-117">Application</span></span>|<span data-ttu-id="6cf73-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cf73-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cf73-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cf73-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6cf73-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cf73-120">Request headers</span></span>
|<span data-ttu-id="6cf73-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6cf73-121">Header</span></span>|<span data-ttu-id="6cf73-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6cf73-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cf73-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cf73-123">Authorization</span></span>|<span data-ttu-id="6cf73-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cf73-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cf73-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6cf73-125">Accept</span></span>|<span data-ttu-id="6cf73-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6cf73-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cf73-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cf73-127">Request body</span></span>
<span data-ttu-id="6cf73-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6cf73-128">In the request body, supply a JSON representation for the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="6cf73-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cf73-129">The following table shows the properties that are required when you create the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="6cf73-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6cf73-130">Property</span></span>|<span data-ttu-id="6cf73-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cf73-131">Type</span></span>|<span data-ttu-id="6cf73-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cf73-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cf73-133">id</span><span class="sxs-lookup"><span data-stu-id="6cf73-133">id</span></span>|<span data-ttu-id="6cf73-134">String</span><span class="sxs-lookup"><span data-stu-id="6cf73-134">String</span></span>|<span data-ttu-id="6cf73-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6cf73-135">Key of the entity.</span></span> <span data-ttu-id="6cf73-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cf73-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cf73-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6cf73-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6cf73-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cf73-138">DateTimeOffset</span></span>|<span data-ttu-id="6cf73-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6cf73-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6cf73-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cf73-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cf73-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6cf73-141">roleScopeTagIds</span></span>|<span data-ttu-id="6cf73-142">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cf73-142">String collection</span></span>|<span data-ttu-id="6cf73-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6cf73-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6cf73-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cf73-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cf73-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6cf73-145">supportsScopeTags</span></span>|<span data-ttu-id="6cf73-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-146">Boolean</span></span>|<span data-ttu-id="6cf73-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6cf73-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6cf73-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6cf73-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6cf73-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6cf73-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6cf73-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6cf73-150">This property is read-only.</span></span> <span data-ttu-id="6cf73-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cf73-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cf73-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6cf73-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6cf73-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6cf73-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6cf73-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="6cf73-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6cf73-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cf73-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cf73-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6cf73-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6cf73-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6cf73-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6cf73-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="6cf73-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6cf73-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cf73-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cf73-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6cf73-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6cf73-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6cf73-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6cf73-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="6cf73-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6cf73-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cf73-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cf73-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6cf73-164">createdDateTime</span></span>|<span data-ttu-id="6cf73-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cf73-165">DateTimeOffset</span></span>|<span data-ttu-id="6cf73-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6cf73-166">DateTime the object was created.</span></span> <span data-ttu-id="6cf73-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cf73-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cf73-168">description</span><span class="sxs-lookup"><span data-stu-id="6cf73-168">description</span></span>|<span data-ttu-id="6cf73-169">String</span><span class="sxs-lookup"><span data-stu-id="6cf73-169">String</span></span>|<span data-ttu-id="6cf73-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6cf73-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6cf73-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cf73-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cf73-172">displayName</span><span class="sxs-lookup"><span data-stu-id="6cf73-172">displayName</span></span>|<span data-ttu-id="6cf73-173">String</span><span class="sxs-lookup"><span data-stu-id="6cf73-173">String</span></span>|<span data-ttu-id="6cf73-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6cf73-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6cf73-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cf73-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cf73-176">versão</span><span class="sxs-lookup"><span data-stu-id="6cf73-176">version</span></span>|<span data-ttu-id="6cf73-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf73-177">Int32</span></span>|<span data-ttu-id="6cf73-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6cf73-178">Version of the device configuration.</span></span> <span data-ttu-id="6cf73-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cf73-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cf73-180">passwordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="6cf73-180">passwordBlockFaceUnlock</span></span>|<span data-ttu-id="6cf73-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-181">Boolean</span></span>|<span data-ttu-id="6cf73-182">Indica se o desbloqueio de face deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6cf73-182">Indicates whether or not to block face unlock.</span></span>|
|<span data-ttu-id="6cf73-183">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="6cf73-183">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="6cf73-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cf73-184">Boolean</span></span>|<span data-ttu-id="6cf73-185">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6cf73-185">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="6cf73-186">passwordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="6cf73-186">passwordBlockIrisUnlock</span></span>|<span data-ttu-id="6cf73-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-187">Boolean</span></span>|<span data-ttu-id="6cf73-188">Indica se o desbloqueio da íris deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6cf73-188">Indicates whether or not to block iris unlock.</span></span>|
|<span data-ttu-id="6cf73-189">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="6cf73-189">passwordBlockTrustAgents</span></span>|<span data-ttu-id="6cf73-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cf73-190">Boolean</span></span>|<span data-ttu-id="6cf73-191">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="6cf73-191">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="6cf73-192">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6cf73-192">passwordExpirationDays</span></span>|<span data-ttu-id="6cf73-193">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf73-193">Int32</span></span>|<span data-ttu-id="6cf73-194">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="6cf73-194">Number of days before the password expires.</span></span> <span data-ttu-id="6cf73-195">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="6cf73-195">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6cf73-196">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6cf73-196">passwordMinimumLength</span></span>|<span data-ttu-id="6cf73-197">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf73-197">Int32</span></span>|<span data-ttu-id="6cf73-198">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="6cf73-198">Minimum length of passwords.</span></span> <span data-ttu-id="6cf73-199">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="6cf73-199">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6cf73-200">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6cf73-200">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6cf73-201">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf73-201">Int32</span></span>|<span data-ttu-id="6cf73-202">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="6cf73-202">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6cf73-203">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6cf73-203">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6cf73-204">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf73-204">Int32</span></span>|<span data-ttu-id="6cf73-205">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="6cf73-205">Number of previous passwords to block.</span></span> <span data-ttu-id="6cf73-206">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="6cf73-206">Valid values 0 to 24</span></span>|
|<span data-ttu-id="6cf73-207">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="6cf73-207">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="6cf73-208">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf73-208">Int32</span></span>|<span data-ttu-id="6cf73-209">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="6cf73-209">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="6cf73-210">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="6cf73-210">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6cf73-211">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6cf73-211">passwordRequiredType</span></span>|[<span data-ttu-id="6cf73-212">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6cf73-212">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="6cf73-213">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="6cf73-213">Type of password that is required.</span></span> <span data-ttu-id="6cf73-214">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="6cf73-214">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="6cf73-215">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="6cf73-215">workProfileDataSharingType</span></span>|[<span data-ttu-id="6cf73-216">androidForWorkCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="6cf73-216">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="6cf73-217">Tipo de compartilhamento de dados permitido.</span><span class="sxs-lookup"><span data-stu-id="6cf73-217">Type of data sharing that is allowed.</span></span> <span data-ttu-id="6cf73-218">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="6cf73-218">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="6cf73-219">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="6cf73-219">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="6cf73-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-220">Boolean</span></span>|<span data-ttu-id="6cf73-221">Indica se as notificações devem ou não ser bloqueadas enquanto o dispositivo estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6cf73-221">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="6cf73-222">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="6cf73-222">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="6cf73-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-223">Boolean</span></span>|<span data-ttu-id="6cf73-224">Impedir que os usuários adicionem/removam contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6cf73-224">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="6cf73-225">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="6cf73-225">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="6cf73-226">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-226">Boolean</span></span>|<span data-ttu-id="6cf73-227">Permitir que dispositivos Bluetooth acessem contatos da empresa.</span><span class="sxs-lookup"><span data-stu-id="6cf73-227">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="6cf73-228">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="6cf73-228">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="6cf73-229">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-229">Boolean</span></span>|<span data-ttu-id="6cf73-230">Bloquear captura de tela em perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6cf73-230">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="6cf73-231">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="6cf73-231">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="6cf73-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-232">Boolean</span></span>|<span data-ttu-id="6cf73-233">Bloquear exibir ID de chamadas de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="6cf73-233">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="6cf73-234">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="6cf73-234">workProfileBlockCamera</span></span>|<span data-ttu-id="6cf73-235">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-235">Boolean</span></span>|<span data-ttu-id="6cf73-236">Bloquear câmera de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6cf73-236">Block work profile camera.</span></span>|
|<span data-ttu-id="6cf73-237">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="6cf73-237">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="6cf73-238">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-238">Boolean</span></span>|<span data-ttu-id="6cf73-239">Bloquear disponibilidade de contatos de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="6cf73-239">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="6cf73-240">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="6cf73-240">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="6cf73-241">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-241">Boolean</span></span>|<span data-ttu-id="6cf73-242">Booliano que indica se a configuração de desautorizar a cópia/colagem entre perfis está habilitada.</span><span class="sxs-lookup"><span data-stu-id="6cf73-242">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="6cf73-243">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="6cf73-243">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="6cf73-244">androidForWorkDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="6cf73-244">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="6cf73-245">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="6cf73-245">Type of password that is required.</span></span> <span data-ttu-id="6cf73-246">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="6cf73-246">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="6cf73-247">workProfilePasswordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="6cf73-247">workProfilePasswordBlockFaceUnlock</span></span>|<span data-ttu-id="6cf73-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-248">Boolean</span></span>|<span data-ttu-id="6cf73-249">Indica se o desbloqueio de face deve ou não ser bloqueado para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6cf73-249">Indicates whether or not to block face unlock for work profile.</span></span>|
|<span data-ttu-id="6cf73-250">Propriedades workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="6cf73-250">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="6cf73-251">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-251">Boolean</span></span>|<span data-ttu-id="6cf73-252">Indica se o desbloqueio de impressão digital para o perfil de trabalho deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6cf73-252">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="6cf73-253">workProfilePasswordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="6cf73-253">workProfilePasswordBlockIrisUnlock</span></span>|<span data-ttu-id="6cf73-254">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-254">Boolean</span></span>|<span data-ttu-id="6cf73-255">Indica se o desbloqueio íris para o perfil de trabalho deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6cf73-255">Indicates whether or not to block iris unlock for work profile.</span></span>|
|<span data-ttu-id="6cf73-256">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="6cf73-256">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="6cf73-257">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-257">Boolean</span></span>|<span data-ttu-id="6cf73-258">Indica se o bloqueio inteligente e outros agentes de confiança devem ou não ser bloqueados para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6cf73-258">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="6cf73-259">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6cf73-259">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="6cf73-260">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf73-260">Int32</span></span>|<span data-ttu-id="6cf73-261">Número de dias antes da senha do perfil de trabalho expirar.</span><span class="sxs-lookup"><span data-stu-id="6cf73-261">Number of days before the work profile password expires.</span></span> <span data-ttu-id="6cf73-262">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="6cf73-262">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6cf73-263">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6cf73-263">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="6cf73-264">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf73-264">Int32</span></span>|<span data-ttu-id="6cf73-265">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6cf73-265">Minimum length of work profile password.</span></span> <span data-ttu-id="6cf73-266">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="6cf73-266">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6cf73-267">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="6cf73-267">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="6cf73-268">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf73-268">Int32</span></span>|<span data-ttu-id="6cf73-269">Mínimo de caracteres numéricos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6cf73-269">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="6cf73-270">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="6cf73-270">Valid values 1 to 10</span></span>|
|<span data-ttu-id="6cf73-271">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="6cf73-271">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="6cf73-272">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf73-272">Int32</span></span>|<span data-ttu-id="6cf73-273">Número mínimo de caracteres não carta necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6cf73-273">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="6cf73-274">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="6cf73-274">Valid values 1 to 10</span></span>|
|<span data-ttu-id="6cf73-275">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="6cf73-275">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="6cf73-276">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf73-276">Int32</span></span>|<span data-ttu-id="6cf73-277">Número mínimo de caracteres de letras necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6cf73-277">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="6cf73-278">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="6cf73-278">Valid values 1 to 10</span></span>|
|<span data-ttu-id="6cf73-279">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="6cf73-279">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="6cf73-280">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf73-280">Int32</span></span>|<span data-ttu-id="6cf73-281">Número mínimo de caracteres em minúsculas exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6cf73-281">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="6cf73-282">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="6cf73-282">Valid values 1 to 10</span></span>|
|<span data-ttu-id="6cf73-283">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="6cf73-283">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="6cf73-284">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf73-284">Int32</span></span>|<span data-ttu-id="6cf73-285">Número mínimo de caracteres em maiúsculas obrigatórios na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6cf73-285">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="6cf73-286">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="6cf73-286">Valid values 1 to 10</span></span>|
|<span data-ttu-id="6cf73-287">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="6cf73-287">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="6cf73-288">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf73-288">Int32</span></span>|<span data-ttu-id="6cf73-289">Número mínimo de símbolos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6cf73-289">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="6cf73-290">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="6cf73-290">Valid values 1 to 10</span></span>|
|<span data-ttu-id="6cf73-291">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6cf73-291">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6cf73-292">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf73-292">Int32</span></span>|<span data-ttu-id="6cf73-293">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="6cf73-293">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6cf73-294">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6cf73-294">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6cf73-295">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf73-295">Int32</span></span>|<span data-ttu-id="6cf73-296">Número de senhas de perfil de trabalho anteriores a serem bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="6cf73-296">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="6cf73-297">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="6cf73-297">Valid values 0 to 24</span></span>|
|<span data-ttu-id="6cf73-298">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="6cf73-298">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="6cf73-299">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf73-299">Int32</span></span>|<span data-ttu-id="6cf73-300">Número de falhas de entrada permitidas antes que o perfil de trabalho seja removido e todos os dados corporativos excluídos.</span><span class="sxs-lookup"><span data-stu-id="6cf73-300">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="6cf73-301">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="6cf73-301">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6cf73-302">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6cf73-302">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="6cf73-303">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6cf73-303">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="6cf73-304">Tipo de senha de perfil de trabalho necessário.</span><span class="sxs-lookup"><span data-stu-id="6cf73-304">Type of work profile password that is required.</span></span> <span data-ttu-id="6cf73-305">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="6cf73-305">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="6cf73-306">Workprofilerequirepassword foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="6cf73-306">workProfileRequirePassword</span></span>|<span data-ttu-id="6cf73-307">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-307">Boolean</span></span>|<span data-ttu-id="6cf73-308">A senha é obrigatória ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="6cf73-308">Password is required or not for work profile</span></span>|
|<span data-ttu-id="6cf73-309">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="6cf73-309">securityRequireVerifyApps</span></span>|<span data-ttu-id="6cf73-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cf73-310">Boolean</span></span>|<span data-ttu-id="6cf73-311">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="6cf73-311">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="6cf73-312">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="6cf73-312">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="6cf73-313">String</span><span class="sxs-lookup"><span data-stu-id="6cf73-313">String</span></span>|<span data-ttu-id="6cf73-314">Habilitar o modo de bloqueio para VPN Always-on.</span><span class="sxs-lookup"><span data-stu-id="6cf73-314">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="6cf73-315">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="6cf73-315">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="6cf73-316">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-316">Boolean</span></span>|<span data-ttu-id="6cf73-317">Habilitar o modo de bloqueio para VPN Always-on.</span><span class="sxs-lookup"><span data-stu-id="6cf73-317">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="6cf73-318">workProfileAllowWidgets</span><span class="sxs-lookup"><span data-stu-id="6cf73-318">workProfileAllowWidgets</span></span>|<span data-ttu-id="6cf73-319">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-319">Boolean</span></span>|<span data-ttu-id="6cf73-320">Permitir widgets de aplicativos de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6cf73-320">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="6cf73-321">workProfileBlockPersonalAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="6cf73-321">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="6cf73-322">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cf73-322">Boolean</span></span>|<span data-ttu-id="6cf73-323">Impedir instalações de aplicativos de fontes desconhecidas no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="6cf73-323">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="6cf73-324">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cf73-324">Response</span></span>
<span data-ttu-id="6cf73-325">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cf73-325">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cf73-326">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cf73-326">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cf73-327">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cf73-327">Request</span></span>
<span data-ttu-id="6cf73-328">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cf73-328">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3079

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
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
  "passwordBlockFaceUnlock": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockIrisUnlock": true,
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
  "workProfilePasswordBlockFaceUnlock": true,
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockIrisUnlock": true,
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

### <a name="response"></a><span data-ttu-id="6cf73-329">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cf73-329">Response</span></span>
<span data-ttu-id="6cf73-p131">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6cf73-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3251

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "id": "a931a366-a366-a931-66a3-31a966a331a9",
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
  "passwordBlockFaceUnlock": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockIrisUnlock": true,
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
  "workProfilePasswordBlockFaceUnlock": true,
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockIrisUnlock": true,
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



