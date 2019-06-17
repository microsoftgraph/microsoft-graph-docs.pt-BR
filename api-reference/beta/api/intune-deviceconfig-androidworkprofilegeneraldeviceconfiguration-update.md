---
title: Atualizar Entidadeandroidforworkprofiledeviceconfiguration
description: Atualiza as propriedades de um objeto Entidadeandroidforworkprofiledeviceconfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 77ee919ad334cf176b59dd09105398148978ceb6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34969355"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="2f0f0-103">Atualizar Entidadeandroidforworkprofiledeviceconfiguration</span><span class="sxs-lookup"><span data-stu-id="2f0f0-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="2f0f0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f0f0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f0f0-106">Atualiza as propriedades de um objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2f0f0-106">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f0f0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f0f0-107">Prerequisites</span></span>
<span data-ttu-id="2f0f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f0f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f0f0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f0f0-110">Permission type</span></span>|<span data-ttu-id="2f0f0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f0f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f0f0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f0f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f0f0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f0f0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f0f0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f0f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f0f0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-115">Not supported.</span></span>|
|<span data-ttu-id="2f0f0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f0f0-116">Application</span></span>|<span data-ttu-id="2f0f0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f0f0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f0f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2f0f0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f0f0-119">Request headers</span></span>
|<span data-ttu-id="2f0f0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f0f0-120">Header</span></span>|<span data-ttu-id="2f0f0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2f0f0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f0f0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f0f0-122">Authorization</span></span>|<span data-ttu-id="2f0f0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f0f0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f0f0-124">Accept</span></span>|<span data-ttu-id="2f0f0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f0f0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f0f0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f0f0-126">Request body</span></span>
<span data-ttu-id="2f0f0-127">No corpo da solicitação, forneça uma representação JSON do objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2f0f0-127">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="2f0f0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f0f0-128">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="2f0f0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f0f0-129">Property</span></span>|<span data-ttu-id="2f0f0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f0f0-130">Type</span></span>|<span data-ttu-id="2f0f0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f0f0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f0f0-132">id</span><span class="sxs-lookup"><span data-stu-id="2f0f0-132">id</span></span>|<span data-ttu-id="2f0f0-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f0f0-133">String</span></span>|<span data-ttu-id="2f0f0-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-134">Key of the entity.</span></span> <span data-ttu-id="2f0f0-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f0f0-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f0f0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f0f0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2f0f0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f0f0-137">DateTimeOffset</span></span>|<span data-ttu-id="2f0f0-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2f0f0-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f0f0-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f0f0-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2f0f0-140">roleScopeTagIds</span></span>|<span data-ttu-id="2f0f0-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f0f0-141">String collection</span></span>|<span data-ttu-id="2f0f0-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2f0f0-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f0f0-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f0f0-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2f0f0-144">supportsScopeTags</span></span>|<span data-ttu-id="2f0f0-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f0f0-145">Boolean</span></span>|<span data-ttu-id="2f0f0-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2f0f0-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2f0f0-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2f0f0-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-149">This property is read-only.</span></span> <span data-ttu-id="2f0f0-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f0f0-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f0f0-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2f0f0-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2f0f0-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2f0f0-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2f0f0-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2f0f0-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f0f0-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f0f0-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2f0f0-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2f0f0-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2f0f0-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2f0f0-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2f0f0-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f0f0-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f0f0-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2f0f0-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2f0f0-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2f0f0-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2f0f0-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2f0f0-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f0f0-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f0f0-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f0f0-163">createdDateTime</span></span>|<span data-ttu-id="2f0f0-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f0f0-164">DateTimeOffset</span></span>|<span data-ttu-id="2f0f0-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-165">DateTime the object was created.</span></span> <span data-ttu-id="2f0f0-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f0f0-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f0f0-167">descrição</span><span class="sxs-lookup"><span data-stu-id="2f0f0-167">description</span></span>|<span data-ttu-id="2f0f0-168">String</span><span class="sxs-lookup"><span data-stu-id="2f0f0-168">String</span></span>|<span data-ttu-id="2f0f0-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2f0f0-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f0f0-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f0f0-171">displayName</span><span class="sxs-lookup"><span data-stu-id="2f0f0-171">displayName</span></span>|<span data-ttu-id="2f0f0-172">String</span><span class="sxs-lookup"><span data-stu-id="2f0f0-172">String</span></span>|<span data-ttu-id="2f0f0-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2f0f0-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f0f0-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f0f0-175">versão</span><span class="sxs-lookup"><span data-stu-id="2f0f0-175">version</span></span>|<span data-ttu-id="2f0f0-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2f0f0-176">Int32</span></span>|<span data-ttu-id="2f0f0-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-177">Version of the device configuration.</span></span> <span data-ttu-id="2f0f0-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f0f0-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f0f0-179">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="2f0f0-179">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="2f0f0-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f0f0-180">Boolean</span></span>|<span data-ttu-id="2f0f0-181">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-181">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="2f0f0-182">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="2f0f0-182">passwordBlockTrustAgents</span></span>|<span data-ttu-id="2f0f0-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f0f0-183">Boolean</span></span>|<span data-ttu-id="2f0f0-184">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-184">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="2f0f0-185">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2f0f0-185">passwordExpirationDays</span></span>|<span data-ttu-id="2f0f0-186">Int32</span><span class="sxs-lookup"><span data-stu-id="2f0f0-186">Int32</span></span>|<span data-ttu-id="2f0f0-187">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-187">Number of days before the password expires.</span></span> <span data-ttu-id="2f0f0-188">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="2f0f0-188">Valid values 1 to 365</span></span>|
|<span data-ttu-id="2f0f0-189">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2f0f0-189">passwordMinimumLength</span></span>|<span data-ttu-id="2f0f0-190">Int32</span><span class="sxs-lookup"><span data-stu-id="2f0f0-190">Int32</span></span>|<span data-ttu-id="2f0f0-191">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-191">Minimum length of passwords.</span></span> <span data-ttu-id="2f0f0-192">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="2f0f0-192">Valid values 4 to 16</span></span>|
|<span data-ttu-id="2f0f0-193">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="2f0f0-193">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="2f0f0-194">Int32</span><span class="sxs-lookup"><span data-stu-id="2f0f0-194">Int32</span></span>|<span data-ttu-id="2f0f0-195">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-195">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="2f0f0-196">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2f0f0-196">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2f0f0-197">Int32</span><span class="sxs-lookup"><span data-stu-id="2f0f0-197">Int32</span></span>|<span data-ttu-id="2f0f0-198">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-198">Number of previous passwords to block.</span></span> <span data-ttu-id="2f0f0-199">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="2f0f0-199">Valid values 0 to 24</span></span>|
|<span data-ttu-id="2f0f0-200">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="2f0f0-200">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="2f0f0-201">Int32</span><span class="sxs-lookup"><span data-stu-id="2f0f0-201">Int32</span></span>|<span data-ttu-id="2f0f0-202">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-202">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="2f0f0-203">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="2f0f0-203">Valid values 1 to 16</span></span>|
|<span data-ttu-id="2f0f0-204">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2f0f0-204">passwordRequiredType</span></span>|[<span data-ttu-id="2f0f0-205">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2f0f0-205">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="2f0f0-206">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-206">Type of password that is required.</span></span> <span data-ttu-id="2f0f0-207">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-207">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="2f0f0-208">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="2f0f0-208">workProfileDataSharingType</span></span>|[<span data-ttu-id="2f0f0-209">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="2f0f0-209">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="2f0f0-210">Tipo de compartilhamento de dados permitido.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-210">Type of data sharing that is allowed.</span></span> <span data-ttu-id="2f0f0-211">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-211">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="2f0f0-212">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="2f0f0-212">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="2f0f0-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f0f0-213">Boolean</span></span>|<span data-ttu-id="2f0f0-214">Indica se as notificações devem ou não ser bloqueadas enquanto o dispositivo estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-214">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="2f0f0-215">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="2f0f0-215">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="2f0f0-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f0f0-216">Boolean</span></span>|<span data-ttu-id="2f0f0-217">Impedir que os usuários adicionem/removam contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-217">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="2f0f0-218">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="2f0f0-218">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="2f0f0-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f0f0-219">Boolean</span></span>|<span data-ttu-id="2f0f0-220">Permitir que dispositivos Bluetooth acessem contatos da empresa.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-220">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="2f0f0-221">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="2f0f0-221">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="2f0f0-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f0f0-222">Boolean</span></span>|<span data-ttu-id="2f0f0-223">Bloquear captura de tela em perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-223">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="2f0f0-224">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="2f0f0-224">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="2f0f0-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f0f0-225">Boolean</span></span>|<span data-ttu-id="2f0f0-226">Bloquear exibir ID de chamadas de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-226">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="2f0f0-227">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="2f0f0-227">workProfileBlockCamera</span></span>|<span data-ttu-id="2f0f0-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f0f0-228">Boolean</span></span>|<span data-ttu-id="2f0f0-229">Bloquear câmera de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-229">Block work profile camera.</span></span>|
|<span data-ttu-id="2f0f0-230">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="2f0f0-230">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="2f0f0-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f0f0-231">Boolean</span></span>|<span data-ttu-id="2f0f0-232">Bloquear disponibilidade de contatos de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-232">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="2f0f0-233">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="2f0f0-233">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="2f0f0-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f0f0-234">Boolean</span></span>|<span data-ttu-id="2f0f0-235">Booliano que indica se a configuração de desautorizar a cópia/colagem entre perfis está habilitada.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-235">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="2f0f0-236">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="2f0f0-236">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="2f0f0-237">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="2f0f0-237">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="2f0f0-238">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-238">Type of password that is required.</span></span> <span data-ttu-id="2f0f0-239">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-239">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="2f0f0-240">Propriedades workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="2f0f0-240">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="2f0f0-241">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f0f0-241">Boolean</span></span>|<span data-ttu-id="2f0f0-242">Indica se o desbloqueio de impressão digital para o perfil de trabalho deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-242">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="2f0f0-243">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="2f0f0-243">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="2f0f0-244">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f0f0-244">Boolean</span></span>|<span data-ttu-id="2f0f0-245">Indica se o bloqueio inteligente e outros agentes de confiança devem ou não ser bloqueados para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-245">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="2f0f0-246">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2f0f0-246">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="2f0f0-247">Int32</span><span class="sxs-lookup"><span data-stu-id="2f0f0-247">Int32</span></span>|<span data-ttu-id="2f0f0-248">Número de dias antes da senha do perfil de trabalho expirar.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-248">Number of days before the work profile password expires.</span></span> <span data-ttu-id="2f0f0-249">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="2f0f0-249">Valid values 1 to 365</span></span>|
|<span data-ttu-id="2f0f0-250">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2f0f0-250">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="2f0f0-251">Int32</span><span class="sxs-lookup"><span data-stu-id="2f0f0-251">Int32</span></span>|<span data-ttu-id="2f0f0-252">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-252">Minimum length of work profile password.</span></span> <span data-ttu-id="2f0f0-253">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="2f0f0-253">Valid values 4 to 16</span></span>|
|<span data-ttu-id="2f0f0-254">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="2f0f0-254">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="2f0f0-255">Int32</span><span class="sxs-lookup"><span data-stu-id="2f0f0-255">Int32</span></span>|<span data-ttu-id="2f0f0-256">Mínimo de caracteres numéricos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-256">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="2f0f0-257">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="2f0f0-257">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2f0f0-258">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="2f0f0-258">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="2f0f0-259">Int32</span><span class="sxs-lookup"><span data-stu-id="2f0f0-259">Int32</span></span>|<span data-ttu-id="2f0f0-260">Número mínimo de caracteres não carta necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-260">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="2f0f0-261">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="2f0f0-261">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2f0f0-262">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="2f0f0-262">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="2f0f0-263">Int32</span><span class="sxs-lookup"><span data-stu-id="2f0f0-263">Int32</span></span>|<span data-ttu-id="2f0f0-264">Número mínimo de caracteres de letras necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-264">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="2f0f0-265">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="2f0f0-265">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2f0f0-266">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="2f0f0-266">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="2f0f0-267">Int32</span><span class="sxs-lookup"><span data-stu-id="2f0f0-267">Int32</span></span>|<span data-ttu-id="2f0f0-268">Número mínimo de caracteres em minúsculas exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-268">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="2f0f0-269">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="2f0f0-269">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2f0f0-270">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="2f0f0-270">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="2f0f0-271">Int32</span><span class="sxs-lookup"><span data-stu-id="2f0f0-271">Int32</span></span>|<span data-ttu-id="2f0f0-272">Número mínimo de caracteres em maiúsculas obrigatórios na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-272">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="2f0f0-273">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="2f0f0-273">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2f0f0-274">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="2f0f0-274">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="2f0f0-275">Int32</span><span class="sxs-lookup"><span data-stu-id="2f0f0-275">Int32</span></span>|<span data-ttu-id="2f0f0-276">Número mínimo de símbolos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-276">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="2f0f0-277">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="2f0f0-277">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2f0f0-278">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="2f0f0-278">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="2f0f0-279">Int32</span><span class="sxs-lookup"><span data-stu-id="2f0f0-279">Int32</span></span>|<span data-ttu-id="2f0f0-280">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-280">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="2f0f0-281">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2f0f0-281">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2f0f0-282">Int32</span><span class="sxs-lookup"><span data-stu-id="2f0f0-282">Int32</span></span>|<span data-ttu-id="2f0f0-283">Número de senhas de perfil de trabalho anteriores a serem bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-283">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="2f0f0-284">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="2f0f0-284">Valid values 0 to 24</span></span>|
|<span data-ttu-id="2f0f0-285">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="2f0f0-285">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="2f0f0-286">Int32</span><span class="sxs-lookup"><span data-stu-id="2f0f0-286">Int32</span></span>|<span data-ttu-id="2f0f0-287">Número de falhas de entrada permitidas antes que o perfil de trabalho seja removido e todos os dados corporativos excluídos.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-287">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="2f0f0-288">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="2f0f0-288">Valid values 1 to 16</span></span>|
|<span data-ttu-id="2f0f0-289">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2f0f0-289">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="2f0f0-290">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2f0f0-290">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="2f0f0-291">Tipo de senha de perfil de trabalho necessário.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-291">Type of work profile password that is required.</span></span> <span data-ttu-id="2f0f0-292">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-292">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="2f0f0-293">Workprofilerequirepassword foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="2f0f0-293">workProfileRequirePassword</span></span>|<span data-ttu-id="2f0f0-294">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f0f0-294">Boolean</span></span>|<span data-ttu-id="2f0f0-295">A senha é obrigatória ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="2f0f0-295">Password is required or not for work profile</span></span>|
|<span data-ttu-id="2f0f0-296">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="2f0f0-296">securityRequireVerifyApps</span></span>|<span data-ttu-id="2f0f0-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f0f0-297">Boolean</span></span>|<span data-ttu-id="2f0f0-298">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-298">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="2f0f0-299">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="2f0f0-299">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="2f0f0-300">String</span><span class="sxs-lookup"><span data-stu-id="2f0f0-300">String</span></span>|<span data-ttu-id="2f0f0-301">Habilitar o modo de bloqueio para VPN Always-on.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-301">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="2f0f0-302">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="2f0f0-302">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="2f0f0-303">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f0f0-303">Boolean</span></span>|<span data-ttu-id="2f0f0-304">Habilitar o modo de bloqueio para VPN Always-on.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-304">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="2f0f0-305">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f0f0-305">Response</span></span>
<span data-ttu-id="2f0f0-306">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-306">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f0f0-307">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f0f0-307">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f0f0-308">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f0f0-308">Request</span></span>
<span data-ttu-id="2f0f0-309">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-309">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="2f0f0-310">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f0f0-310">Response</span></span>
<span data-ttu-id="2f0f0-p131">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





