---
title: Criar macOSGeneralDeviceConfiguration
description: Cria um novo objeto macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 343798542aab40e769b18cf8e4a33993d40af3f2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137256"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="97421-103">Criar macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="97421-103">Create macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="97421-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97421-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97421-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="97421-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97421-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="97421-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97421-107">Cria um novo objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97421-107">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97421-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97421-108">Prerequisites</span></span>
<span data-ttu-id="97421-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97421-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97421-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97421-111">Permission type</span></span>|<span data-ttu-id="97421-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97421-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97421-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97421-113">Delegated (work or school account)</span></span>|<span data-ttu-id="97421-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97421-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="97421-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97421-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97421-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97421-116">Not supported.</span></span>|
|<span data-ttu-id="97421-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97421-117">Application</span></span>|<span data-ttu-id="97421-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97421-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97421-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97421-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="97421-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97421-120">Request headers</span></span>
|<span data-ttu-id="97421-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97421-121">Header</span></span>|<span data-ttu-id="97421-122">Valor</span><span class="sxs-lookup"><span data-stu-id="97421-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97421-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="97421-123">Authorization</span></span>|<span data-ttu-id="97421-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97421-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97421-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="97421-125">Accept</span></span>|<span data-ttu-id="97421-126">application/json</span><span class="sxs-lookup"><span data-stu-id="97421-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97421-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97421-127">Request body</span></span>
<span data-ttu-id="97421-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="97421-128">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="97421-129">A tabela a seguir mostra as propriedades obrigatórias ao criar macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="97421-129">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="97421-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97421-130">Property</span></span>|<span data-ttu-id="97421-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="97421-131">Type</span></span>|<span data-ttu-id="97421-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="97421-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97421-133">id</span><span class="sxs-lookup"><span data-stu-id="97421-133">id</span></span>|<span data-ttu-id="97421-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97421-134">String</span></span>|<span data-ttu-id="97421-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="97421-135">Key of the entity.</span></span> <span data-ttu-id="97421-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97421-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97421-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97421-137">lastModifiedDateTime</span></span>|<span data-ttu-id="97421-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97421-138">DateTimeOffset</span></span>|<span data-ttu-id="97421-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="97421-139">DateTime the object was last modified.</span></span> <span data-ttu-id="97421-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97421-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97421-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="97421-141">roleScopeTagIds</span></span>|<span data-ttu-id="97421-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="97421-142">String collection</span></span>|<span data-ttu-id="97421-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="97421-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="97421-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97421-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97421-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="97421-145">supportsScopeTags</span></span>|<span data-ttu-id="97421-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-146">Boolean</span></span>|<span data-ttu-id="97421-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="97421-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="97421-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="97421-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="97421-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="97421-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="97421-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="97421-150">This property is read-only.</span></span> <span data-ttu-id="97421-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97421-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97421-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="97421-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="97421-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="97421-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="97421-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="97421-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="97421-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97421-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97421-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="97421-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="97421-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="97421-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="97421-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="97421-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="97421-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97421-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97421-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="97421-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="97421-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="97421-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="97421-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="97421-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="97421-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97421-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97421-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97421-164">createdDateTime</span></span>|<span data-ttu-id="97421-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97421-165">DateTimeOffset</span></span>|<span data-ttu-id="97421-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="97421-166">DateTime the object was created.</span></span> <span data-ttu-id="97421-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97421-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97421-168">descrição</span><span class="sxs-lookup"><span data-stu-id="97421-168">description</span></span>|<span data-ttu-id="97421-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97421-169">String</span></span>|<span data-ttu-id="97421-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97421-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="97421-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97421-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97421-172">displayName</span><span class="sxs-lookup"><span data-stu-id="97421-172">displayName</span></span>|<span data-ttu-id="97421-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97421-173">String</span></span>|<span data-ttu-id="97421-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97421-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="97421-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97421-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97421-176">versão</span><span class="sxs-lookup"><span data-stu-id="97421-176">version</span></span>|<span data-ttu-id="97421-177">Int32</span><span class="sxs-lookup"><span data-stu-id="97421-177">Int32</span></span>|<span data-ttu-id="97421-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97421-178">Version of the device configuration.</span></span> <span data-ttu-id="97421-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97421-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97421-180">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="97421-180">compliantAppsList</span></span>|<span data-ttu-id="97421-181">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="97421-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="97421-182">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="97421-182">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="97421-183">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="97421-183">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="97421-184">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="97421-184">compliantAppListType</span></span>|[<span data-ttu-id="97421-185">appListType</span><span class="sxs-lookup"><span data-stu-id="97421-185">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="97421-186">Lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="97421-186">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="97421-187">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="97421-187">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="97421-188">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="97421-188">emailInDomainSuffixes</span></span>|<span data-ttu-id="97421-189">String collection</span><span class="sxs-lookup"><span data-stu-id="97421-189">String collection</span></span>|<span data-ttu-id="97421-190">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="97421-190">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="97421-191">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="97421-191">passwordBlockSimple</span></span>|<span data-ttu-id="97421-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="97421-192">Boolean</span></span>|<span data-ttu-id="97421-193">Bloquear senhas simples.</span><span class="sxs-lookup"><span data-stu-id="97421-193">Block simple passwords.</span></span>|
|<span data-ttu-id="97421-194">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="97421-194">passwordExpirationDays</span></span>|<span data-ttu-id="97421-195">Int32</span><span class="sxs-lookup"><span data-stu-id="97421-195">Int32</span></span>|<span data-ttu-id="97421-196">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="97421-196">Number of days before the password expires.</span></span>|
|<span data-ttu-id="97421-197">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="97421-197">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="97421-198">Int32</span><span class="sxs-lookup"><span data-stu-id="97421-198">Int32</span></span>|<span data-ttu-id="97421-199">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="97421-199">Number of character sets a password must contain.</span></span> <span data-ttu-id="97421-200">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="97421-200">Valid values 0 to 4</span></span>|
|<span data-ttu-id="97421-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="97421-201">passwordMinimumLength</span></span>|<span data-ttu-id="97421-202">Int32</span><span class="sxs-lookup"><span data-stu-id="97421-202">Int32</span></span>|<span data-ttu-id="97421-203">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="97421-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="97421-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="97421-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="97421-205">Int32</span><span class="sxs-lookup"><span data-stu-id="97421-205">Int32</span></span>|<span data-ttu-id="97421-206">Minutos de inatividade necessários antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="97421-206">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="97421-207">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="97421-207">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="97421-208">Int32</span><span class="sxs-lookup"><span data-stu-id="97421-208">Int32</span></span>|<span data-ttu-id="97421-209">Minutos de inatividade necessários antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="97421-209">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="97421-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="97421-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="97421-211">Int32</span><span class="sxs-lookup"><span data-stu-id="97421-211">Int32</span></span>|<span data-ttu-id="97421-212">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="97421-212">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="97421-213">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="97421-213">passwordRequiredType</span></span>|[<span data-ttu-id="97421-214">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="97421-214">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="97421-215">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="97421-215">Type of password that is required.</span></span> <span data-ttu-id="97421-216">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="97421-216">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="97421-217">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="97421-217">passwordRequired</span></span>|<span data-ttu-id="97421-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="97421-218">Boolean</span></span>|<span data-ttu-id="97421-219">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="97421-219">Whether or not to require a password.</span></span>|
|<span data-ttu-id="97421-220">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="97421-220">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="97421-221">Int32</span><span class="sxs-lookup"><span data-stu-id="97421-221">Int32</span></span>|<span data-ttu-id="97421-222">O número de tentativas de falha permitidas para inserir a senha na tela de bloqueio do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97421-222">The number of allowed failed attempts to enter the passcode at the device's lock screen.</span></span> <span data-ttu-id="97421-223">Valores válidos de 2 a 11</span><span class="sxs-lookup"><span data-stu-id="97421-223">Valid values 2 to 11</span></span>|
|<span data-ttu-id="97421-224">passwordMinutesUntilFailedLoginReset</span><span class="sxs-lookup"><span data-stu-id="97421-224">passwordMinutesUntilFailedLoginReset</span></span>|<span data-ttu-id="97421-225">Int32</span><span class="sxs-lookup"><span data-stu-id="97421-225">Int32</span></span>|<span data-ttu-id="97421-226">O número de minutos antes de o logon ser redefinido depois que o número máximo de tentativas de logon malsucedida é atingido.</span><span class="sxs-lookup"><span data-stu-id="97421-226">The number of minutes before the login is reset after the maximum number of unsuccessful login attempts is reached.</span></span>|
|<span data-ttu-id="97421-227">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="97421-227">keychainBlockCloudSync</span></span>|<span data-ttu-id="97421-228">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-228">Boolean</span></span>|<span data-ttu-id="97421-229">Indica se a sincronização do chaveiro do iCloud está bloqueada ou não (macOS 10.12 e posterior).</span><span class="sxs-lookup"><span data-stu-id="97421-229">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="97421-230">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="97421-230">airPrintBlocked</span></span>|<span data-ttu-id="97421-231">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-231">Boolean</span></span>|<span data-ttu-id="97421-232">Indica se o AirPrint está bloqueado ou não (macOS 10.12 e posterior).</span><span class="sxs-lookup"><span data-stu-id="97421-232">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="97421-233">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="97421-233">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="97421-234">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-234">Boolean</span></span>|<span data-ttu-id="97421-235">Indica se certificados confiáveis são necessários para comunicação de impressão TLS (macOS 10.13 e posterior).</span><span class="sxs-lookup"><span data-stu-id="97421-235">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="97421-236">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="97421-236">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="97421-237">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-237">Boolean</span></span>|<span data-ttu-id="97421-238">Indica se a descoberta iBeacon ou não de impressoras AirPrint está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="97421-238">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="97421-239">Isso impede que os sinalizadores airPrint Bluetooth phishing para tráfego de rede (macOS 10.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="97421-239">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="97421-240">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="97421-240">safariBlockAutofill</span></span>|<span data-ttu-id="97421-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="97421-241">Boolean</span></span>|<span data-ttu-id="97421-242">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="97421-242">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="97421-243">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="97421-243">cameraBlocked</span></span>|<span data-ttu-id="97421-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="97421-244">Boolean</span></span>|<span data-ttu-id="97421-245">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97421-245">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="97421-246">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="97421-246">iTunesBlockMusicService</span></span>|<span data-ttu-id="97421-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="97421-247">Boolean</span></span>|<span data-ttu-id="97421-248">Indica se o serviço música deve ou não ser bloqueado e reverter o aplicativo música para o modo clássico.</span><span class="sxs-lookup"><span data-stu-id="97421-248">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="97421-249">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="97421-249">spotlightBlockInternetResults</span></span>|<span data-ttu-id="97421-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="97421-250">Boolean</span></span>|<span data-ttu-id="97421-251">Indica se o Destaque deve ou não ser bloqueado de retornar quaisquer resultados de uma pesquisa na Internet.</span><span class="sxs-lookup"><span data-stu-id="97421-251">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="97421-252">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="97421-252">keyboardBlockDictation</span></span>|<span data-ttu-id="97421-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="97421-253">Boolean</span></span>|<span data-ttu-id="97421-254">Indica se o usuário deve ou não bloquear o uso da entrada de ditado.</span><span class="sxs-lookup"><span data-stu-id="97421-254">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="97421-255">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="97421-255">definitionLookupBlocked</span></span>|<span data-ttu-id="97421-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="97421-256">Boolean</span></span>|<span data-ttu-id="97421-257">Indica se a pesquisa de definição deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="97421-257">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="97421-258">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="97421-258">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="97421-259">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-259">Boolean</span></span>|<span data-ttu-id="97421-260">Indica se os usuários podem ou não bloquear o desbloqueio do Mac com o Apple Watch.</span><span class="sxs-lookup"><span data-stu-id="97421-260">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="97421-261">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="97421-261">iTunesBlockFileSharing</span></span>|<span data-ttu-id="97421-262">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-262">Boolean</span></span>|<span data-ttu-id="97421-263">Indica se os arquivos serão ou não bloqueados de serem transferidos usando o iTunes.</span><span class="sxs-lookup"><span data-stu-id="97421-263">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="97421-264">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="97421-264">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="97421-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="97421-265">Boolean</span></span>|<span data-ttu-id="97421-266">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="97421-266">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="97421-267">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="97421-267">iCloudBlockMail</span></span>|<span data-ttu-id="97421-268">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-268">Boolean</span></span>|<span data-ttu-id="97421-269">Indica se o iCloud deve ou não ser bloqueado da sincronização de emails.</span><span class="sxs-lookup"><span data-stu-id="97421-269">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="97421-270">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="97421-270">iCloudBlockAddressBook</span></span>|<span data-ttu-id="97421-271">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-271">Boolean</span></span>|<span data-ttu-id="97421-272">Indica se o iCloud deve ou não impedir a sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="97421-272">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="97421-273">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="97421-273">iCloudBlockCalendar</span></span>|<span data-ttu-id="97421-274">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-274">Boolean</span></span>|<span data-ttu-id="97421-275">Indica se o iCloud deve ou não bloquear a sincronização de calendários.</span><span class="sxs-lookup"><span data-stu-id="97421-275">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="97421-276">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="97421-276">iCloudBlockReminders</span></span>|<span data-ttu-id="97421-277">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-277">Boolean</span></span>|<span data-ttu-id="97421-278">Indica se o iCloud deve ou não bloquear a sincronização de lembretes.</span><span class="sxs-lookup"><span data-stu-id="97421-278">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="97421-279">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="97421-279">iCloudBlockBookmarks</span></span>|<span data-ttu-id="97421-280">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-280">Boolean</span></span>|<span data-ttu-id="97421-281">Indica se o iCloud deve ou não ser bloqueado da sincronização de indicadores.</span><span class="sxs-lookup"><span data-stu-id="97421-281">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="97421-282">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="97421-282">iCloudBlockNotes</span></span>|<span data-ttu-id="97421-283">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-283">Boolean</span></span>|<span data-ttu-id="97421-284">Indica se o iCloud deve ou não bloquear a sincronização de anotações.</span><span class="sxs-lookup"><span data-stu-id="97421-284">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="97421-285">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="97421-285">airDropBlocked</span></span>|<span data-ttu-id="97421-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="97421-286">Boolean</span></span>|<span data-ttu-id="97421-287">Indica se o AirDrop permitirá ou não.</span><span class="sxs-lookup"><span data-stu-id="97421-287">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="97421-288">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="97421-288">passwordBlockModification</span></span>|<span data-ttu-id="97421-289">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-289">Boolean</span></span>|<span data-ttu-id="97421-290">Indica se a modificação da senha deve ou não ser possível.</span><span class="sxs-lookup"><span data-stu-id="97421-290">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="97421-291">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="97421-291">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="97421-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="97421-292">Boolean</span></span>|<span data-ttu-id="97421-293">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="97421-293">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="97421-294">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="97421-294">passwordBlockAutoFill</span></span>|<span data-ttu-id="97421-295">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-295">Boolean</span></span>|<span data-ttu-id="97421-296">Indica se o recurso Senhas de Preenchimento Automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="97421-296">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="97421-297">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="97421-297">passwordBlockProximityRequests</span></span>|<span data-ttu-id="97421-298">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-298">Boolean</span></span>|<span data-ttu-id="97421-299">Indica se deve ou não bloquear a solicitação de senhas de dispositivos próximos.</span><span class="sxs-lookup"><span data-stu-id="97421-299">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="97421-300">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="97421-300">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="97421-301">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-301">Boolean</span></span>|<span data-ttu-id="97421-302">Indica se deve ou não bloquear o compartilhamento de senhas com o recurso de senhas do AirDrop.</span><span class="sxs-lookup"><span data-stu-id="97421-302">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="97421-303">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="97421-303">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="97421-304">Int32</span><span class="sxs-lookup"><span data-stu-id="97421-304">Int32</span></span>|<span data-ttu-id="97421-305">Define quantos dias uma atualização de software será usada para um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="97421-305">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="97421-306">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="97421-306">Valid values 0 to 90</span></span>|
|<span data-ttu-id="97421-307">updateDelayPolicy</span><span class="sxs-lookup"><span data-stu-id="97421-307">updateDelayPolicy</span></span>|[<span data-ttu-id="97421-308">macOSSoftwareUpdateDelayPolicy</span><span class="sxs-lookup"><span data-stu-id="97421-308">macOSSoftwareUpdateDelayPolicy</span></span>](../resources/intune-deviceconfig-macossoftwareupdatedelaypolicy.md)|<span data-ttu-id="97421-309">Determina se as atualizações do sistema operacional e/ou do aplicativo são demoradas para macOS.</span><span class="sxs-lookup"><span data-stu-id="97421-309">Determines whether to delay OS and/or app updates for macOS.</span></span> <span data-ttu-id="97421-310">Os valores possíveis são: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`.</span><span class="sxs-lookup"><span data-stu-id="97421-310">Possible values are: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`.</span></span>|
|<span data-ttu-id="97421-311">contentCachingBlocked</span><span class="sxs-lookup"><span data-stu-id="97421-311">contentCachingBlocked</span></span>|<span data-ttu-id="97421-312">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-312">Boolean</span></span>|<span data-ttu-id="97421-313">Indica se é ou não para permitir o cache de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="97421-313">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="97421-314">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="97421-314">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="97421-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="97421-315">Boolean</span></span>|<span data-ttu-id="97421-316">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="97421-316">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="97421-317">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="97421-317">screenCaptureBlocked</span></span>|<span data-ttu-id="97421-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="97421-318">Boolean</span></span>|<span data-ttu-id="97421-319">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="97421-319">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="97421-320">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="97421-320">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="97421-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="97421-321">Boolean</span></span>|<span data-ttu-id="97421-322">Indica se a observação de tela remota deve ou não ser permitida pelo aplicativo Classroom.</span><span class="sxs-lookup"><span data-stu-id="97421-322">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="97421-323">Requer o registro MDM por meio do Apple School Manager ou do Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="97421-323">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="97421-324">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="97421-324">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="97421-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="97421-325">Boolean</span></span>|<span data-ttu-id="97421-326">Indica se o professor de um curso gerenciado no aplicativo Classroom deve ou não dar permissão ao professor para exibir a tela de um aluno sem solicitar.</span><span class="sxs-lookup"><span data-stu-id="97421-326">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="97421-327">Requer o registro MDM por meio do Apple School Manager ou do Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="97421-327">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="97421-328">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="97421-328">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="97421-329">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-329">Boolean</span></span>|<span data-ttu-id="97421-330">Indica se o aluno deve ou não dar permissão automaticamente às solicitações do professor, sem solicitar ao aluno.</span><span class="sxs-lookup"><span data-stu-id="97421-330">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="97421-331">Requer o registro MDM por meio do Apple School Manager ou do Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="97421-331">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="97421-332">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="97421-332">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="97421-333">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-333">Boolean</span></span>|<span data-ttu-id="97421-334">Indica se um aluno matriculado em um curso não organizado via Sala de Aula será necessário para solicitar permissão do professor ao tentar sair do curso.</span><span class="sxs-lookup"><span data-stu-id="97421-334">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="97421-335">Requer o registro MDM por meio do Apple School Manager ou do Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="97421-335">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="97421-336">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="97421-336">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="97421-337">Booleano</span><span class="sxs-lookup"><span data-stu-id="97421-337">Boolean</span></span>|<span data-ttu-id="97421-338">Indica se o professor deve ou não permitir que o professor bloqueie aplicativos ou o dispositivo sem solicitar ao aluno.</span><span class="sxs-lookup"><span data-stu-id="97421-338">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="97421-339">Requer o registro MDM por meio do Apple School Manager ou do Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="97421-339">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="97421-340">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="97421-340">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="97421-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="97421-341">Boolean</span></span>|<span data-ttu-id="97421-342">Indica se o usuário deve ou não bloquear o trabalho contínuo iniciado em um dispositivo MacOS em outro dispositivo iOS ou MacOS (MacOS 10.15 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="97421-342">Indicates whether or not to block the user from continuing work that they started on a MacOS device on another iOS or MacOS device (MacOS 10.15 or later).</span></span>|
|<span data-ttu-id="97421-343">privacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="97421-343">privacyAccessControls</span></span>|<span data-ttu-id="97421-344">[Coleção macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md)</span><span class="sxs-lookup"><span data-stu-id="97421-344">[macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="97421-345">Lista de controles de política de preferência de privacidade.</span><span class="sxs-lookup"><span data-stu-id="97421-345">List of privacy preference policy controls.</span></span> <span data-ttu-id="97421-346">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="97421-346">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="97421-347">Resposta</span><span class="sxs-lookup"><span data-stu-id="97421-347">Response</span></span>
<span data-ttu-id="97421-348">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97421-348">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97421-349">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97421-349">Example</span></span>

### <a name="request"></a><span data-ttu-id="97421-350">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97421-350">Request</span></span>
<span data-ttu-id="97421-351">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97421-351">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4640

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
  "passwordMaximumAttemptCount": 11,
  "passwordMinutesUntilFailedLoginReset": 4,
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
  "updateDelayPolicy": "delayOSUpdateVisibility",
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true,
  "privacyAccessControls": [
    {
      "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem",
      "displayName": "Display Name value",
      "identifier": "Identifier value",
      "identifierType": "path",
      "codeRequirement": "Code Requirement value",
      "staticCodeValidation": true,
      "blockCamera": true,
      "blockMicrophone": true,
      "blockScreenCapture": true,
      "blockListenEvent": true,
      "speechRecognition": "enabled",
      "accessibility": "enabled",
      "addressBook": "enabled",
      "calendar": "enabled",
      "reminders": "enabled",
      "photos": "enabled",
      "mediaLibrary": "enabled",
      "fileProviderPresence": "enabled",
      "systemPolicyAllFiles": "enabled",
      "systemPolicySystemAdminFiles": "enabled",
      "systemPolicyDesktopFolder": "enabled",
      "systemPolicyDocumentsFolder": "enabled",
      "systemPolicyDownloadsFolder": "enabled",
      "systemPolicyNetworkVolumes": "enabled",
      "systemPolicyRemovableVolumes": "enabled",
      "postEvent": "enabled",
      "appleEventsAllowedReceivers": [
        {
          "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
          "codeRequirement": "Code Requirement value",
          "identifier": "Identifier value",
          "identifierType": "path",
          "allowed": true
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="97421-352">Resposta</span><span class="sxs-lookup"><span data-stu-id="97421-352">Response</span></span>
<span data-ttu-id="97421-p127">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97421-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4812

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
  "passwordMaximumAttemptCount": 11,
  "passwordMinutesUntilFailedLoginReset": 4,
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
  "updateDelayPolicy": "delayOSUpdateVisibility",
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true,
  "privacyAccessControls": [
    {
      "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem",
      "displayName": "Display Name value",
      "identifier": "Identifier value",
      "identifierType": "path",
      "codeRequirement": "Code Requirement value",
      "staticCodeValidation": true,
      "blockCamera": true,
      "blockMicrophone": true,
      "blockScreenCapture": true,
      "blockListenEvent": true,
      "speechRecognition": "enabled",
      "accessibility": "enabled",
      "addressBook": "enabled",
      "calendar": "enabled",
      "reminders": "enabled",
      "photos": "enabled",
      "mediaLibrary": "enabled",
      "fileProviderPresence": "enabled",
      "systemPolicyAllFiles": "enabled",
      "systemPolicySystemAdminFiles": "enabled",
      "systemPolicyDesktopFolder": "enabled",
      "systemPolicyDocumentsFolder": "enabled",
      "systemPolicyDownloadsFolder": "enabled",
      "systemPolicyNetworkVolumes": "enabled",
      "systemPolicyRemovableVolumes": "enabled",
      "postEvent": "enabled",
      "appleEventsAllowedReceivers": [
        {
          "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
          "codeRequirement": "Code Requirement value",
          "identifier": "Identifier value",
          "identifierType": "path",
          "allowed": true
        }
      ]
    }
  ]
}
```




