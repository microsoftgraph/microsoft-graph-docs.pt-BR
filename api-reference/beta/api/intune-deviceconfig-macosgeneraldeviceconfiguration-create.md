---
title: Criar macOSGeneralDeviceConfiguration
description: Cria um novo objeto macOSGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0be9ed43a9557d3f4a94a58de80b7ea2f15b35a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34976705"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="6c385-103">Criar macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c385-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="6c385-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c385-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c385-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c385-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c385-106">Cria um novo objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c385-106">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c385-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c385-107">Prerequisites</span></span>
<span data-ttu-id="6c385-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c385-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c385-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c385-110">Permission type</span></span>|<span data-ttu-id="6c385-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6c385-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c385-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c385-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c385-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c385-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c385-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c385-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c385-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c385-115">Not supported.</span></span>|
|<span data-ttu-id="6c385-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c385-116">Application</span></span>|<span data-ttu-id="6c385-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c385-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c385-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c385-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6c385-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c385-119">Request headers</span></span>
|<span data-ttu-id="6c385-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c385-120">Header</span></span>|<span data-ttu-id="6c385-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6c385-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c385-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c385-122">Authorization</span></span>|<span data-ttu-id="6c385-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c385-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c385-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c385-124">Accept</span></span>|<span data-ttu-id="6c385-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6c385-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c385-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c385-126">Request body</span></span>
<span data-ttu-id="6c385-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6c385-127">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="6c385-128">A tabela a seguir mostra as propriedades obrigatórias ao criar macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6c385-128">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="6c385-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c385-129">Property</span></span>|<span data-ttu-id="6c385-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c385-130">Type</span></span>|<span data-ttu-id="6c385-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c385-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c385-132">id</span><span class="sxs-lookup"><span data-stu-id="6c385-132">id</span></span>|<span data-ttu-id="6c385-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c385-133">String</span></span>|<span data-ttu-id="6c385-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6c385-134">Key of the entity.</span></span> <span data-ttu-id="6c385-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c385-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c385-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c385-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6c385-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c385-137">DateTimeOffset</span></span>|<span data-ttu-id="6c385-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6c385-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6c385-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c385-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c385-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6c385-140">roleScopeTagIds</span></span>|<span data-ttu-id="6c385-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c385-141">String collection</span></span>|<span data-ttu-id="6c385-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6c385-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6c385-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c385-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c385-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6c385-144">supportsScopeTags</span></span>|<span data-ttu-id="6c385-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-145">Boolean</span></span>|<span data-ttu-id="6c385-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6c385-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6c385-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6c385-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6c385-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6c385-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6c385-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6c385-149">This property is read-only.</span></span> <span data-ttu-id="6c385-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c385-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c385-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6c385-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6c385-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6c385-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6c385-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="6c385-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6c385-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c385-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c385-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6c385-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6c385-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6c385-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6c385-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="6c385-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6c385-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c385-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c385-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6c385-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6c385-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6c385-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6c385-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="6c385-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6c385-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c385-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c385-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c385-163">createdDateTime</span></span>|<span data-ttu-id="6c385-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c385-164">DateTimeOffset</span></span>|<span data-ttu-id="6c385-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6c385-165">DateTime the object was created.</span></span> <span data-ttu-id="6c385-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c385-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c385-167">descrição</span><span class="sxs-lookup"><span data-stu-id="6c385-167">description</span></span>|<span data-ttu-id="6c385-168">String</span><span class="sxs-lookup"><span data-stu-id="6c385-168">String</span></span>|<span data-ttu-id="6c385-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c385-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6c385-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c385-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c385-171">displayName</span><span class="sxs-lookup"><span data-stu-id="6c385-171">displayName</span></span>|<span data-ttu-id="6c385-172">String</span><span class="sxs-lookup"><span data-stu-id="6c385-172">String</span></span>|<span data-ttu-id="6c385-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c385-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6c385-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c385-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c385-175">versão</span><span class="sxs-lookup"><span data-stu-id="6c385-175">version</span></span>|<span data-ttu-id="6c385-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6c385-176">Int32</span></span>|<span data-ttu-id="6c385-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c385-177">Version of the device configuration.</span></span> <span data-ttu-id="6c385-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c385-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c385-179">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="6c385-179">compliantAppsList</span></span>|<span data-ttu-id="6c385-180">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6c385-180">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6c385-181">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="6c385-181">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="6c385-182">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="6c385-182">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="6c385-183">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="6c385-183">compliantAppListType</span></span>|[<span data-ttu-id="6c385-184">appListType</span><span class="sxs-lookup"><span data-stu-id="6c385-184">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="6c385-185">Lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="6c385-185">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="6c385-186">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="6c385-186">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="6c385-187">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="6c385-187">emailInDomainSuffixes</span></span>|<span data-ttu-id="6c385-188">String collection</span><span class="sxs-lookup"><span data-stu-id="6c385-188">String collection</span></span>|<span data-ttu-id="6c385-189">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="6c385-189">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="6c385-190">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6c385-190">passwordBlockSimple</span></span>|<span data-ttu-id="6c385-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-191">Boolean</span></span>|<span data-ttu-id="6c385-192">Bloquear senhas simples.</span><span class="sxs-lookup"><span data-stu-id="6c385-192">Block simple passwords.</span></span>|
|<span data-ttu-id="6c385-193">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6c385-193">passwordExpirationDays</span></span>|<span data-ttu-id="6c385-194">Int32</span><span class="sxs-lookup"><span data-stu-id="6c385-194">Int32</span></span>|<span data-ttu-id="6c385-195">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="6c385-195">Number of days before the password expires.</span></span>|
|<span data-ttu-id="6c385-196">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6c385-196">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="6c385-197">Int32</span><span class="sxs-lookup"><span data-stu-id="6c385-197">Int32</span></span>|<span data-ttu-id="6c385-198">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="6c385-198">Number of character sets a password must contain.</span></span> <span data-ttu-id="6c385-199">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="6c385-199">Valid values 0 to 4</span></span>|
|<span data-ttu-id="6c385-200">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6c385-200">passwordMinimumLength</span></span>|<span data-ttu-id="6c385-201">Int32</span><span class="sxs-lookup"><span data-stu-id="6c385-201">Int32</span></span>|<span data-ttu-id="6c385-202">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="6c385-202">Minimum length of passwords.</span></span>|
|<span data-ttu-id="6c385-203">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6c385-203">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6c385-204">Int32</span><span class="sxs-lookup"><span data-stu-id="6c385-204">Int32</span></span>|<span data-ttu-id="6c385-205">Minutos de inatividade necessários antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="6c385-205">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="6c385-206">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6c385-206">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6c385-207">Int32</span><span class="sxs-lookup"><span data-stu-id="6c385-207">Int32</span></span>|<span data-ttu-id="6c385-208">Minutos de inatividade necessários antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="6c385-208">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="6c385-209">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6c385-209">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6c385-210">Int32</span><span class="sxs-lookup"><span data-stu-id="6c385-210">Int32</span></span>|<span data-ttu-id="6c385-211">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="6c385-211">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="6c385-212">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6c385-212">passwordRequiredType</span></span>|[<span data-ttu-id="6c385-213">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6c385-213">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6c385-214">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="6c385-214">Type of password that is required.</span></span> <span data-ttu-id="6c385-215">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="6c385-215">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6c385-216">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6c385-216">passwordRequired</span></span>|<span data-ttu-id="6c385-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c385-217">Boolean</span></span>|<span data-ttu-id="6c385-218">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="6c385-218">Whether or not to require a password.</span></span>|
|<span data-ttu-id="6c385-219">Propriedadeskeychainblockcloudsync</span><span class="sxs-lookup"><span data-stu-id="6c385-219">keychainBlockCloudSync</span></span>|<span data-ttu-id="6c385-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-220">Boolean</span></span>|<span data-ttu-id="6c385-221">Indica se a sincronização de chaves do iCloud está bloqueada (macOS 10,12 e posterior).</span><span class="sxs-lookup"><span data-stu-id="6c385-221">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="6c385-222">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="6c385-222">airPrintBlocked</span></span>|<span data-ttu-id="6c385-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-223">Boolean</span></span>|<span data-ttu-id="6c385-224">Indica se o arquivo de impressão está bloqueado (macOS 10,12 e posterior).</span><span class="sxs-lookup"><span data-stu-id="6c385-224">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="6c385-225">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="6c385-225">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="6c385-226">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-226">Boolean</span></span>|<span data-ttu-id="6c385-227">Indica se certificados confiáveis são necessários para comunicação de impressão TLS (macOS 10,13 e posterior).</span><span class="sxs-lookup"><span data-stu-id="6c385-227">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="6c385-228">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="6c385-228">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="6c385-229">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-229">Boolean</span></span>|<span data-ttu-id="6c385-230">Indica se a descoberta de impressoras de impressão do iBeacon está ou não bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6c385-230">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="6c385-231">Isso impede os beacons Bluetooth de impressão de mensagens de phishing para tráfego de rede (macOS 10,3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="6c385-231">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="6c385-232">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="6c385-232">safariBlockAutofill</span></span>|<span data-ttu-id="6c385-233">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-233">Boolean</span></span>|<span data-ttu-id="6c385-234">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="6c385-234">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="6c385-235">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="6c385-235">cameraBlocked</span></span>|<span data-ttu-id="6c385-236">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-236">Boolean</span></span>|<span data-ttu-id="6c385-237">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c385-237">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="6c385-238">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="6c385-238">iTunesBlockMusicService</span></span>|<span data-ttu-id="6c385-239">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-239">Boolean</span></span>|<span data-ttu-id="6c385-240">Indica se o serviço de música deve ou não ser bloqueado e o aplicativo de música é revertido para o modo clássico.</span><span class="sxs-lookup"><span data-stu-id="6c385-240">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="6c385-241">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="6c385-241">spotlightBlockInternetResults</span></span>|<span data-ttu-id="6c385-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c385-242">Boolean</span></span>|<span data-ttu-id="6c385-243">Indica se o Spotlight deve ou não bloquear o retorno de qualquer resultado de uma pesquisa na Internet.</span><span class="sxs-lookup"><span data-stu-id="6c385-243">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="6c385-244">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="6c385-244">keyboardBlockDictation</span></span>|<span data-ttu-id="6c385-245">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-245">Boolean</span></span>|<span data-ttu-id="6c385-246">Indica se o usuário será ou não impedido de usar a entrada de ditado.</span><span class="sxs-lookup"><span data-stu-id="6c385-246">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="6c385-247">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="6c385-247">definitionLookupBlocked</span></span>|<span data-ttu-id="6c385-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-248">Boolean</span></span>|<span data-ttu-id="6c385-249">Indica se a pesquisa de definição deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6c385-249">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="6c385-250">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="6c385-250">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="6c385-251">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-251">Boolean</span></span>|<span data-ttu-id="6c385-252">Indica se os usuários devem ou não bloquear seu Mac com o Apple Watch.</span><span class="sxs-lookup"><span data-stu-id="6c385-252">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="6c385-253">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="6c385-253">iTunesBlockFileSharing</span></span>|<span data-ttu-id="6c385-254">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-254">Boolean</span></span>|<span data-ttu-id="6c385-255">Indica se os arquivos devem ou não ser transferidos usando o iTunes.</span><span class="sxs-lookup"><span data-stu-id="6c385-255">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="6c385-256">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="6c385-256">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="6c385-257">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-257">Boolean</span></span>|<span data-ttu-id="6c385-258">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6c385-258">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="6c385-259">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="6c385-259">iCloudBlockMail</span></span>|<span data-ttu-id="6c385-260">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-260">Boolean</span></span>|<span data-ttu-id="6c385-261">Indica se o iCloud deve ou não bloquear emails de sincronização.</span><span class="sxs-lookup"><span data-stu-id="6c385-261">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="6c385-262">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="6c385-262">iCloudBlockAddressBook</span></span>|<span data-ttu-id="6c385-263">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-263">Boolean</span></span>|<span data-ttu-id="6c385-264">Indica se o iCloud deve ou não bloquear os contatos de sincronização.</span><span class="sxs-lookup"><span data-stu-id="6c385-264">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="6c385-265">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="6c385-265">iCloudBlockCalendar</span></span>|<span data-ttu-id="6c385-266">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-266">Boolean</span></span>|<span data-ttu-id="6c385-267">Indica se o iCloud deve ou não bloquear calendários de sincronização.</span><span class="sxs-lookup"><span data-stu-id="6c385-267">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="6c385-268">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="6c385-268">iCloudBlockReminders</span></span>|<span data-ttu-id="6c385-269">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-269">Boolean</span></span>|<span data-ttu-id="6c385-270">Indica se o iCloud deve ou não bloquear lembretes de sincronização.</span><span class="sxs-lookup"><span data-stu-id="6c385-270">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="6c385-271">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="6c385-271">iCloudBlockBookmarks</span></span>|<span data-ttu-id="6c385-272">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-272">Boolean</span></span>|<span data-ttu-id="6c385-273">Indica se o iCloud deve ou não bloquear os indicadores de sincronização.</span><span class="sxs-lookup"><span data-stu-id="6c385-273">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="6c385-274">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="6c385-274">iCloudBlockNotes</span></span>|<span data-ttu-id="6c385-275">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-275">Boolean</span></span>|<span data-ttu-id="6c385-276">Indica se o iCloud deve ou não bloquear as anotações de sincronização.</span><span class="sxs-lookup"><span data-stu-id="6c385-276">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="6c385-277">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="6c385-277">airDropBlocked</span></span>|<span data-ttu-id="6c385-278">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-278">Boolean</span></span>|<span data-ttu-id="6c385-279">Indica se o recurso de recebimento de esficado deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="6c385-279">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="6c385-280">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="6c385-280">passwordBlockModification</span></span>|<span data-ttu-id="6c385-281">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-281">Boolean</span></span>|<span data-ttu-id="6c385-282">Indica se a modificação de senha deve ou não ser permitida.</span><span class="sxs-lookup"><span data-stu-id="6c385-282">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="6c385-283">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="6c385-283">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="6c385-284">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-284">Boolean</span></span>|<span data-ttu-id="6c385-285">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6c385-285">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="6c385-286">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="6c385-286">passwordBlockAutoFill</span></span>|<span data-ttu-id="6c385-287">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-287">Boolean</span></span>|<span data-ttu-id="6c385-288">Indica se o recurso de senhas de preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6c385-288">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="6c385-289">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="6c385-289">passwordBlockProximityRequests</span></span>|<span data-ttu-id="6c385-290">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-290">Boolean</span></span>|<span data-ttu-id="6c385-291">Indica se as senhas de solicitação devem ou não ser bloqueadas de dispositivos próximos.</span><span class="sxs-lookup"><span data-stu-id="6c385-291">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="6c385-292">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="6c385-292">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="6c385-293">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-293">Boolean</span></span>|<span data-ttu-id="6c385-294">Indica se as senhas de compartilhamento devem ou não ser bloqueadas com o recurso de senha de soltura.</span><span class="sxs-lookup"><span data-stu-id="6c385-294">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="6c385-295">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="6c385-295">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="6c385-296">Int32</span><span class="sxs-lookup"><span data-stu-id="6c385-296">Int32</span></span>|<span data-ttu-id="6c385-297">Define o número de dias que uma atualização de software será delyed para um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6c385-297">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="6c385-298">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="6c385-298">Valid values 0 to 90</span></span>|
|<span data-ttu-id="6c385-299">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="6c385-299">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="6c385-300">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-300">Boolean</span></span>|<span data-ttu-id="6c385-301">Indica se o usuário deve ou não atrasar a visibilidade de atualizações de software quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6c385-301">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6c385-302">contentCachingBlocked</span><span class="sxs-lookup"><span data-stu-id="6c385-302">contentCachingBlocked</span></span>|<span data-ttu-id="6c385-303">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-303">Boolean</span></span>|<span data-ttu-id="6c385-304">Indica se o cache de conteúdo deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="6c385-304">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="6c385-305">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="6c385-305">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="6c385-306">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-306">Boolean</span></span>|<span data-ttu-id="6c385-307">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6c385-307">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="6c385-308">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="6c385-308">screenCaptureBlocked</span></span>|<span data-ttu-id="6c385-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c385-309">Boolean</span></span>|<span data-ttu-id="6c385-310">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="6c385-310">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="6c385-311">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="6c385-311">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="6c385-312">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-312">Boolean</span></span>|<span data-ttu-id="6c385-313">Indica se a observação de tela remota deve ou não ser permitida por aplicativo de sala de aula.</span><span class="sxs-lookup"><span data-stu-id="6c385-313">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="6c385-314">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="6c385-314">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="6c385-315">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="6c385-315">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="6c385-316">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-316">Boolean</span></span>|<span data-ttu-id="6c385-317">Indica se a permissão será ou não automaticamente para o professor de um curso gerenciado no aplicativo da sala de aula para exibir a tela de um aluno sem avisar.</span><span class="sxs-lookup"><span data-stu-id="6c385-317">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="6c385-318">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="6c385-318">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="6c385-319">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="6c385-319">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="6c385-320">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-320">Boolean</span></span>|<span data-ttu-id="6c385-321">Indica se a permissão será ou não automaticamente para as solicitações do professor, sem avisar o aluno.</span><span class="sxs-lookup"><span data-stu-id="6c385-321">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="6c385-322">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="6c385-322">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="6c385-323">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="6c385-323">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="6c385-324">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-324">Boolean</span></span>|<span data-ttu-id="6c385-325">Indica se um aluno inscrito em um curso não gerenciado via sala de aula será solicitado a solicitar permissão do professor ao tentar sair do curso.</span><span class="sxs-lookup"><span data-stu-id="6c385-325">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="6c385-326">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="6c385-326">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="6c385-327">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="6c385-327">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="6c385-328">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c385-328">Boolean</span></span>|<span data-ttu-id="6c385-329">Indica se o professor deve ou não bloquear aplicativos ou o dispositivo sem avisar o aluno.</span><span class="sxs-lookup"><span data-stu-id="6c385-329">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="6c385-330">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="6c385-330">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|



## <a name="response"></a><span data-ttu-id="6c385-331">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c385-331">Response</span></span>
<span data-ttu-id="6c385-332">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c385-332">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c385-333">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c385-333">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c385-334">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c385-334">Request</span></span>
<span data-ttu-id="6c385-335">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c385-335">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3102

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
  "classroomForceUnpromptedAppAndDeviceLock": true
}
```

### <a name="response"></a><span data-ttu-id="6c385-336">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c385-336">Response</span></span>
<span data-ttu-id="6c385-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c385-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3274

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
  "classroomForceUnpromptedAppAndDeviceLock": true
}
```





