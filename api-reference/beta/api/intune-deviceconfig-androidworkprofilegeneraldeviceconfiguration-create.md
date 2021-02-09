---
title: Criar androidWorkProfileGeneralDeviceConfiguration
description: Crie um novo objeto androidWorkProfileGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 914f95106f8962304bf180a22edcae26300ad093
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155213"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="6ff7a-103">Criar androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="6ff7a-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="6ff7a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ff7a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ff7a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ff7a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ff7a-107">Crie um novo [objeto androidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ff7a-107">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ff7a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6ff7a-108">Prerequisites</span></span>
<span data-ttu-id="6ff7a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ff7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ff7a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ff7a-111">Permission type</span></span>|<span data-ttu-id="6ff7a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6ff7a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ff7a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ff7a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ff7a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ff7a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ff7a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ff7a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ff7a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-116">Not supported.</span></span>|
|<span data-ttu-id="6ff7a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ff7a-117">Application</span></span>|<span data-ttu-id="6ff7a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ff7a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ff7a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ff7a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6ff7a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ff7a-120">Request headers</span></span>
|<span data-ttu-id="6ff7a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6ff7a-121">Header</span></span>|<span data-ttu-id="6ff7a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6ff7a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ff7a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ff7a-123">Authorization</span></span>|<span data-ttu-id="6ff7a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ff7a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6ff7a-125">Accept</span></span>|<span data-ttu-id="6ff7a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ff7a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ff7a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ff7a-127">Request body</span></span>
<span data-ttu-id="6ff7a-128">No corpo da solicitação, fornece uma representação JSON do objeto androidWorkProfileGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-128">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="6ff7a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidWorkProfileGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-129">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="6ff7a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ff7a-130">Property</span></span>|<span data-ttu-id="6ff7a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ff7a-131">Type</span></span>|<span data-ttu-id="6ff7a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ff7a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ff7a-133">id</span><span class="sxs-lookup"><span data-stu-id="6ff7a-133">id</span></span>|<span data-ttu-id="6ff7a-134">String</span><span class="sxs-lookup"><span data-stu-id="6ff7a-134">String</span></span>|<span data-ttu-id="6ff7a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-135">Key of the entity.</span></span> <span data-ttu-id="6ff7a-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ff7a-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ff7a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ff7a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6ff7a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ff7a-138">DateTimeOffset</span></span>|<span data-ttu-id="6ff7a-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6ff7a-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ff7a-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ff7a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6ff7a-141">roleScopeTagIds</span></span>|<span data-ttu-id="6ff7a-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ff7a-142">String collection</span></span>|<span data-ttu-id="6ff7a-143">Lista de Marcas de Escopo para esta instância de Entidade.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6ff7a-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ff7a-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ff7a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6ff7a-145">supportsScopeTags</span></span>|<span data-ttu-id="6ff7a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-146">Boolean</span></span>|<span data-ttu-id="6ff7a-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6ff7a-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6ff7a-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvida excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6ff7a-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-150">This property is read-only.</span></span> <span data-ttu-id="6ff7a-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ff7a-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ff7a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6ff7a-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6ff7a-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6ff7a-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6ff7a-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6ff7a-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ff7a-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ff7a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6ff7a-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6ff7a-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6ff7a-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6ff7a-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6ff7a-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ff7a-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ff7a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6ff7a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6ff7a-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6ff7a-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6ff7a-162">A regra de aplicabilidade do modo de dispositivo para esta política.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6ff7a-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ff7a-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ff7a-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ff7a-164">createdDateTime</span></span>|<span data-ttu-id="6ff7a-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ff7a-165">DateTimeOffset</span></span>|<span data-ttu-id="6ff7a-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-166">DateTime the object was created.</span></span> <span data-ttu-id="6ff7a-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ff7a-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ff7a-168">description</span><span class="sxs-lookup"><span data-stu-id="6ff7a-168">description</span></span>|<span data-ttu-id="6ff7a-169">String</span><span class="sxs-lookup"><span data-stu-id="6ff7a-169">String</span></span>|<span data-ttu-id="6ff7a-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6ff7a-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ff7a-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ff7a-172">displayName</span><span class="sxs-lookup"><span data-stu-id="6ff7a-172">displayName</span></span>|<span data-ttu-id="6ff7a-173">String</span><span class="sxs-lookup"><span data-stu-id="6ff7a-173">String</span></span>|<span data-ttu-id="6ff7a-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6ff7a-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ff7a-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ff7a-176">versão</span><span class="sxs-lookup"><span data-stu-id="6ff7a-176">version</span></span>|<span data-ttu-id="6ff7a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff7a-177">Int32</span></span>|<span data-ttu-id="6ff7a-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-178">Version of the device configuration.</span></span> <span data-ttu-id="6ff7a-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ff7a-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ff7a-180">passwordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="6ff7a-180">passwordBlockFaceUnlock</span></span>|<span data-ttu-id="6ff7a-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-181">Boolean</span></span>|<span data-ttu-id="6ff7a-182">Indica se o desbloqueio facial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-182">Indicates whether or not to block face unlock.</span></span>|
|<span data-ttu-id="6ff7a-183">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="6ff7a-183">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="6ff7a-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-184">Boolean</span></span>|<span data-ttu-id="6ff7a-185">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-185">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="6ff7a-186">passwordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="6ff7a-186">passwordBlockIrisUnlock</span></span>|<span data-ttu-id="6ff7a-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-187">Boolean</span></span>|<span data-ttu-id="6ff7a-188">Indica se o desbloqueio da íris deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-188">Indicates whether or not to block iris unlock.</span></span>|
|<span data-ttu-id="6ff7a-189">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="6ff7a-189">passwordBlockTrustAgents</span></span>|<span data-ttu-id="6ff7a-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-190">Boolean</span></span>|<span data-ttu-id="6ff7a-191">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-191">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="6ff7a-192">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6ff7a-192">passwordExpirationDays</span></span>|<span data-ttu-id="6ff7a-193">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff7a-193">Int32</span></span>|<span data-ttu-id="6ff7a-194">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-194">Number of days before the password expires.</span></span> <span data-ttu-id="6ff7a-195">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="6ff7a-195">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6ff7a-196">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6ff7a-196">passwordMinimumLength</span></span>|<span data-ttu-id="6ff7a-197">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff7a-197">Int32</span></span>|<span data-ttu-id="6ff7a-198">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-198">Minimum length of passwords.</span></span> <span data-ttu-id="6ff7a-199">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="6ff7a-199">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6ff7a-200">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6ff7a-200">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6ff7a-201">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff7a-201">Int32</span></span>|<span data-ttu-id="6ff7a-202">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-202">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6ff7a-203">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6ff7a-203">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6ff7a-204">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff7a-204">Int32</span></span>|<span data-ttu-id="6ff7a-205">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-205">Number of previous passwords to block.</span></span> <span data-ttu-id="6ff7a-206">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="6ff7a-206">Valid values 0 to 24</span></span>|
|<span data-ttu-id="6ff7a-207">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="6ff7a-207">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="6ff7a-208">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff7a-208">Int32</span></span>|<span data-ttu-id="6ff7a-209">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-209">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="6ff7a-210">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="6ff7a-210">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6ff7a-211">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6ff7a-211">passwordRequiredType</span></span>|[<span data-ttu-id="6ff7a-212">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6ff7a-212">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="6ff7a-213">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-213">Type of password that is required.</span></span> <span data-ttu-id="6ff7a-214">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-214">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="6ff7a-215">workProfileAllowAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="6ff7a-215">workProfileAllowAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="6ff7a-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-216">Boolean</span></span>|<span data-ttu-id="6ff7a-217">Indica se é para permitir a instalação de aplicativos de fontes desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-217">Indicates whether to allow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="6ff7a-218">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="6ff7a-218">workProfileDataSharingType</span></span>|[<span data-ttu-id="6ff7a-219">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="6ff7a-219">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="6ff7a-220">Tipo de compartilhamento de dados permitido.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-220">Type of data sharing that is allowed.</span></span> <span data-ttu-id="6ff7a-221">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-221">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="6ff7a-222">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="6ff7a-222">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="6ff7a-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-223">Boolean</span></span>|<span data-ttu-id="6ff7a-224">Indica se as notificações de bloqueio são ou não durante o bloqueio do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-224">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="6ff7a-225">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="6ff7a-225">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="6ff7a-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-226">Boolean</span></span>|<span data-ttu-id="6ff7a-227">Impedir que os usuários adicionem/removam contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-227">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="6ff7a-228">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="6ff7a-228">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="6ff7a-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-229">Boolean</span></span>|<span data-ttu-id="6ff7a-230">Permitir que dispositivos bluetooth acessem contatos corporativos.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-230">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="6ff7a-231">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="6ff7a-231">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="6ff7a-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-232">Boolean</span></span>|<span data-ttu-id="6ff7a-233">Bloquear captura de tela no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-233">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="6ff7a-234">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="6ff7a-234">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="6ff7a-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-235">Boolean</span></span>|<span data-ttu-id="6ff7a-236">Bloquear a ID de chamada do perfil de trabalho de exibição no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-236">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="6ff7a-237">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="6ff7a-237">workProfileBlockCamera</span></span>|<span data-ttu-id="6ff7a-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-238">Boolean</span></span>|<span data-ttu-id="6ff7a-239">Bloquear câmera de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-239">Block work profile camera.</span></span>|
|<span data-ttu-id="6ff7a-240">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="6ff7a-240">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="6ff7a-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-241">Boolean</span></span>|<span data-ttu-id="6ff7a-242">Bloquear a disponibilidade de contatos do perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-242">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="6ff7a-243">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="6ff7a-243">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="6ff7a-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-244">Boolean</span></span>|<span data-ttu-id="6ff7a-245">Booliana que indica se a configuração não permitir a cópia/colar entre perfis está habilitada.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-245">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="6ff7a-246">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="6ff7a-246">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="6ff7a-247">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="6ff7a-247">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="6ff7a-248">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-248">Type of password that is required.</span></span> <span data-ttu-id="6ff7a-249">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-249">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="6ff7a-250">workProfilePasswordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="6ff7a-250">workProfilePasswordBlockFaceUnlock</span></span>|<span data-ttu-id="6ff7a-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-251">Boolean</span></span>|<span data-ttu-id="6ff7a-252">Indica se o desbloqueio facial deve ou não ser bloqueado para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-252">Indicates whether or not to block face unlock for work profile.</span></span>|
|<span data-ttu-id="6ff7a-253">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="6ff7a-253">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="6ff7a-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-254">Boolean</span></span>|<span data-ttu-id="6ff7a-255">Indica se o desbloqueio por impressão digital deve ou não ser bloqueado para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-255">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="6ff7a-256">workProfilePasswordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="6ff7a-256">workProfilePasswordBlockIrisUnlock</span></span>|<span data-ttu-id="6ff7a-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-257">Boolean</span></span>|<span data-ttu-id="6ff7a-258">Indica se o desbloqueio da íris deve ou não ser bloqueado para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-258">Indicates whether or not to block iris unlock for work profile.</span></span>|
|<span data-ttu-id="6ff7a-259">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="6ff7a-259">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="6ff7a-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-260">Boolean</span></span>|<span data-ttu-id="6ff7a-261">Indica se o Smart Lock e outros agentes de confiança do perfil de trabalho são bloqueados ou não.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-261">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="6ff7a-262">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6ff7a-262">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="6ff7a-263">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff7a-263">Int32</span></span>|<span data-ttu-id="6ff7a-264">Número de dias antes da expiração da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-264">Number of days before the work profile password expires.</span></span> <span data-ttu-id="6ff7a-265">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="6ff7a-265">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6ff7a-266">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6ff7a-266">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="6ff7a-267">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff7a-267">Int32</span></span>|<span data-ttu-id="6ff7a-268">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-268">Minimum length of work profile password.</span></span> <span data-ttu-id="6ff7a-269">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="6ff7a-269">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6ff7a-270">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="6ff7a-270">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="6ff7a-271">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff7a-271">Int32</span></span>|<span data-ttu-id="6ff7a-272">Número mínimo de caracteres numéricos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-272">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="6ff7a-273">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="6ff7a-273">Valid values 1 to 10</span></span>|
|<span data-ttu-id="6ff7a-274">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="6ff7a-274">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="6ff7a-275">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff7a-275">Int32</span></span>|<span data-ttu-id="6ff7a-276">Número mínimo de caracteres sem letra necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-276">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="6ff7a-277">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="6ff7a-277">Valid values 1 to 10</span></span>|
|<span data-ttu-id="6ff7a-278">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="6ff7a-278">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="6ff7a-279">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff7a-279">Int32</span></span>|<span data-ttu-id="6ff7a-280">Número mínimo de caracteres de carta necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-280">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="6ff7a-281">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="6ff7a-281">Valid values 1 to 10</span></span>|
|<span data-ttu-id="6ff7a-282">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="6ff7a-282">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="6ff7a-283">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff7a-283">Int32</span></span>|<span data-ttu-id="6ff7a-284">Número mínimo de caracteres de casos inferiores necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-284">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="6ff7a-285">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="6ff7a-285">Valid values 1 to 10</span></span>|
|<span data-ttu-id="6ff7a-286">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="6ff7a-286">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="6ff7a-287">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff7a-287">Int32</span></span>|<span data-ttu-id="6ff7a-288">Número mínimo de caracteres de maiúsculas necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-288">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="6ff7a-289">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="6ff7a-289">Valid values 1 to 10</span></span>|
|<span data-ttu-id="6ff7a-290">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="6ff7a-290">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="6ff7a-291">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff7a-291">Int32</span></span>|<span data-ttu-id="6ff7a-292">Número mínimo de símbolos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-292">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="6ff7a-293">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="6ff7a-293">Valid values 1 to 10</span></span>|
|<span data-ttu-id="6ff7a-294">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6ff7a-294">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6ff7a-295">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff7a-295">Int32</span></span>|<span data-ttu-id="6ff7a-296">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-296">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6ff7a-297">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6ff7a-297">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6ff7a-298">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff7a-298">Int32</span></span>|<span data-ttu-id="6ff7a-299">Número de senhas de perfil de trabalho anteriores a bloquear.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-299">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="6ff7a-300">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="6ff7a-300">Valid values 0 to 24</span></span>|
|<span data-ttu-id="6ff7a-301">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="6ff7a-301">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="6ff7a-302">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff7a-302">Int32</span></span>|<span data-ttu-id="6ff7a-303">Número de falhas de entrada permitidas antes que o perfil de trabalho seja removido e todos os dados corporativos excluídos.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-303">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="6ff7a-304">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="6ff7a-304">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6ff7a-305">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6ff7a-305">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="6ff7a-306">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6ff7a-306">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="6ff7a-307">Tipo de senha de perfil de trabalho necessária.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-307">Type of work profile password that is required.</span></span> <span data-ttu-id="6ff7a-308">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-308">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="6ff7a-309">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="6ff7a-309">workProfileRequirePassword</span></span>|<span data-ttu-id="6ff7a-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-310">Boolean</span></span>|<span data-ttu-id="6ff7a-311">A senha é necessária ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="6ff7a-311">Password is required or not for work profile</span></span>|
|<span data-ttu-id="6ff7a-312">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="6ff7a-312">securityRequireVerifyApps</span></span>|<span data-ttu-id="6ff7a-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-313">Boolean</span></span>|<span data-ttu-id="6ff7a-314">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-314">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="6ff7a-315">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="6ff7a-315">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="6ff7a-316">String</span><span class="sxs-lookup"><span data-stu-id="6ff7a-316">String</span></span>|<span data-ttu-id="6ff7a-317">Habilita o modo de bloqueio para VPN sempre ativada.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-317">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="6ff7a-318">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="6ff7a-318">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="6ff7a-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-319">Boolean</span></span>|<span data-ttu-id="6ff7a-320">Habilita o modo de bloqueio para VPN sempre ativada.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-320">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="6ff7a-321">workProfileAllowWzelts</span><span class="sxs-lookup"><span data-stu-id="6ff7a-321">workProfileAllowWidgets</span></span>|<span data-ttu-id="6ff7a-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-322">Boolean</span></span>|<span data-ttu-id="6ff7a-323">Permitir widgets de aplicativos de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-323">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="6ff7a-324">workProfileBlockPersonalAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="6ff7a-324">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="6ff7a-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff7a-325">Boolean</span></span>|<span data-ttu-id="6ff7a-326">Impedir instalações de aplicativos de fontes desconhecidas no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-326">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="6ff7a-327">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ff7a-327">Response</span></span>
<span data-ttu-id="6ff7a-328">Se tiver êxito, este método retornará um código de resposta e um objeto `201 Created` [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-328">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ff7a-329">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ff7a-329">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ff7a-330">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ff7a-330">Request</span></span>
<span data-ttu-id="6ff7a-331">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-331">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3141

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
  "workProfileAllowAppInstallsFromUnknownSources": true,
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

### <a name="response"></a><span data-ttu-id="6ff7a-332">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ff7a-332">Response</span></span>
<span data-ttu-id="6ff7a-p131">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ff7a-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3313

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
  "workProfileAllowAppInstallsFromUnknownSources": true,
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




