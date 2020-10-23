---
title: Criar macOSGeneralDeviceConfiguration
description: Cria um novo objeto macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ee139961988844061258f23f611a2c300464ff55
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724828"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="2f358-103">Criar macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f358-103">Create macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="2f358-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f358-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f358-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f358-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f358-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f358-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f358-107">Cria um novo objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f358-107">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f358-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f358-108">Prerequisites</span></span>
<span data-ttu-id="2f358-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f358-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f358-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f358-111">Permission type</span></span>|<span data-ttu-id="2f358-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f358-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f358-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f358-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f358-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f358-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f358-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f358-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f358-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f358-116">Not supported.</span></span>|
|<span data-ttu-id="2f358-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f358-117">Application</span></span>|<span data-ttu-id="2f358-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f358-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f358-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f358-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2f358-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f358-120">Request headers</span></span>
|<span data-ttu-id="2f358-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f358-121">Header</span></span>|<span data-ttu-id="2f358-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2f358-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f358-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f358-123">Authorization</span></span>|<span data-ttu-id="2f358-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f358-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f358-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f358-125">Accept</span></span>|<span data-ttu-id="2f358-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f358-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f358-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f358-127">Request body</span></span>
<span data-ttu-id="2f358-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2f358-128">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="2f358-129">A tabela a seguir mostra as propriedades obrigatórias ao criar macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2f358-129">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="2f358-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f358-130">Property</span></span>|<span data-ttu-id="2f358-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f358-131">Type</span></span>|<span data-ttu-id="2f358-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f358-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f358-133">id</span><span class="sxs-lookup"><span data-stu-id="2f358-133">id</span></span>|<span data-ttu-id="2f358-134">String</span><span class="sxs-lookup"><span data-stu-id="2f358-134">String</span></span>|<span data-ttu-id="2f358-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2f358-135">Key of the entity.</span></span> <span data-ttu-id="2f358-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f358-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f358-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f358-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2f358-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f358-138">DateTimeOffset</span></span>|<span data-ttu-id="2f358-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2f358-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2f358-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f358-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f358-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2f358-141">roleScopeTagIds</span></span>|<span data-ttu-id="2f358-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f358-142">String collection</span></span>|<span data-ttu-id="2f358-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="2f358-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2f358-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f358-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f358-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2f358-145">supportsScopeTags</span></span>|<span data-ttu-id="2f358-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-146">Boolean</span></span>|<span data-ttu-id="2f358-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="2f358-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2f358-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="2f358-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2f358-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="2f358-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2f358-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f358-150">This property is read-only.</span></span> <span data-ttu-id="2f358-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f358-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f358-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2f358-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2f358-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2f358-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2f358-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="2f358-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2f358-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f358-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f358-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2f358-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2f358-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2f358-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2f358-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="2f358-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2f358-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f358-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f358-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2f358-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2f358-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2f358-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2f358-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="2f358-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2f358-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f358-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f358-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f358-164">createdDateTime</span></span>|<span data-ttu-id="2f358-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f358-165">DateTimeOffset</span></span>|<span data-ttu-id="2f358-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2f358-166">DateTime the object was created.</span></span> <span data-ttu-id="2f358-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f358-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f358-168">description</span><span class="sxs-lookup"><span data-stu-id="2f358-168">description</span></span>|<span data-ttu-id="2f358-169">String</span><span class="sxs-lookup"><span data-stu-id="2f358-169">String</span></span>|<span data-ttu-id="2f358-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f358-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2f358-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f358-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f358-172">displayName</span><span class="sxs-lookup"><span data-stu-id="2f358-172">displayName</span></span>|<span data-ttu-id="2f358-173">String</span><span class="sxs-lookup"><span data-stu-id="2f358-173">String</span></span>|<span data-ttu-id="2f358-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f358-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2f358-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f358-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f358-176">versão</span><span class="sxs-lookup"><span data-stu-id="2f358-176">version</span></span>|<span data-ttu-id="2f358-177">Int32</span><span class="sxs-lookup"><span data-stu-id="2f358-177">Int32</span></span>|<span data-ttu-id="2f358-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f358-178">Version of the device configuration.</span></span> <span data-ttu-id="2f358-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f358-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f358-180">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="2f358-180">compliantAppsList</span></span>|<span data-ttu-id="2f358-181">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="2f358-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="2f358-182">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="2f358-182">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="2f358-183">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="2f358-183">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="2f358-184">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="2f358-184">compliantAppListType</span></span>|[<span data-ttu-id="2f358-185">appListType</span><span class="sxs-lookup"><span data-stu-id="2f358-185">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="2f358-186">Lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="2f358-186">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="2f358-187">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="2f358-187">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="2f358-188">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="2f358-188">emailInDomainSuffixes</span></span>|<span data-ttu-id="2f358-189">String collection</span><span class="sxs-lookup"><span data-stu-id="2f358-189">String collection</span></span>|<span data-ttu-id="2f358-190">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="2f358-190">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="2f358-191">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="2f358-191">passwordBlockSimple</span></span>|<span data-ttu-id="2f358-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f358-192">Boolean</span></span>|<span data-ttu-id="2f358-193">Bloquear senhas simples.</span><span class="sxs-lookup"><span data-stu-id="2f358-193">Block simple passwords.</span></span>|
|<span data-ttu-id="2f358-194">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2f358-194">passwordExpirationDays</span></span>|<span data-ttu-id="2f358-195">Int32</span><span class="sxs-lookup"><span data-stu-id="2f358-195">Int32</span></span>|<span data-ttu-id="2f358-196">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="2f358-196">Number of days before the password expires.</span></span>|
|<span data-ttu-id="2f358-197">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="2f358-197">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="2f358-198">Int32</span><span class="sxs-lookup"><span data-stu-id="2f358-198">Int32</span></span>|<span data-ttu-id="2f358-199">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="2f358-199">Number of character sets a password must contain.</span></span> <span data-ttu-id="2f358-200">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="2f358-200">Valid values 0 to 4</span></span>|
|<span data-ttu-id="2f358-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2f358-201">passwordMinimumLength</span></span>|<span data-ttu-id="2f358-202">Int32</span><span class="sxs-lookup"><span data-stu-id="2f358-202">Int32</span></span>|<span data-ttu-id="2f358-203">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="2f358-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="2f358-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="2f358-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="2f358-205">Int32</span><span class="sxs-lookup"><span data-stu-id="2f358-205">Int32</span></span>|<span data-ttu-id="2f358-206">Minutos de inatividade necessários antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="2f358-206">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="2f358-207">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="2f358-207">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="2f358-208">Int32</span><span class="sxs-lookup"><span data-stu-id="2f358-208">Int32</span></span>|<span data-ttu-id="2f358-209">Minutos de inatividade necessários antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="2f358-209">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="2f358-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2f358-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2f358-211">Int32</span><span class="sxs-lookup"><span data-stu-id="2f358-211">Int32</span></span>|<span data-ttu-id="2f358-212">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="2f358-212">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="2f358-213">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2f358-213">passwordRequiredType</span></span>|[<span data-ttu-id="2f358-214">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2f358-214">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="2f358-215">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="2f358-215">Type of password that is required.</span></span> <span data-ttu-id="2f358-216">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="2f358-216">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="2f358-217">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="2f358-217">passwordRequired</span></span>|<span data-ttu-id="2f358-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f358-218">Boolean</span></span>|<span data-ttu-id="2f358-219">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="2f358-219">Whether or not to require a password.</span></span>|
|<span data-ttu-id="2f358-220">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="2f358-220">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="2f358-221">Int32</span><span class="sxs-lookup"><span data-stu-id="2f358-221">Int32</span></span>|<span data-ttu-id="2f358-222">O número de tentativas com falha de tentativa de inserir a senha na tela de bloqueio do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f358-222">The number of allowed failed attempts to enter the passcode at the device's lock screen.</span></span> <span data-ttu-id="2f358-223">Valores válidos de 2 a 11</span><span class="sxs-lookup"><span data-stu-id="2f358-223">Valid values 2 to 11</span></span>|
|<span data-ttu-id="2f358-224">passwordMinutesUntilFailedLoginReset</span><span class="sxs-lookup"><span data-stu-id="2f358-224">passwordMinutesUntilFailedLoginReset</span></span>|<span data-ttu-id="2f358-225">Int32</span><span class="sxs-lookup"><span data-stu-id="2f358-225">Int32</span></span>|<span data-ttu-id="2f358-226">O número de minutos antes do logon ser redefinido após o número máximo de tentativas de logon malsucedidas ser atingido.</span><span class="sxs-lookup"><span data-stu-id="2f358-226">The number of minutes before the login is reset after the maximum number of unsuccessful login attempts is reached.</span></span>|
|<span data-ttu-id="2f358-227">Propriedadeskeychainblockcloudsync</span><span class="sxs-lookup"><span data-stu-id="2f358-227">keychainBlockCloudSync</span></span>|<span data-ttu-id="2f358-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-228">Boolean</span></span>|<span data-ttu-id="2f358-229">Indica se a sincronização de chaves do iCloud está bloqueada (macOS 10,12 e posterior).</span><span class="sxs-lookup"><span data-stu-id="2f358-229">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="2f358-230">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="2f358-230">airPrintBlocked</span></span>|<span data-ttu-id="2f358-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-231">Boolean</span></span>|<span data-ttu-id="2f358-232">Indica se o arquivo de impressão está bloqueado (macOS 10,12 e posterior).</span><span class="sxs-lookup"><span data-stu-id="2f358-232">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="2f358-233">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="2f358-233">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="2f358-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-234">Boolean</span></span>|<span data-ttu-id="2f358-235">Indica se certificados confiáveis são necessários para comunicação de impressão TLS (macOS 10,13 e posterior).</span><span class="sxs-lookup"><span data-stu-id="2f358-235">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="2f358-236">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="2f358-236">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="2f358-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-237">Boolean</span></span>|<span data-ttu-id="2f358-238">Indica se a descoberta de impressoras de impressão do iBeacon está ou não bloqueada.</span><span class="sxs-lookup"><span data-stu-id="2f358-238">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="2f358-239">Isso impede os beacons Bluetooth de impressão de mensagens de phishing para tráfego de rede (macOS 10,3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="2f358-239">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="2f358-240">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="2f358-240">safariBlockAutofill</span></span>|<span data-ttu-id="2f358-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f358-241">Boolean</span></span>|<span data-ttu-id="2f358-242">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="2f358-242">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="2f358-243">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="2f358-243">cameraBlocked</span></span>|<span data-ttu-id="2f358-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f358-244">Boolean</span></span>|<span data-ttu-id="2f358-245">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f358-245">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="2f358-246">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="2f358-246">iTunesBlockMusicService</span></span>|<span data-ttu-id="2f358-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f358-247">Boolean</span></span>|<span data-ttu-id="2f358-248">Indica se o serviço de música deve ou não ser bloqueado e o aplicativo de música é revertido para o modo clássico.</span><span class="sxs-lookup"><span data-stu-id="2f358-248">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="2f358-249">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="2f358-249">spotlightBlockInternetResults</span></span>|<span data-ttu-id="2f358-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f358-250">Boolean</span></span>|<span data-ttu-id="2f358-251">Indica se o Spotlight deve ou não bloquear o retorno de qualquer resultado de uma pesquisa na Internet.</span><span class="sxs-lookup"><span data-stu-id="2f358-251">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="2f358-252">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="2f358-252">keyboardBlockDictation</span></span>|<span data-ttu-id="2f358-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f358-253">Boolean</span></span>|<span data-ttu-id="2f358-254">Indica se o usuário será ou não impedido de usar a entrada de ditado.</span><span class="sxs-lookup"><span data-stu-id="2f358-254">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="2f358-255">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="2f358-255">definitionLookupBlocked</span></span>|<span data-ttu-id="2f358-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f358-256">Boolean</span></span>|<span data-ttu-id="2f358-257">Indica se a pesquisa de definição deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="2f358-257">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="2f358-258">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="2f358-258">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="2f358-259">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-259">Boolean</span></span>|<span data-ttu-id="2f358-260">Indica se os usuários devem ou não bloquear seu Mac com o Apple Watch.</span><span class="sxs-lookup"><span data-stu-id="2f358-260">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="2f358-261">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="2f358-261">iTunesBlockFileSharing</span></span>|<span data-ttu-id="2f358-262">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-262">Boolean</span></span>|<span data-ttu-id="2f358-263">Indica se os arquivos devem ou não ser transferidos usando o iTunes.</span><span class="sxs-lookup"><span data-stu-id="2f358-263">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="2f358-264">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="2f358-264">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="2f358-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f358-265">Boolean</span></span>|<span data-ttu-id="2f358-266">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="2f358-266">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="2f358-267">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="2f358-267">iCloudBlockMail</span></span>|<span data-ttu-id="2f358-268">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-268">Boolean</span></span>|<span data-ttu-id="2f358-269">Indica se o iCloud deve ou não bloquear emails de sincronização.</span><span class="sxs-lookup"><span data-stu-id="2f358-269">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="2f358-270">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="2f358-270">iCloudBlockAddressBook</span></span>|<span data-ttu-id="2f358-271">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-271">Boolean</span></span>|<span data-ttu-id="2f358-272">Indica se o iCloud deve ou não bloquear os contatos de sincronização.</span><span class="sxs-lookup"><span data-stu-id="2f358-272">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="2f358-273">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="2f358-273">iCloudBlockCalendar</span></span>|<span data-ttu-id="2f358-274">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-274">Boolean</span></span>|<span data-ttu-id="2f358-275">Indica se o iCloud deve ou não bloquear calendários de sincronização.</span><span class="sxs-lookup"><span data-stu-id="2f358-275">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="2f358-276">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="2f358-276">iCloudBlockReminders</span></span>|<span data-ttu-id="2f358-277">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-277">Boolean</span></span>|<span data-ttu-id="2f358-278">Indica se o iCloud deve ou não bloquear lembretes de sincronização.</span><span class="sxs-lookup"><span data-stu-id="2f358-278">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="2f358-279">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="2f358-279">iCloudBlockBookmarks</span></span>|<span data-ttu-id="2f358-280">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-280">Boolean</span></span>|<span data-ttu-id="2f358-281">Indica se o iCloud deve ou não bloquear os indicadores de sincronização.</span><span class="sxs-lookup"><span data-stu-id="2f358-281">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="2f358-282">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="2f358-282">iCloudBlockNotes</span></span>|<span data-ttu-id="2f358-283">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-283">Boolean</span></span>|<span data-ttu-id="2f358-284">Indica se o iCloud deve ou não bloquear as anotações de sincronização.</span><span class="sxs-lookup"><span data-stu-id="2f358-284">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="2f358-285">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="2f358-285">airDropBlocked</span></span>|<span data-ttu-id="2f358-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f358-286">Boolean</span></span>|<span data-ttu-id="2f358-287">Indica se o recurso de recebimento de esficado deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="2f358-287">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="2f358-288">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="2f358-288">passwordBlockModification</span></span>|<span data-ttu-id="2f358-289">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-289">Boolean</span></span>|<span data-ttu-id="2f358-290">Indica se a modificação de senha deve ou não ser permitida.</span><span class="sxs-lookup"><span data-stu-id="2f358-290">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="2f358-291">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="2f358-291">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="2f358-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f358-292">Boolean</span></span>|<span data-ttu-id="2f358-293">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="2f358-293">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="2f358-294">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="2f358-294">passwordBlockAutoFill</span></span>|<span data-ttu-id="2f358-295">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-295">Boolean</span></span>|<span data-ttu-id="2f358-296">Indica se o recurso de senhas de preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="2f358-296">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="2f358-297">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="2f358-297">passwordBlockProximityRequests</span></span>|<span data-ttu-id="2f358-298">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-298">Boolean</span></span>|<span data-ttu-id="2f358-299">Indica se as senhas de solicitação devem ou não ser bloqueadas de dispositivos próximos.</span><span class="sxs-lookup"><span data-stu-id="2f358-299">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="2f358-300">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="2f358-300">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="2f358-301">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-301">Boolean</span></span>|<span data-ttu-id="2f358-302">Indica se as senhas de compartilhamento devem ou não ser bloqueadas com o recurso de senha de soltura.</span><span class="sxs-lookup"><span data-stu-id="2f358-302">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="2f358-303">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="2f358-303">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="2f358-304">Int32</span><span class="sxs-lookup"><span data-stu-id="2f358-304">Int32</span></span>|<span data-ttu-id="2f358-305">Define o número de dias que uma atualização de software será delyed para um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="2f358-305">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="2f358-306">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="2f358-306">Valid values 0 to 90</span></span>|
|<span data-ttu-id="2f358-307">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="2f358-307">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="2f358-308">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-308">Boolean</span></span>|<span data-ttu-id="2f358-309">Indica se o usuário deve ou não atrasar a visibilidade de atualizações de software quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="2f358-309">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="2f358-310">updateDelayPolicy</span><span class="sxs-lookup"><span data-stu-id="2f358-310">updateDelayPolicy</span></span>|[<span data-ttu-id="2f358-311">macOSSoftwareUpdateDelayPolicy</span><span class="sxs-lookup"><span data-stu-id="2f358-311">macOSSoftwareUpdateDelayPolicy</span></span>](../resources/intune-deviceconfig-macossoftwareupdatedelaypolicy.md)|<span data-ttu-id="2f358-312">Determina se deve atrasar as atualizações de sistema operacional e/ou aplicativo para o macOS.</span><span class="sxs-lookup"><span data-stu-id="2f358-312">Determines whether to delay OS and/or app updates for macOS.</span></span> <span data-ttu-id="2f358-313">Os valores possíveis são: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`.</span><span class="sxs-lookup"><span data-stu-id="2f358-313">Possible values are: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`.</span></span>|
|<span data-ttu-id="2f358-314">contentCachingBlocked</span><span class="sxs-lookup"><span data-stu-id="2f358-314">contentCachingBlocked</span></span>|<span data-ttu-id="2f358-315">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-315">Boolean</span></span>|<span data-ttu-id="2f358-316">Indica se o cache de conteúdo deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="2f358-316">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="2f358-317">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="2f358-317">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="2f358-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f358-318">Boolean</span></span>|<span data-ttu-id="2f358-319">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="2f358-319">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="2f358-320">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="2f358-320">screenCaptureBlocked</span></span>|<span data-ttu-id="2f358-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f358-321">Boolean</span></span>|<span data-ttu-id="2f358-322">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="2f358-322">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="2f358-323">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="2f358-323">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="2f358-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f358-324">Boolean</span></span>|<span data-ttu-id="2f358-325">Indica se a observação de tela remota deve ou não ser permitida por aplicativo de sala de aula.</span><span class="sxs-lookup"><span data-stu-id="2f358-325">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="2f358-326">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="2f358-326">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="2f358-327">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="2f358-327">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="2f358-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f358-328">Boolean</span></span>|<span data-ttu-id="2f358-329">Indica se a permissão será ou não automaticamente para o professor de um curso gerenciado no aplicativo da sala de aula para exibir a tela de um aluno sem avisar.</span><span class="sxs-lookup"><span data-stu-id="2f358-329">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="2f358-330">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="2f358-330">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="2f358-331">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="2f358-331">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="2f358-332">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-332">Boolean</span></span>|<span data-ttu-id="2f358-333">Indica se a permissão será ou não automaticamente para as solicitações do professor, sem avisar o aluno.</span><span class="sxs-lookup"><span data-stu-id="2f358-333">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="2f358-334">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="2f358-334">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="2f358-335">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="2f358-335">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="2f358-336">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-336">Boolean</span></span>|<span data-ttu-id="2f358-337">Indica se um aluno inscrito em um curso não gerenciado via sala de aula será solicitado a solicitar permissão do professor ao tentar sair do curso.</span><span class="sxs-lookup"><span data-stu-id="2f358-337">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="2f358-338">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="2f358-338">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="2f358-339">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="2f358-339">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="2f358-340">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f358-340">Boolean</span></span>|<span data-ttu-id="2f358-341">Indica se o professor deve ou não bloquear aplicativos ou o dispositivo sem avisar o aluno.</span><span class="sxs-lookup"><span data-stu-id="2f358-341">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="2f358-342">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="2f358-342">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="2f358-343">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="2f358-343">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="2f358-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f358-344">Boolean</span></span>|<span data-ttu-id="2f358-345">Indica se o usuário será ou não impedido de continuar o trabalho que iniciou em um dispositivo MacOS em outro dispositivo iOS ou MacOS (MacOS 10,15 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="2f358-345">Indicates whether or not to block the user from continuing work that they started on a MacOS device on another iOS or MacOS device (MacOS 10.15 or later).</span></span>|
|<span data-ttu-id="2f358-346">privacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="2f358-346">privacyAccessControls</span></span>|<span data-ttu-id="2f358-347">coleção [macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md)</span><span class="sxs-lookup"><span data-stu-id="2f358-347">[macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="2f358-348">Lista de controles de política de preferência de privacidade.</span><span class="sxs-lookup"><span data-stu-id="2f358-348">List of privacy preference policy controls.</span></span> <span data-ttu-id="2f358-349">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="2f358-349">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="2f358-350">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f358-350">Response</span></span>
<span data-ttu-id="2f358-351">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f358-351">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f358-352">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f358-352">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f358-353">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f358-353">Request</span></span>
<span data-ttu-id="2f358-354">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f358-354">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4680

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
  "softwareUpdatesForceDelayed": true,
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

### <a name="response"></a><span data-ttu-id="2f358-355">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f358-355">Response</span></span>
<span data-ttu-id="2f358-p127">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f358-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4852

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
  "softwareUpdatesForceDelayed": true,
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





