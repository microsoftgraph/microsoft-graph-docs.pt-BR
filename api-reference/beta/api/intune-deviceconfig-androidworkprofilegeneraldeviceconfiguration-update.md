---
title: Atualizar androidWorkProfileGeneralDeviceConfiguration
description: Atualizar as propriedades de um objeto androidWorkProfileGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7b8e9f0bcfcde7ffc4dbc19a469e663b2d8f12b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154681"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="1447d-103">Atualizar androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1447d-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="1447d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1447d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1447d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1447d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1447d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1447d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1447d-107">Atualizar as propriedades de um [objeto androidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1447d-107">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1447d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1447d-108">Prerequisites</span></span>
<span data-ttu-id="1447d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1447d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1447d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1447d-111">Permission type</span></span>|<span data-ttu-id="1447d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1447d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1447d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1447d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1447d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1447d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1447d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1447d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1447d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1447d-116">Not supported.</span></span>|
|<span data-ttu-id="1447d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1447d-117">Application</span></span>|<span data-ttu-id="1447d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1447d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1447d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1447d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1447d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1447d-120">Request headers</span></span>
|<span data-ttu-id="1447d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1447d-121">Header</span></span>|<span data-ttu-id="1447d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1447d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1447d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1447d-123">Authorization</span></span>|<span data-ttu-id="1447d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1447d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1447d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1447d-125">Accept</span></span>|<span data-ttu-id="1447d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1447d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1447d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1447d-127">Request body</span></span>
<span data-ttu-id="1447d-128">No corpo da solicitação, fornece uma representação JSON do objeto [androidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1447d-128">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="1447d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1447d-129">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="1447d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1447d-130">Property</span></span>|<span data-ttu-id="1447d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1447d-131">Type</span></span>|<span data-ttu-id="1447d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1447d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1447d-133">id</span><span class="sxs-lookup"><span data-stu-id="1447d-133">id</span></span>|<span data-ttu-id="1447d-134">String</span><span class="sxs-lookup"><span data-stu-id="1447d-134">String</span></span>|<span data-ttu-id="1447d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1447d-135">Key of the entity.</span></span> <span data-ttu-id="1447d-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1447d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1447d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1447d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1447d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1447d-138">DateTimeOffset</span></span>|<span data-ttu-id="1447d-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1447d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1447d-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1447d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1447d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1447d-141">roleScopeTagIds</span></span>|<span data-ttu-id="1447d-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1447d-142">String collection</span></span>|<span data-ttu-id="1447d-143">Lista de Marcas de Escopo para esta instância de Entidade.</span><span class="sxs-lookup"><span data-stu-id="1447d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1447d-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1447d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1447d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1447d-145">supportsScopeTags</span></span>|<span data-ttu-id="1447d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-146">Boolean</span></span>|<span data-ttu-id="1447d-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="1447d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1447d-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="1447d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1447d-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvida excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="1447d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1447d-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1447d-150">This property is read-only.</span></span> <span data-ttu-id="1447d-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1447d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1447d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1447d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1447d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1447d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1447d-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="1447d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1447d-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1447d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1447d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1447d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1447d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1447d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1447d-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="1447d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1447d-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1447d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1447d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1447d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1447d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1447d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1447d-162">A regra de aplicabilidade do modo de dispositivo para esta política.</span><span class="sxs-lookup"><span data-stu-id="1447d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1447d-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1447d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1447d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1447d-164">createdDateTime</span></span>|<span data-ttu-id="1447d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1447d-165">DateTimeOffset</span></span>|<span data-ttu-id="1447d-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1447d-166">DateTime the object was created.</span></span> <span data-ttu-id="1447d-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1447d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1447d-168">description</span><span class="sxs-lookup"><span data-stu-id="1447d-168">description</span></span>|<span data-ttu-id="1447d-169">String</span><span class="sxs-lookup"><span data-stu-id="1447d-169">String</span></span>|<span data-ttu-id="1447d-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1447d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1447d-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1447d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1447d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="1447d-172">displayName</span></span>|<span data-ttu-id="1447d-173">String</span><span class="sxs-lookup"><span data-stu-id="1447d-173">String</span></span>|<span data-ttu-id="1447d-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1447d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1447d-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1447d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1447d-176">versão</span><span class="sxs-lookup"><span data-stu-id="1447d-176">version</span></span>|<span data-ttu-id="1447d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1447d-177">Int32</span></span>|<span data-ttu-id="1447d-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1447d-178">Version of the device configuration.</span></span> <span data-ttu-id="1447d-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1447d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1447d-180">passwordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="1447d-180">passwordBlockFaceUnlock</span></span>|<span data-ttu-id="1447d-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-181">Boolean</span></span>|<span data-ttu-id="1447d-182">Indica se o desbloqueio facial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1447d-182">Indicates whether or not to block face unlock.</span></span>|
|<span data-ttu-id="1447d-183">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="1447d-183">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="1447d-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-184">Boolean</span></span>|<span data-ttu-id="1447d-185">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1447d-185">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="1447d-186">passwordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="1447d-186">passwordBlockIrisUnlock</span></span>|<span data-ttu-id="1447d-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-187">Boolean</span></span>|<span data-ttu-id="1447d-188">Indica se o desbloqueio da íris deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1447d-188">Indicates whether or not to block iris unlock.</span></span>|
|<span data-ttu-id="1447d-189">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="1447d-189">passwordBlockTrustAgents</span></span>|<span data-ttu-id="1447d-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-190">Boolean</span></span>|<span data-ttu-id="1447d-191">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="1447d-191">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="1447d-192">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1447d-192">passwordExpirationDays</span></span>|<span data-ttu-id="1447d-193">Int32</span><span class="sxs-lookup"><span data-stu-id="1447d-193">Int32</span></span>|<span data-ttu-id="1447d-194">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="1447d-194">Number of days before the password expires.</span></span> <span data-ttu-id="1447d-195">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="1447d-195">Valid values 1 to 365</span></span>|
|<span data-ttu-id="1447d-196">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1447d-196">passwordMinimumLength</span></span>|<span data-ttu-id="1447d-197">Int32</span><span class="sxs-lookup"><span data-stu-id="1447d-197">Int32</span></span>|<span data-ttu-id="1447d-198">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="1447d-198">Minimum length of passwords.</span></span> <span data-ttu-id="1447d-199">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="1447d-199">Valid values 4 to 16</span></span>|
|<span data-ttu-id="1447d-200">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="1447d-200">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="1447d-201">Int32</span><span class="sxs-lookup"><span data-stu-id="1447d-201">Int32</span></span>|<span data-ttu-id="1447d-202">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="1447d-202">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="1447d-203">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="1447d-203">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="1447d-204">Int32</span><span class="sxs-lookup"><span data-stu-id="1447d-204">Int32</span></span>|<span data-ttu-id="1447d-205">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="1447d-205">Number of previous passwords to block.</span></span> <span data-ttu-id="1447d-206">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="1447d-206">Valid values 0 to 24</span></span>|
|<span data-ttu-id="1447d-207">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="1447d-207">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="1447d-208">Int32</span><span class="sxs-lookup"><span data-stu-id="1447d-208">Int32</span></span>|<span data-ttu-id="1447d-209">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="1447d-209">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="1447d-210">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="1447d-210">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1447d-211">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1447d-211">passwordRequiredType</span></span>|[<span data-ttu-id="1447d-212">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1447d-212">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="1447d-213">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="1447d-213">Type of password that is required.</span></span> <span data-ttu-id="1447d-214">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="1447d-214">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="1447d-215">workProfileAllowAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="1447d-215">workProfileAllowAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="1447d-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-216">Boolean</span></span>|<span data-ttu-id="1447d-217">Indica se é para permitir a instalação de aplicativos de fontes desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="1447d-217">Indicates whether to allow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="1447d-218">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="1447d-218">workProfileDataSharingType</span></span>|[<span data-ttu-id="1447d-219">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="1447d-219">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="1447d-220">Tipo de compartilhamento de dados permitido.</span><span class="sxs-lookup"><span data-stu-id="1447d-220">Type of data sharing that is allowed.</span></span> <span data-ttu-id="1447d-221">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="1447d-221">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="1447d-222">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="1447d-222">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="1447d-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-223">Boolean</span></span>|<span data-ttu-id="1447d-224">Indica se as notificações de bloqueio são ou não durante o bloqueio do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1447d-224">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="1447d-225">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="1447d-225">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="1447d-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-226">Boolean</span></span>|<span data-ttu-id="1447d-227">Impedir que os usuários adicionem/removam contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1447d-227">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="1447d-228">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="1447d-228">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="1447d-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-229">Boolean</span></span>|<span data-ttu-id="1447d-230">Permitir que dispositivos bluetooth acessem contatos corporativos.</span><span class="sxs-lookup"><span data-stu-id="1447d-230">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="1447d-231">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="1447d-231">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="1447d-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-232">Boolean</span></span>|<span data-ttu-id="1447d-233">Bloquear captura de tela no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1447d-233">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="1447d-234">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="1447d-234">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="1447d-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-235">Boolean</span></span>|<span data-ttu-id="1447d-236">Bloquear a ID de chamada do perfil de trabalho de exibição no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="1447d-236">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="1447d-237">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="1447d-237">workProfileBlockCamera</span></span>|<span data-ttu-id="1447d-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-238">Boolean</span></span>|<span data-ttu-id="1447d-239">Bloquear câmera de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1447d-239">Block work profile camera.</span></span>|
|<span data-ttu-id="1447d-240">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="1447d-240">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="1447d-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-241">Boolean</span></span>|<span data-ttu-id="1447d-242">Bloquear a disponibilidade de contatos do perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="1447d-242">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="1447d-243">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="1447d-243">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="1447d-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-244">Boolean</span></span>|<span data-ttu-id="1447d-245">Booliana que indica se a configuração não permitir cópia/colar perfil cruzado está habilitada.</span><span class="sxs-lookup"><span data-stu-id="1447d-245">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="1447d-246">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="1447d-246">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="1447d-247">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="1447d-247">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="1447d-248">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="1447d-248">Type of password that is required.</span></span> <span data-ttu-id="1447d-249">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="1447d-249">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="1447d-250">workProfilePasswordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="1447d-250">workProfilePasswordBlockFaceUnlock</span></span>|<span data-ttu-id="1447d-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-251">Boolean</span></span>|<span data-ttu-id="1447d-252">Indica se o desbloqueio facial deve ou não ser bloqueado para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1447d-252">Indicates whether or not to block face unlock for work profile.</span></span>|
|<span data-ttu-id="1447d-253">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="1447d-253">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="1447d-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-254">Boolean</span></span>|<span data-ttu-id="1447d-255">Indica se o desbloqueio por impressão digital deve ou não ser bloqueado para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1447d-255">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="1447d-256">workProfilePasswordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="1447d-256">workProfilePasswordBlockIrisUnlock</span></span>|<span data-ttu-id="1447d-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-257">Boolean</span></span>|<span data-ttu-id="1447d-258">Indica se o desbloqueio da íris deve ou não ser bloqueado para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1447d-258">Indicates whether or not to block iris unlock for work profile.</span></span>|
|<span data-ttu-id="1447d-259">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="1447d-259">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="1447d-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-260">Boolean</span></span>|<span data-ttu-id="1447d-261">Indica se o Smart Lock e outros agentes de confiança do perfil de trabalho são bloqueados ou não.</span><span class="sxs-lookup"><span data-stu-id="1447d-261">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="1447d-262">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1447d-262">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="1447d-263">Int32</span><span class="sxs-lookup"><span data-stu-id="1447d-263">Int32</span></span>|<span data-ttu-id="1447d-264">Número de dias antes da expiração da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1447d-264">Number of days before the work profile password expires.</span></span> <span data-ttu-id="1447d-265">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="1447d-265">Valid values 1 to 365</span></span>|
|<span data-ttu-id="1447d-266">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1447d-266">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="1447d-267">Int32</span><span class="sxs-lookup"><span data-stu-id="1447d-267">Int32</span></span>|<span data-ttu-id="1447d-268">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1447d-268">Minimum length of work profile password.</span></span> <span data-ttu-id="1447d-269">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="1447d-269">Valid values 4 to 16</span></span>|
|<span data-ttu-id="1447d-270">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="1447d-270">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="1447d-271">Int32</span><span class="sxs-lookup"><span data-stu-id="1447d-271">Int32</span></span>|<span data-ttu-id="1447d-272">Número mínimo de caracteres numéricos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1447d-272">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="1447d-273">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="1447d-273">Valid values 1 to 10</span></span>|
|<span data-ttu-id="1447d-274">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="1447d-274">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="1447d-275">Int32</span><span class="sxs-lookup"><span data-stu-id="1447d-275">Int32</span></span>|<span data-ttu-id="1447d-276">Número mínimo de caracteres sem letra necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1447d-276">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="1447d-277">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="1447d-277">Valid values 1 to 10</span></span>|
|<span data-ttu-id="1447d-278">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="1447d-278">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="1447d-279">Int32</span><span class="sxs-lookup"><span data-stu-id="1447d-279">Int32</span></span>|<span data-ttu-id="1447d-280">Número mínimo de caracteres de carta necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1447d-280">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="1447d-281">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="1447d-281">Valid values 1 to 10</span></span>|
|<span data-ttu-id="1447d-282">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="1447d-282">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="1447d-283">Int32</span><span class="sxs-lookup"><span data-stu-id="1447d-283">Int32</span></span>|<span data-ttu-id="1447d-284">Número mínimo de caracteres de casos inferiores necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1447d-284">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="1447d-285">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="1447d-285">Valid values 1 to 10</span></span>|
|<span data-ttu-id="1447d-286">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="1447d-286">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="1447d-287">Int32</span><span class="sxs-lookup"><span data-stu-id="1447d-287">Int32</span></span>|<span data-ttu-id="1447d-288">Número mínimo de caracteres de maiúsculas necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1447d-288">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="1447d-289">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="1447d-289">Valid values 1 to 10</span></span>|
|<span data-ttu-id="1447d-290">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="1447d-290">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="1447d-291">Int32</span><span class="sxs-lookup"><span data-stu-id="1447d-291">Int32</span></span>|<span data-ttu-id="1447d-292">Número mínimo de símbolos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1447d-292">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="1447d-293">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="1447d-293">Valid values 1 to 10</span></span>|
|<span data-ttu-id="1447d-294">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="1447d-294">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="1447d-295">Int32</span><span class="sxs-lookup"><span data-stu-id="1447d-295">Int32</span></span>|<span data-ttu-id="1447d-296">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="1447d-296">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="1447d-297">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="1447d-297">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="1447d-298">Int32</span><span class="sxs-lookup"><span data-stu-id="1447d-298">Int32</span></span>|<span data-ttu-id="1447d-299">Número de senhas de perfil de trabalho anteriores a bloquear.</span><span class="sxs-lookup"><span data-stu-id="1447d-299">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="1447d-300">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="1447d-300">Valid values 0 to 24</span></span>|
|<span data-ttu-id="1447d-301">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="1447d-301">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="1447d-302">Int32</span><span class="sxs-lookup"><span data-stu-id="1447d-302">Int32</span></span>|<span data-ttu-id="1447d-303">Número de falhas de entrada permitidas antes que o perfil de trabalho seja removido e todos os dados corporativos excluídos.</span><span class="sxs-lookup"><span data-stu-id="1447d-303">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="1447d-304">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="1447d-304">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1447d-305">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1447d-305">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="1447d-306">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1447d-306">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="1447d-307">Tipo de senha de perfil de trabalho necessária.</span><span class="sxs-lookup"><span data-stu-id="1447d-307">Type of work profile password that is required.</span></span> <span data-ttu-id="1447d-308">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="1447d-308">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="1447d-309">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="1447d-309">workProfileRequirePassword</span></span>|<span data-ttu-id="1447d-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-310">Boolean</span></span>|<span data-ttu-id="1447d-311">A senha é necessária ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="1447d-311">Password is required or not for work profile</span></span>|
|<span data-ttu-id="1447d-312">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="1447d-312">securityRequireVerifyApps</span></span>|<span data-ttu-id="1447d-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-313">Boolean</span></span>|<span data-ttu-id="1447d-314">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="1447d-314">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="1447d-315">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="1447d-315">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="1447d-316">String</span><span class="sxs-lookup"><span data-stu-id="1447d-316">String</span></span>|<span data-ttu-id="1447d-317">Habilita o modo de bloqueio para VPN sempre ativada.</span><span class="sxs-lookup"><span data-stu-id="1447d-317">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="1447d-318">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="1447d-318">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="1447d-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-319">Boolean</span></span>|<span data-ttu-id="1447d-320">Habilita o modo de bloqueio para VPN sempre ativada.</span><span class="sxs-lookup"><span data-stu-id="1447d-320">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="1447d-321">workProfileAllowWzelts</span><span class="sxs-lookup"><span data-stu-id="1447d-321">workProfileAllowWidgets</span></span>|<span data-ttu-id="1447d-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-322">Boolean</span></span>|<span data-ttu-id="1447d-323">Permitir widgets de aplicativos de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1447d-323">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="1447d-324">workProfileBlockPersonalAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="1447d-324">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="1447d-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="1447d-325">Boolean</span></span>|<span data-ttu-id="1447d-326">Impedir instalações de aplicativos de fontes desconhecidas no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="1447d-326">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="1447d-327">Resposta</span><span class="sxs-lookup"><span data-stu-id="1447d-327">Response</span></span>
<span data-ttu-id="1447d-328">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1447d-328">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1447d-329">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1447d-329">Example</span></span>

### <a name="request"></a><span data-ttu-id="1447d-330">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1447d-330">Request</span></span>
<span data-ttu-id="1447d-331">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1447d-331">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="1447d-332">Resposta</span><span class="sxs-lookup"><span data-stu-id="1447d-332">Response</span></span>
<span data-ttu-id="1447d-p131">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1447d-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




