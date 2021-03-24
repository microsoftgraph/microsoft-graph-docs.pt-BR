---
title: Criar androidForWorkGeneralDeviceConfiguration
description: Crie um novo objeto androidForWorkGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3767131656c961e859bdd7316b78fecd91eeccd0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130333"
---
# <a name="create-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="e8ed3-103">Criar androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e8ed3-103">Create androidForWorkGeneralDeviceConfiguration</span></span>

<span data-ttu-id="e8ed3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8ed3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8ed3-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8ed3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8ed3-107">Crie um novo [objeto androidForWorkGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e8ed3-107">Create a new [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8ed3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8ed3-108">Prerequisites</span></span>
<span data-ttu-id="e8ed3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8ed3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8ed3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8ed3-111">Permission type</span></span>|<span data-ttu-id="e8ed3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8ed3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8ed3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8ed3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8ed3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8ed3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e8ed3-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8ed3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8ed3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-116">Not supported.</span></span>|
|<span data-ttu-id="e8ed3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8ed3-117">Application</span></span>|<span data-ttu-id="e8ed3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8ed3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8ed3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8ed3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e8ed3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8ed3-120">Request headers</span></span>
|<span data-ttu-id="e8ed3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8ed3-121">Header</span></span>|<span data-ttu-id="e8ed3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e8ed3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8ed3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8ed3-123">Authorization</span></span>|<span data-ttu-id="e8ed3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8ed3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e8ed3-125">Accept</span></span>|<span data-ttu-id="e8ed3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8ed3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8ed3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8ed3-127">Request body</span></span>
<span data-ttu-id="e8ed3-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidForWorkGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-128">In the request body, supply a JSON representation for the androidForWorkGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="e8ed3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o androidForWorkGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-129">The following table shows the properties that are required when you create the androidForWorkGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="e8ed3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8ed3-130">Property</span></span>|<span data-ttu-id="e8ed3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8ed3-131">Type</span></span>|<span data-ttu-id="e8ed3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8ed3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8ed3-133">id</span><span class="sxs-lookup"><span data-stu-id="e8ed3-133">id</span></span>|<span data-ttu-id="e8ed3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8ed3-134">String</span></span>|<span data-ttu-id="e8ed3-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-135">Key of the entity.</span></span> <span data-ttu-id="e8ed3-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e8ed3-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8ed3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8ed3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e8ed3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8ed3-138">DateTimeOffset</span></span>|<span data-ttu-id="e8ed3-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e8ed3-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e8ed3-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8ed3-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e8ed3-141">roleScopeTagIds</span></span>|<span data-ttu-id="e8ed3-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8ed3-142">String collection</span></span>|<span data-ttu-id="e8ed3-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e8ed3-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e8ed3-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8ed3-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e8ed3-145">supportsScopeTags</span></span>|<span data-ttu-id="e8ed3-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-146">Boolean</span></span>|<span data-ttu-id="e8ed3-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e8ed3-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e8ed3-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e8ed3-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-150">This property is read-only.</span></span> <span data-ttu-id="e8ed3-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e8ed3-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8ed3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e8ed3-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e8ed3-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e8ed3-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e8ed3-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e8ed3-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e8ed3-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8ed3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e8ed3-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e8ed3-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e8ed3-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e8ed3-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e8ed3-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e8ed3-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8ed3-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e8ed3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e8ed3-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e8ed3-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e8ed3-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e8ed3-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e8ed3-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8ed3-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8ed3-164">createdDateTime</span></span>|<span data-ttu-id="e8ed3-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8ed3-165">DateTimeOffset</span></span>|<span data-ttu-id="e8ed3-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-166">DateTime the object was created.</span></span> <span data-ttu-id="e8ed3-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e8ed3-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8ed3-168">descrição</span><span class="sxs-lookup"><span data-stu-id="e8ed3-168">description</span></span>|<span data-ttu-id="e8ed3-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8ed3-169">String</span></span>|<span data-ttu-id="e8ed3-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e8ed3-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e8ed3-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8ed3-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e8ed3-172">displayName</span></span>|<span data-ttu-id="e8ed3-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8ed3-173">String</span></span>|<span data-ttu-id="e8ed3-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e8ed3-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e8ed3-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8ed3-176">versão</span><span class="sxs-lookup"><span data-stu-id="e8ed3-176">version</span></span>|<span data-ttu-id="e8ed3-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e8ed3-177">Int32</span></span>|<span data-ttu-id="e8ed3-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-178">Version of the device configuration.</span></span> <span data-ttu-id="e8ed3-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e8ed3-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8ed3-180">passwordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="e8ed3-180">passwordBlockFaceUnlock</span></span>|<span data-ttu-id="e8ed3-181">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-181">Boolean</span></span>|<span data-ttu-id="e8ed3-182">Indica se o desbloqueio facial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-182">Indicates whether or not to block face unlock.</span></span>|
|<span data-ttu-id="e8ed3-183">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="e8ed3-183">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="e8ed3-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8ed3-184">Boolean</span></span>|<span data-ttu-id="e8ed3-185">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-185">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="e8ed3-186">passwordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="e8ed3-186">passwordBlockIrisUnlock</span></span>|<span data-ttu-id="e8ed3-187">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-187">Boolean</span></span>|<span data-ttu-id="e8ed3-188">Indica se o desbloqueio de íris deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-188">Indicates whether or not to block iris unlock.</span></span>|
|<span data-ttu-id="e8ed3-189">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="e8ed3-189">passwordBlockTrustAgents</span></span>|<span data-ttu-id="e8ed3-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8ed3-190">Boolean</span></span>|<span data-ttu-id="e8ed3-191">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-191">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="e8ed3-192">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e8ed3-192">passwordExpirationDays</span></span>|<span data-ttu-id="e8ed3-193">Int32</span><span class="sxs-lookup"><span data-stu-id="e8ed3-193">Int32</span></span>|<span data-ttu-id="e8ed3-194">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-194">Number of days before the password expires.</span></span> <span data-ttu-id="e8ed3-195">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="e8ed3-195">Valid values 1 to 365</span></span>|
|<span data-ttu-id="e8ed3-196">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e8ed3-196">passwordMinimumLength</span></span>|<span data-ttu-id="e8ed3-197">Int32</span><span class="sxs-lookup"><span data-stu-id="e8ed3-197">Int32</span></span>|<span data-ttu-id="e8ed3-198">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-198">Minimum length of passwords.</span></span> <span data-ttu-id="e8ed3-199">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="e8ed3-199">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e8ed3-200">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e8ed3-200">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e8ed3-201">Int32</span><span class="sxs-lookup"><span data-stu-id="e8ed3-201">Int32</span></span>|<span data-ttu-id="e8ed3-202">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-202">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e8ed3-203">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e8ed3-203">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e8ed3-204">Int32</span><span class="sxs-lookup"><span data-stu-id="e8ed3-204">Int32</span></span>|<span data-ttu-id="e8ed3-205">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-205">Number of previous passwords to block.</span></span> <span data-ttu-id="e8ed3-206">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="e8ed3-206">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e8ed3-207">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e8ed3-207">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e8ed3-208">Int32</span><span class="sxs-lookup"><span data-stu-id="e8ed3-208">Int32</span></span>|<span data-ttu-id="e8ed3-209">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-209">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="e8ed3-210">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="e8ed3-210">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e8ed3-211">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e8ed3-211">passwordRequiredType</span></span>|[<span data-ttu-id="e8ed3-212">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e8ed3-212">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="e8ed3-213">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-213">Type of password that is required.</span></span> <span data-ttu-id="e8ed3-214">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-214">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="e8ed3-215">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="e8ed3-215">workProfileDataSharingType</span></span>|[<span data-ttu-id="e8ed3-216">androidForWorkCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="e8ed3-216">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="e8ed3-217">Tipo de compartilhamento de dados permitido.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-217">Type of data sharing that is allowed.</span></span> <span data-ttu-id="e8ed3-218">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-218">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="e8ed3-219">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="e8ed3-219">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="e8ed3-220">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-220">Boolean</span></span>|<span data-ttu-id="e8ed3-221">Indica se as notificações são bloqueadas ou não enquanto o dispositivo está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-221">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="e8ed3-222">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="e8ed3-222">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="e8ed3-223">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-223">Boolean</span></span>|<span data-ttu-id="e8ed3-224">Impedir que os usuários adicionem/removam contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-224">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="e8ed3-225">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="e8ed3-225">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="e8ed3-226">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-226">Boolean</span></span>|<span data-ttu-id="e8ed3-227">Permitir que dispositivos bluetooth acessem contatos corporativos.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-227">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="e8ed3-228">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="e8ed3-228">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="e8ed3-229">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-229">Boolean</span></span>|<span data-ttu-id="e8ed3-230">Bloquear captura de tela no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-230">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="e8ed3-231">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="e8ed3-231">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="e8ed3-232">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-232">Boolean</span></span>|<span data-ttu-id="e8ed3-233">Bloqueie a ID do chamador de perfil de trabalho de exibição no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-233">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="e8ed3-234">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="e8ed3-234">workProfileBlockCamera</span></span>|<span data-ttu-id="e8ed3-235">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-235">Boolean</span></span>|<span data-ttu-id="e8ed3-236">Bloquear a câmera de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-236">Block work profile camera.</span></span>|
|<span data-ttu-id="e8ed3-237">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="e8ed3-237">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="e8ed3-238">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-238">Boolean</span></span>|<span data-ttu-id="e8ed3-239">Bloquear a disponibilidade de contatos de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-239">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="e8ed3-240">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="e8ed3-240">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="e8ed3-241">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-241">Boolean</span></span>|<span data-ttu-id="e8ed3-242">Boolean que indica se a configuração não permitir cópia/colar entre perfis está habilitada.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-242">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="e8ed3-243">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="e8ed3-243">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="e8ed3-244">androidForWorkDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="e8ed3-244">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="e8ed3-245">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-245">Type of password that is required.</span></span> <span data-ttu-id="e8ed3-246">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-246">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="e8ed3-247">workProfilePasswordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="e8ed3-247">workProfilePasswordBlockFaceUnlock</span></span>|<span data-ttu-id="e8ed3-248">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-248">Boolean</span></span>|<span data-ttu-id="e8ed3-249">Indica se o desbloqueio facial deve ou não ser bloqueado para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-249">Indicates whether or not to block face unlock for work profile.</span></span>|
|<span data-ttu-id="e8ed3-250">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="e8ed3-250">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="e8ed3-251">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-251">Boolean</span></span>|<span data-ttu-id="e8ed3-252">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-252">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="e8ed3-253">workProfilePasswordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="e8ed3-253">workProfilePasswordBlockIrisUnlock</span></span>|<span data-ttu-id="e8ed3-254">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-254">Boolean</span></span>|<span data-ttu-id="e8ed3-255">Indica se o desbloqueio de íris deve ou não ser bloqueado para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-255">Indicates whether or not to block iris unlock for work profile.</span></span>|
|<span data-ttu-id="e8ed3-256">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="e8ed3-256">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="e8ed3-257">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-257">Boolean</span></span>|<span data-ttu-id="e8ed3-258">Indica se o Smart Lock deve ou não ser bloqueado e outros agentes de confiança para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-258">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="e8ed3-259">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e8ed3-259">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="e8ed3-260">Int32</span><span class="sxs-lookup"><span data-stu-id="e8ed3-260">Int32</span></span>|<span data-ttu-id="e8ed3-261">Número de dias antes que a senha do perfil de trabalho expire.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-261">Number of days before the work profile password expires.</span></span> <span data-ttu-id="e8ed3-262">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="e8ed3-262">Valid values 1 to 365</span></span>|
|<span data-ttu-id="e8ed3-263">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e8ed3-263">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="e8ed3-264">Int32</span><span class="sxs-lookup"><span data-stu-id="e8ed3-264">Int32</span></span>|<span data-ttu-id="e8ed3-265">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-265">Minimum length of work profile password.</span></span> <span data-ttu-id="e8ed3-266">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="e8ed3-266">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e8ed3-267">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="e8ed3-267">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="e8ed3-268">Int32</span><span class="sxs-lookup"><span data-stu-id="e8ed3-268">Int32</span></span>|<span data-ttu-id="e8ed3-269">Mínimo # de caracteres numéricos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-269">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="e8ed3-270">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="e8ed3-270">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e8ed3-271">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="e8ed3-271">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="e8ed3-272">Int32</span><span class="sxs-lookup"><span data-stu-id="e8ed3-272">Int32</span></span>|<span data-ttu-id="e8ed3-273">Mínimo # de caracteres que não são letras exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-273">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="e8ed3-274">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="e8ed3-274">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e8ed3-275">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="e8ed3-275">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="e8ed3-276">Int32</span><span class="sxs-lookup"><span data-stu-id="e8ed3-276">Int32</span></span>|<span data-ttu-id="e8ed3-277">Mínimo # de caracteres de letra necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-277">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="e8ed3-278">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="e8ed3-278">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e8ed3-279">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="e8ed3-279">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="e8ed3-280">Int32</span><span class="sxs-lookup"><span data-stu-id="e8ed3-280">Int32</span></span>|<span data-ttu-id="e8ed3-281">Mínimo # de caracteres de menor ocorrência exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-281">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="e8ed3-282">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="e8ed3-282">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e8ed3-283">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="e8ed3-283">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="e8ed3-284">Int32</span><span class="sxs-lookup"><span data-stu-id="e8ed3-284">Int32</span></span>|<span data-ttu-id="e8ed3-285">Mínimo # de caracteres de maiúsculas e médias exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-285">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="e8ed3-286">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="e8ed3-286">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e8ed3-287">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="e8ed3-287">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="e8ed3-288">Int32</span><span class="sxs-lookup"><span data-stu-id="e8ed3-288">Int32</span></span>|<span data-ttu-id="e8ed3-289">Mínimo # de símbolos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-289">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="e8ed3-290">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="e8ed3-290">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e8ed3-291">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e8ed3-291">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e8ed3-292">Int32</span><span class="sxs-lookup"><span data-stu-id="e8ed3-292">Int32</span></span>|<span data-ttu-id="e8ed3-293">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-293">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e8ed3-294">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e8ed3-294">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e8ed3-295">Int32</span><span class="sxs-lookup"><span data-stu-id="e8ed3-295">Int32</span></span>|<span data-ttu-id="e8ed3-296">Número de senhas de perfil de trabalho anteriores a bloquear.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-296">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="e8ed3-297">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="e8ed3-297">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e8ed3-298">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e8ed3-298">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e8ed3-299">Int32</span><span class="sxs-lookup"><span data-stu-id="e8ed3-299">Int32</span></span>|<span data-ttu-id="e8ed3-300">Número de falhas de entrada permitidas antes que o perfil de trabalho seja removido e todos os dados corporativos excluídos.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-300">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="e8ed3-301">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="e8ed3-301">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e8ed3-302">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e8ed3-302">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="e8ed3-303">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e8ed3-303">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="e8ed3-304">Tipo de senha de perfil de trabalho necessária.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-304">Type of work profile password that is required.</span></span> <span data-ttu-id="e8ed3-305">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-305">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="e8ed3-306">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="e8ed3-306">workProfileRequirePassword</span></span>|<span data-ttu-id="e8ed3-307">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-307">Boolean</span></span>|<span data-ttu-id="e8ed3-308">A senha é necessária ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="e8ed3-308">Password is required or not for work profile</span></span>|
|<span data-ttu-id="e8ed3-309">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="e8ed3-309">securityRequireVerifyApps</span></span>|<span data-ttu-id="e8ed3-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8ed3-310">Boolean</span></span>|<span data-ttu-id="e8ed3-311">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-311">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="e8ed3-312">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="e8ed3-312">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="e8ed3-313">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8ed3-313">String</span></span>|<span data-ttu-id="e8ed3-314">Habilitar o modo de bloqueio para VPN always-on.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-314">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="e8ed3-315">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="e8ed3-315">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="e8ed3-316">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-316">Boolean</span></span>|<span data-ttu-id="e8ed3-317">Habilitar o modo de bloqueio para VPN always-on.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-317">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="e8ed3-318">workProfileAllowWidgets</span><span class="sxs-lookup"><span data-stu-id="e8ed3-318">workProfileAllowWidgets</span></span>|<span data-ttu-id="e8ed3-319">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-319">Boolean</span></span>|<span data-ttu-id="e8ed3-320">Permitir widgets de aplicativos de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-320">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="e8ed3-321">workProfileBlockPersonalAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="e8ed3-321">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="e8ed3-322">Booleano</span><span class="sxs-lookup"><span data-stu-id="e8ed3-322">Boolean</span></span>|<span data-ttu-id="e8ed3-323">Impedir instalações de aplicativos de fontes desconhecidas no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-323">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="e8ed3-324">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8ed3-324">Response</span></span>
<span data-ttu-id="e8ed3-325">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-325">If successful, this method returns a `201 Created` response code and a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8ed3-326">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8ed3-326">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8ed3-327">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8ed3-327">Request</span></span>
<span data-ttu-id="e8ed3-328">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-328">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="e8ed3-329">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8ed3-329">Response</span></span>
<span data-ttu-id="e8ed3-p131">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8ed3-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




