---
title: Criar macOSGeneralDeviceConfiguration
description: Cria um novo objeto macOSGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 102c8386bfa0336a22dda3111a19e64b311b4661
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948279"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="44653-103">Criar macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="44653-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="44653-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="44653-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44653-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="44653-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44653-106">Cria um novo objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44653-106">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44653-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="44653-107">Prerequisites</span></span>
<span data-ttu-id="44653-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44653-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44653-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44653-110">Permission type</span></span>|<span data-ttu-id="44653-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="44653-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44653-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44653-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44653-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44653-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44653-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44653-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44653-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44653-115">Not supported.</span></span>|
|<span data-ttu-id="44653-116">Application</span><span class="sxs-lookup"><span data-stu-id="44653-116">Application</span></span>|<span data-ttu-id="44653-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44653-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44653-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44653-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="44653-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44653-119">Request headers</span></span>
|<span data-ttu-id="44653-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="44653-120">Header</span></span>|<span data-ttu-id="44653-121">Valor</span><span class="sxs-lookup"><span data-stu-id="44653-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44653-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="44653-122">Authorization</span></span>|<span data-ttu-id="44653-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44653-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44653-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="44653-124">Accept</span></span>|<span data-ttu-id="44653-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44653-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44653-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44653-126">Request body</span></span>
<span data-ttu-id="44653-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="44653-127">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="44653-128">A tabela a seguir mostra as propriedades obrigatórias ao criar macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="44653-128">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="44653-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44653-129">Property</span></span>|<span data-ttu-id="44653-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="44653-130">Type</span></span>|<span data-ttu-id="44653-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="44653-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44653-132">id</span><span class="sxs-lookup"><span data-stu-id="44653-132">id</span></span>|<span data-ttu-id="44653-133">String</span><span class="sxs-lookup"><span data-stu-id="44653-133">String</span></span>|<span data-ttu-id="44653-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="44653-134">Key of the entity.</span></span> <span data-ttu-id="44653-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44653-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44653-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44653-136">lastModifiedDateTime</span></span>|<span data-ttu-id="44653-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44653-137">DateTimeOffset</span></span>|<span data-ttu-id="44653-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="44653-138">DateTime the object was last modified.</span></span> <span data-ttu-id="44653-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44653-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44653-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="44653-140">roleScopeTagIds</span></span>|<span data-ttu-id="44653-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="44653-141">String collection</span></span>|<span data-ttu-id="44653-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="44653-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="44653-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44653-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44653-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="44653-144">supportsScopeTags</span></span>|<span data-ttu-id="44653-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-145">Boolean</span></span>|<span data-ttu-id="44653-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="44653-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="44653-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="44653-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="44653-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="44653-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="44653-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44653-149">This property is read-only.</span></span> <span data-ttu-id="44653-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44653-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44653-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="44653-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="44653-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="44653-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="44653-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="44653-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="44653-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44653-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44653-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="44653-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="44653-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="44653-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="44653-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="44653-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="44653-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44653-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44653-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="44653-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="44653-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="44653-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="44653-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="44653-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="44653-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44653-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44653-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44653-163">createdDateTime</span></span>|<span data-ttu-id="44653-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44653-164">DateTimeOffset</span></span>|<span data-ttu-id="44653-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="44653-165">DateTime the object was created.</span></span> <span data-ttu-id="44653-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44653-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44653-167">description</span><span class="sxs-lookup"><span data-stu-id="44653-167">description</span></span>|<span data-ttu-id="44653-168">String</span><span class="sxs-lookup"><span data-stu-id="44653-168">String</span></span>|<span data-ttu-id="44653-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44653-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="44653-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44653-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44653-171">displayName</span><span class="sxs-lookup"><span data-stu-id="44653-171">displayName</span></span>|<span data-ttu-id="44653-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44653-172">String</span></span>|<span data-ttu-id="44653-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44653-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="44653-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44653-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44653-175">versão</span><span class="sxs-lookup"><span data-stu-id="44653-175">version</span></span>|<span data-ttu-id="44653-176">Int32</span><span class="sxs-lookup"><span data-stu-id="44653-176">Int32</span></span>|<span data-ttu-id="44653-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44653-177">Version of the device configuration.</span></span> <span data-ttu-id="44653-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44653-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44653-179">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="44653-179">compliantAppsList</span></span>|<span data-ttu-id="44653-180">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="44653-180">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="44653-181">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="44653-181">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="44653-182">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="44653-182">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="44653-183">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="44653-183">compliantAppListType</span></span>|[<span data-ttu-id="44653-184">appListType</span><span class="sxs-lookup"><span data-stu-id="44653-184">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="44653-185">Lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="44653-185">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="44653-186">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="44653-186">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="44653-187">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="44653-187">emailInDomainSuffixes</span></span>|<span data-ttu-id="44653-188">String collection</span><span class="sxs-lookup"><span data-stu-id="44653-188">String collection</span></span>|<span data-ttu-id="44653-189">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="44653-189">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="44653-190">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="44653-190">passwordBlockSimple</span></span>|<span data-ttu-id="44653-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="44653-191">Boolean</span></span>|<span data-ttu-id="44653-192">Bloquear senhas simples.</span><span class="sxs-lookup"><span data-stu-id="44653-192">Block simple passwords.</span></span>|
|<span data-ttu-id="44653-193">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="44653-193">passwordExpirationDays</span></span>|<span data-ttu-id="44653-194">Int32</span><span class="sxs-lookup"><span data-stu-id="44653-194">Int32</span></span>|<span data-ttu-id="44653-195">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="44653-195">Number of days before the password expires.</span></span>|
|<span data-ttu-id="44653-196">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="44653-196">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="44653-197">Int32</span><span class="sxs-lookup"><span data-stu-id="44653-197">Int32</span></span>|<span data-ttu-id="44653-198">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="44653-198">Number of character sets a password must contain.</span></span> <span data-ttu-id="44653-199">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="44653-199">Valid values 0 to 4</span></span>|
|<span data-ttu-id="44653-200">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="44653-200">passwordMinimumLength</span></span>|<span data-ttu-id="44653-201">Int32</span><span class="sxs-lookup"><span data-stu-id="44653-201">Int32</span></span>|<span data-ttu-id="44653-202">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="44653-202">Minimum length of passwords.</span></span>|
|<span data-ttu-id="44653-203">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="44653-203">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="44653-204">Int32</span><span class="sxs-lookup"><span data-stu-id="44653-204">Int32</span></span>|<span data-ttu-id="44653-205">Minutos de inatividade necessários antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="44653-205">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="44653-206">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="44653-206">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="44653-207">Int32</span><span class="sxs-lookup"><span data-stu-id="44653-207">Int32</span></span>|<span data-ttu-id="44653-208">Minutos de inatividade necessários antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="44653-208">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="44653-209">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="44653-209">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="44653-210">Int32</span><span class="sxs-lookup"><span data-stu-id="44653-210">Int32</span></span>|<span data-ttu-id="44653-211">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="44653-211">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="44653-212">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="44653-212">passwordRequiredType</span></span>|[<span data-ttu-id="44653-213">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="44653-213">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="44653-214">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="44653-214">Type of password that is required.</span></span> <span data-ttu-id="44653-215">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="44653-215">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="44653-216">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="44653-216">passwordRequired</span></span>|<span data-ttu-id="44653-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-217">Boolean</span></span>|<span data-ttu-id="44653-218">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="44653-218">Whether or not to require a password.</span></span>|
|<span data-ttu-id="44653-219">Propriedadeskeychainblockcloudsync</span><span class="sxs-lookup"><span data-stu-id="44653-219">keychainBlockCloudSync</span></span>|<span data-ttu-id="44653-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-220">Boolean</span></span>|<span data-ttu-id="44653-221">Indica se a sincronização de chaves do iCloud está bloqueada (macOS 10,12 e posterior).</span><span class="sxs-lookup"><span data-stu-id="44653-221">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="44653-222">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="44653-222">airPrintBlocked</span></span>|<span data-ttu-id="44653-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-223">Boolean</span></span>|<span data-ttu-id="44653-224">Indica se o arquivo de impressão está bloqueado (macOS 10,12 e posterior).</span><span class="sxs-lookup"><span data-stu-id="44653-224">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="44653-225">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="44653-225">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="44653-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-226">Boolean</span></span>|<span data-ttu-id="44653-227">Indica se certificados confiáveis são necessários para comunicação de impressão TLS (macOS 10,13 e posterior).</span><span class="sxs-lookup"><span data-stu-id="44653-227">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="44653-228">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="44653-228">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="44653-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-229">Boolean</span></span>|<span data-ttu-id="44653-230">Indica se a descoberta de impressoras de impressão do iBeacon está ou não bloqueada.</span><span class="sxs-lookup"><span data-stu-id="44653-230">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="44653-231">Isso impede os beacons Bluetooth de impressão de mensagens de phishing para tráfego de rede (macOS 10,3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="44653-231">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="44653-232">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="44653-232">safariBlockAutofill</span></span>|<span data-ttu-id="44653-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-233">Boolean</span></span>|<span data-ttu-id="44653-234">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="44653-234">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="44653-235">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="44653-235">cameraBlocked</span></span>|<span data-ttu-id="44653-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-236">Boolean</span></span>|<span data-ttu-id="44653-237">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44653-237">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="44653-238">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="44653-238">iTunesBlockMusicService</span></span>|<span data-ttu-id="44653-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-239">Boolean</span></span>|<span data-ttu-id="44653-240">Indica se o serviço de música deve ou não ser bloqueado e o aplicativo de música é revertido para o modo clássico.</span><span class="sxs-lookup"><span data-stu-id="44653-240">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="44653-241">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="44653-241">spotlightBlockInternetResults</span></span>|<span data-ttu-id="44653-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-242">Boolean</span></span>|<span data-ttu-id="44653-243">Indica se o Spotlight deve ou não bloquear o retorno de qualquer resultado de uma pesquisa na Internet.</span><span class="sxs-lookup"><span data-stu-id="44653-243">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="44653-244">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="44653-244">keyboardBlockDictation</span></span>|<span data-ttu-id="44653-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-245">Boolean</span></span>|<span data-ttu-id="44653-246">Indica se o usuário será ou não impedido de usar a entrada de ditado.</span><span class="sxs-lookup"><span data-stu-id="44653-246">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="44653-247">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="44653-247">definitionLookupBlocked</span></span>|<span data-ttu-id="44653-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-248">Boolean</span></span>|<span data-ttu-id="44653-249">Indica se a pesquisa de definição deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="44653-249">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="44653-250">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="44653-250">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="44653-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-251">Boolean</span></span>|<span data-ttu-id="44653-252">Indica se os usuários devem ou não bloquear seu Mac com o Apple Watch.</span><span class="sxs-lookup"><span data-stu-id="44653-252">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="44653-253">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="44653-253">iTunesBlockFileSharing</span></span>|<span data-ttu-id="44653-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-254">Boolean</span></span>|<span data-ttu-id="44653-255">Indica se os arquivos devem ou não ser transferidos usando o iTunes.</span><span class="sxs-lookup"><span data-stu-id="44653-255">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="44653-256">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="44653-256">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="44653-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-257">Boolean</span></span>|<span data-ttu-id="44653-258">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="44653-258">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="44653-259">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="44653-259">iCloudBlockMail</span></span>|<span data-ttu-id="44653-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-260">Boolean</span></span>|<span data-ttu-id="44653-261">Indica se o iCloud deve ou não bloquear emails de sincronização.</span><span class="sxs-lookup"><span data-stu-id="44653-261">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="44653-262">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="44653-262">iCloudBlockAddressBook</span></span>|<span data-ttu-id="44653-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-263">Boolean</span></span>|<span data-ttu-id="44653-264">Indica se o iCloud deve ou não bloquear os contatos de sincronização.</span><span class="sxs-lookup"><span data-stu-id="44653-264">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="44653-265">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="44653-265">iCloudBlockCalendar</span></span>|<span data-ttu-id="44653-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-266">Boolean</span></span>|<span data-ttu-id="44653-267">Indica se o iCloud deve ou não bloquear calendários de sincronização.</span><span class="sxs-lookup"><span data-stu-id="44653-267">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="44653-268">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="44653-268">iCloudBlockReminders</span></span>|<span data-ttu-id="44653-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-269">Boolean</span></span>|<span data-ttu-id="44653-270">Indica se o iCloud deve ou não bloquear lembretes de sincronização.</span><span class="sxs-lookup"><span data-stu-id="44653-270">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="44653-271">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="44653-271">iCloudBlockBookmarks</span></span>|<span data-ttu-id="44653-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-272">Boolean</span></span>|<span data-ttu-id="44653-273">Indica se o iCloud deve ou não bloquear os indicadores de sincronização.</span><span class="sxs-lookup"><span data-stu-id="44653-273">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="44653-274">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="44653-274">iCloudBlockNotes</span></span>|<span data-ttu-id="44653-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-275">Boolean</span></span>|<span data-ttu-id="44653-276">Indica se o iCloud deve ou não bloquear as anotações de sincronização.</span><span class="sxs-lookup"><span data-stu-id="44653-276">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="44653-277">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="44653-277">airDropBlocked</span></span>|<span data-ttu-id="44653-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-278">Boolean</span></span>|<span data-ttu-id="44653-279">Indica se o recurso de recebimento de esficado deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="44653-279">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="44653-280">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="44653-280">passwordBlockModification</span></span>|<span data-ttu-id="44653-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-281">Boolean</span></span>|<span data-ttu-id="44653-282">Indica se a modificação de senha deve ou não ser permitida.</span><span class="sxs-lookup"><span data-stu-id="44653-282">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="44653-283">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="44653-283">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="44653-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-284">Boolean</span></span>|<span data-ttu-id="44653-285">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="44653-285">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="44653-286">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="44653-286">passwordBlockAutoFill</span></span>|<span data-ttu-id="44653-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-287">Boolean</span></span>|<span data-ttu-id="44653-288">Indica se o recurso de senhas de preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="44653-288">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="44653-289">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="44653-289">passwordBlockProximityRequests</span></span>|<span data-ttu-id="44653-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-290">Boolean</span></span>|<span data-ttu-id="44653-291">Indica se as senhas de solicitação devem ou não ser bloqueadas de dispositivos próximos.</span><span class="sxs-lookup"><span data-stu-id="44653-291">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="44653-292">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="44653-292">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="44653-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-293">Boolean</span></span>|<span data-ttu-id="44653-294">Indica se as senhas de compartilhamento devem ou não ser bloqueadas com o recurso de senha de soltura.</span><span class="sxs-lookup"><span data-stu-id="44653-294">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="44653-295">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="44653-295">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="44653-296">Int32</span><span class="sxs-lookup"><span data-stu-id="44653-296">Int32</span></span>|<span data-ttu-id="44653-297">Define o número de dias que uma atualização de software será delyed para um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="44653-297">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="44653-298">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="44653-298">Valid values 0 to 90</span></span>|
|<span data-ttu-id="44653-299">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="44653-299">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="44653-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-300">Boolean</span></span>|<span data-ttu-id="44653-301">Indica se o usuário deve ou não atrasar a visibilidade de atualizações de software quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="44653-301">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="44653-302">contentCachingBlocked</span><span class="sxs-lookup"><span data-stu-id="44653-302">contentCachingBlocked</span></span>|<span data-ttu-id="44653-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-303">Boolean</span></span>|<span data-ttu-id="44653-304">Indica se o cache de conteúdo deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="44653-304">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="44653-305">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="44653-305">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="44653-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-306">Boolean</span></span>|<span data-ttu-id="44653-307">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="44653-307">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="44653-308">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="44653-308">screenCaptureBlocked</span></span>|<span data-ttu-id="44653-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-309">Boolean</span></span>|<span data-ttu-id="44653-310">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="44653-310">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="44653-311">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="44653-311">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="44653-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-312">Boolean</span></span>|<span data-ttu-id="44653-313">Indica se a observação de tela remota deve ou não ser permitida por aplicativo de sala de aula.</span><span class="sxs-lookup"><span data-stu-id="44653-313">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="44653-314">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="44653-314">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="44653-315">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="44653-315">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="44653-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-316">Boolean</span></span>|<span data-ttu-id="44653-317">Indica se a permissão será ou não automaticamente para o professor de um curso gerenciado no aplicativo da sala de aula para exibir a tela de um aluno sem avisar.</span><span class="sxs-lookup"><span data-stu-id="44653-317">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="44653-318">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="44653-318">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="44653-319">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="44653-319">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="44653-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-320">Boolean</span></span>|<span data-ttu-id="44653-321">Indica se a permissão será ou não automaticamente para as solicitações do professor, sem avisar o aluno.</span><span class="sxs-lookup"><span data-stu-id="44653-321">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="44653-322">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="44653-322">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="44653-323">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="44653-323">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="44653-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-324">Boolean</span></span>|<span data-ttu-id="44653-325">Indica se um aluno inscrito em um curso não gerenciado via sala de aula será solicitado a solicitar permissão do professor ao tentar sair do curso.</span><span class="sxs-lookup"><span data-stu-id="44653-325">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="44653-326">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="44653-326">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="44653-327">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="44653-327">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="44653-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-328">Boolean</span></span>|<span data-ttu-id="44653-329">Indica se o professor deve ou não bloquear aplicativos ou o dispositivo sem avisar o aluno.</span><span class="sxs-lookup"><span data-stu-id="44653-329">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="44653-330">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="44653-330">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="44653-331">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="44653-331">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="44653-332">Boolean</span><span class="sxs-lookup"><span data-stu-id="44653-332">Boolean</span></span>|<span data-ttu-id="44653-333">Indica se o usuário será ou não impedido de continuar o trabalho que iniciou em um dispositivo MacOS em outro dispositivo iOS ou MacOS (MacOS 10,15 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="44653-333">Indicates whether or not to block the user from continuing work that they started on a MacOS device on another iOS or MacOS device (MacOS 10.15 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="44653-334">Resposta</span><span class="sxs-lookup"><span data-stu-id="44653-334">Response</span></span>
<span data-ttu-id="44653-335">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44653-335">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44653-336">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44653-336">Example</span></span>

### <a name="request"></a><span data-ttu-id="44653-337">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44653-337">Request</span></span>
<span data-ttu-id="44653-338">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44653-338">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3146

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
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
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true
}
```

### <a name="response"></a><span data-ttu-id="44653-339">Resposta</span><span class="sxs-lookup"><span data-stu-id="44653-339">Response</span></span>
<span data-ttu-id="44653-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44653-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3318

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
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
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true
}
```





