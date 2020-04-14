---
title: Atualizar macOSGeneralDeviceConfiguration
description: Atualiza as propriedades de um objeto macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 697b952af6227114ecd967b1597cac674688e208
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432588"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="ed77b-103">Atualizar macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="ed77b-103">Update macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="ed77b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed77b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed77b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ed77b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed77b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed77b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed77b-107">Atualiza as propriedades de um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed77b-107">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed77b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed77b-108">Prerequisites</span></span>
<span data-ttu-id="ed77b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed77b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed77b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed77b-111">Permission type</span></span>|<span data-ttu-id="ed77b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ed77b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed77b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed77b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed77b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed77b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ed77b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed77b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed77b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed77b-116">Not supported.</span></span>|
|<span data-ttu-id="ed77b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed77b-117">Application</span></span>|<span data-ttu-id="ed77b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed77b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed77b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed77b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ed77b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed77b-120">Request headers</span></span>
|<span data-ttu-id="ed77b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed77b-121">Header</span></span>|<span data-ttu-id="ed77b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ed77b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed77b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed77b-123">Authorization</span></span>|<span data-ttu-id="ed77b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed77b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed77b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ed77b-125">Accept</span></span>|<span data-ttu-id="ed77b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed77b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed77b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed77b-127">Request body</span></span>
<span data-ttu-id="ed77b-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed77b-128">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="ed77b-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed77b-129">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="ed77b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed77b-130">Property</span></span>|<span data-ttu-id="ed77b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed77b-131">Type</span></span>|<span data-ttu-id="ed77b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed77b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed77b-133">id</span><span class="sxs-lookup"><span data-stu-id="ed77b-133">id</span></span>|<span data-ttu-id="ed77b-134">String</span><span class="sxs-lookup"><span data-stu-id="ed77b-134">String</span></span>|<span data-ttu-id="ed77b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ed77b-135">Key of the entity.</span></span> <span data-ttu-id="ed77b-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed77b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed77b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed77b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ed77b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed77b-138">DateTimeOffset</span></span>|<span data-ttu-id="ed77b-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ed77b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ed77b-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed77b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed77b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ed77b-141">roleScopeTagIds</span></span>|<span data-ttu-id="ed77b-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="ed77b-142">String collection</span></span>|<span data-ttu-id="ed77b-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="ed77b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ed77b-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed77b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed77b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ed77b-145">supportsScopeTags</span></span>|<span data-ttu-id="ed77b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-146">Boolean</span></span>|<span data-ttu-id="ed77b-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ed77b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ed77b-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ed77b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ed77b-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ed77b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ed77b-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed77b-150">This property is read-only.</span></span> <span data-ttu-id="ed77b-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed77b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed77b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ed77b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ed77b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ed77b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ed77b-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="ed77b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ed77b-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed77b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed77b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ed77b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ed77b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ed77b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ed77b-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="ed77b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ed77b-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed77b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed77b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ed77b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ed77b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ed77b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ed77b-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="ed77b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ed77b-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed77b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed77b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed77b-164">createdDateTime</span></span>|<span data-ttu-id="ed77b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed77b-165">DateTimeOffset</span></span>|<span data-ttu-id="ed77b-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ed77b-166">DateTime the object was created.</span></span> <span data-ttu-id="ed77b-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed77b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed77b-168">description</span><span class="sxs-lookup"><span data-stu-id="ed77b-168">description</span></span>|<span data-ttu-id="ed77b-169">String</span><span class="sxs-lookup"><span data-stu-id="ed77b-169">String</span></span>|<span data-ttu-id="ed77b-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ed77b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ed77b-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed77b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed77b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ed77b-172">displayName</span></span>|<span data-ttu-id="ed77b-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed77b-173">String</span></span>|<span data-ttu-id="ed77b-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ed77b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ed77b-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed77b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed77b-176">versão</span><span class="sxs-lookup"><span data-stu-id="ed77b-176">version</span></span>|<span data-ttu-id="ed77b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ed77b-177">Int32</span></span>|<span data-ttu-id="ed77b-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ed77b-178">Version of the device configuration.</span></span> <span data-ttu-id="ed77b-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed77b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed77b-180">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="ed77b-180">compliantAppsList</span></span>|<span data-ttu-id="ed77b-181">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ed77b-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ed77b-182">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="ed77b-182">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="ed77b-183">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="ed77b-183">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ed77b-184">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="ed77b-184">compliantAppListType</span></span>|[<span data-ttu-id="ed77b-185">appListType</span><span class="sxs-lookup"><span data-stu-id="ed77b-185">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="ed77b-186">Lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="ed77b-186">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="ed77b-187">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="ed77b-187">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="ed77b-188">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="ed77b-188">emailInDomainSuffixes</span></span>|<span data-ttu-id="ed77b-189">String collection</span><span class="sxs-lookup"><span data-stu-id="ed77b-189">String collection</span></span>|<span data-ttu-id="ed77b-190">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="ed77b-190">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="ed77b-191">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="ed77b-191">passwordBlockSimple</span></span>|<span data-ttu-id="ed77b-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="ed77b-192">Boolean</span></span>|<span data-ttu-id="ed77b-193">Bloquear senhas simples.</span><span class="sxs-lookup"><span data-stu-id="ed77b-193">Block simple passwords.</span></span>|
|<span data-ttu-id="ed77b-194">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ed77b-194">passwordExpirationDays</span></span>|<span data-ttu-id="ed77b-195">Int32</span><span class="sxs-lookup"><span data-stu-id="ed77b-195">Int32</span></span>|<span data-ttu-id="ed77b-196">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="ed77b-196">Number of days before the password expires.</span></span>|
|<span data-ttu-id="ed77b-197">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ed77b-197">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="ed77b-198">Int32</span><span class="sxs-lookup"><span data-stu-id="ed77b-198">Int32</span></span>|<span data-ttu-id="ed77b-199">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="ed77b-199">Number of character sets a password must contain.</span></span> <span data-ttu-id="ed77b-200">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="ed77b-200">Valid values 0 to 4</span></span>|
|<span data-ttu-id="ed77b-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ed77b-201">passwordMinimumLength</span></span>|<span data-ttu-id="ed77b-202">Int32</span><span class="sxs-lookup"><span data-stu-id="ed77b-202">Int32</span></span>|<span data-ttu-id="ed77b-203">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="ed77b-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="ed77b-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ed77b-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ed77b-205">Int32</span><span class="sxs-lookup"><span data-stu-id="ed77b-205">Int32</span></span>|<span data-ttu-id="ed77b-206">Minutos de inatividade necessários antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="ed77b-206">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="ed77b-207">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="ed77b-207">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="ed77b-208">Int32</span><span class="sxs-lookup"><span data-stu-id="ed77b-208">Int32</span></span>|<span data-ttu-id="ed77b-209">Minutos de inatividade necessários antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="ed77b-209">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="ed77b-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ed77b-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ed77b-211">Int32</span><span class="sxs-lookup"><span data-stu-id="ed77b-211">Int32</span></span>|<span data-ttu-id="ed77b-212">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="ed77b-212">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="ed77b-213">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ed77b-213">passwordRequiredType</span></span>|[<span data-ttu-id="ed77b-214">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ed77b-214">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ed77b-215">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="ed77b-215">Type of password that is required.</span></span> <span data-ttu-id="ed77b-216">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="ed77b-216">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ed77b-217">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="ed77b-217">passwordRequired</span></span>|<span data-ttu-id="ed77b-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-218">Boolean</span></span>|<span data-ttu-id="ed77b-219">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="ed77b-219">Whether or not to require a password.</span></span>|
|<span data-ttu-id="ed77b-220">Propriedadeskeychainblockcloudsync</span><span class="sxs-lookup"><span data-stu-id="ed77b-220">keychainBlockCloudSync</span></span>|<span data-ttu-id="ed77b-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-221">Boolean</span></span>|<span data-ttu-id="ed77b-222">Indica se a sincronização de chaves do iCloud está bloqueada (macOS 10,12 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ed77b-222">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="ed77b-223">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="ed77b-223">airPrintBlocked</span></span>|<span data-ttu-id="ed77b-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-224">Boolean</span></span>|<span data-ttu-id="ed77b-225">Indica se o arquivo de impressão está bloqueado (macOS 10,12 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ed77b-225">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="ed77b-226">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="ed77b-226">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="ed77b-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-227">Boolean</span></span>|<span data-ttu-id="ed77b-228">Indica se certificados confiáveis são necessários para comunicação de impressão TLS (macOS 10,13 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ed77b-228">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="ed77b-229">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="ed77b-229">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="ed77b-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-230">Boolean</span></span>|<span data-ttu-id="ed77b-231">Indica se a descoberta de impressoras de impressão do iBeacon está ou não bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ed77b-231">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="ed77b-232">Isso impede os beacons Bluetooth de impressão de mensagens de phishing para tráfego de rede (macOS 10,3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ed77b-232">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="ed77b-233">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="ed77b-233">safariBlockAutofill</span></span>|<span data-ttu-id="ed77b-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-234">Boolean</span></span>|<span data-ttu-id="ed77b-235">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="ed77b-235">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="ed77b-236">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="ed77b-236">cameraBlocked</span></span>|<span data-ttu-id="ed77b-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-237">Boolean</span></span>|<span data-ttu-id="ed77b-238">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ed77b-238">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="ed77b-239">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="ed77b-239">iTunesBlockMusicService</span></span>|<span data-ttu-id="ed77b-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-240">Boolean</span></span>|<span data-ttu-id="ed77b-241">Indica se o serviço de música deve ou não ser bloqueado e o aplicativo de música é revertido para o modo clássico.</span><span class="sxs-lookup"><span data-stu-id="ed77b-241">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="ed77b-242">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="ed77b-242">spotlightBlockInternetResults</span></span>|<span data-ttu-id="ed77b-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-243">Boolean</span></span>|<span data-ttu-id="ed77b-244">Indica se o Spotlight deve ou não bloquear o retorno de qualquer resultado de uma pesquisa na Internet.</span><span class="sxs-lookup"><span data-stu-id="ed77b-244">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="ed77b-245">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="ed77b-245">keyboardBlockDictation</span></span>|<span data-ttu-id="ed77b-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-246">Boolean</span></span>|<span data-ttu-id="ed77b-247">Indica se o usuário será ou não impedido de usar a entrada de ditado.</span><span class="sxs-lookup"><span data-stu-id="ed77b-247">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="ed77b-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="ed77b-248">definitionLookupBlocked</span></span>|<span data-ttu-id="ed77b-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-249">Boolean</span></span>|<span data-ttu-id="ed77b-250">Indica se a pesquisa de definição deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ed77b-250">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="ed77b-251">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="ed77b-251">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="ed77b-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-252">Boolean</span></span>|<span data-ttu-id="ed77b-253">Indica se os usuários devem ou não bloquear seu Mac com o Apple Watch.</span><span class="sxs-lookup"><span data-stu-id="ed77b-253">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="ed77b-254">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="ed77b-254">iTunesBlockFileSharing</span></span>|<span data-ttu-id="ed77b-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-255">Boolean</span></span>|<span data-ttu-id="ed77b-256">Indica se os arquivos devem ou não ser transferidos usando o iTunes.</span><span class="sxs-lookup"><span data-stu-id="ed77b-256">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="ed77b-257">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="ed77b-257">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="ed77b-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-258">Boolean</span></span>|<span data-ttu-id="ed77b-259">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ed77b-259">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="ed77b-260">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="ed77b-260">iCloudBlockMail</span></span>|<span data-ttu-id="ed77b-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-261">Boolean</span></span>|<span data-ttu-id="ed77b-262">Indica se o iCloud deve ou não bloquear emails de sincronização.</span><span class="sxs-lookup"><span data-stu-id="ed77b-262">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="ed77b-263">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="ed77b-263">iCloudBlockAddressBook</span></span>|<span data-ttu-id="ed77b-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-264">Boolean</span></span>|<span data-ttu-id="ed77b-265">Indica se o iCloud deve ou não bloquear os contatos de sincronização.</span><span class="sxs-lookup"><span data-stu-id="ed77b-265">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="ed77b-266">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="ed77b-266">iCloudBlockCalendar</span></span>|<span data-ttu-id="ed77b-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-267">Boolean</span></span>|<span data-ttu-id="ed77b-268">Indica se o iCloud deve ou não bloquear calendários de sincronização.</span><span class="sxs-lookup"><span data-stu-id="ed77b-268">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="ed77b-269">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="ed77b-269">iCloudBlockReminders</span></span>|<span data-ttu-id="ed77b-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-270">Boolean</span></span>|<span data-ttu-id="ed77b-271">Indica se o iCloud deve ou não bloquear lembretes de sincronização.</span><span class="sxs-lookup"><span data-stu-id="ed77b-271">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="ed77b-272">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="ed77b-272">iCloudBlockBookmarks</span></span>|<span data-ttu-id="ed77b-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-273">Boolean</span></span>|<span data-ttu-id="ed77b-274">Indica se o iCloud deve ou não bloquear os indicadores de sincronização.</span><span class="sxs-lookup"><span data-stu-id="ed77b-274">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="ed77b-275">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="ed77b-275">iCloudBlockNotes</span></span>|<span data-ttu-id="ed77b-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-276">Boolean</span></span>|<span data-ttu-id="ed77b-277">Indica se o iCloud deve ou não bloquear as anotações de sincronização.</span><span class="sxs-lookup"><span data-stu-id="ed77b-277">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="ed77b-278">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="ed77b-278">airDropBlocked</span></span>|<span data-ttu-id="ed77b-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-279">Boolean</span></span>|<span data-ttu-id="ed77b-280">Indica se o recurso de recebimento de esficado deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="ed77b-280">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="ed77b-281">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="ed77b-281">passwordBlockModification</span></span>|<span data-ttu-id="ed77b-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-282">Boolean</span></span>|<span data-ttu-id="ed77b-283">Indica se a modificação de senha deve ou não ser permitida.</span><span class="sxs-lookup"><span data-stu-id="ed77b-283">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="ed77b-284">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="ed77b-284">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="ed77b-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-285">Boolean</span></span>|<span data-ttu-id="ed77b-286">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ed77b-286">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="ed77b-287">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="ed77b-287">passwordBlockAutoFill</span></span>|<span data-ttu-id="ed77b-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-288">Boolean</span></span>|<span data-ttu-id="ed77b-289">Indica se o recurso de senhas de preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ed77b-289">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="ed77b-290">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="ed77b-290">passwordBlockProximityRequests</span></span>|<span data-ttu-id="ed77b-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-291">Boolean</span></span>|<span data-ttu-id="ed77b-292">Indica se as senhas de solicitação devem ou não ser bloqueadas de dispositivos próximos.</span><span class="sxs-lookup"><span data-stu-id="ed77b-292">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="ed77b-293">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="ed77b-293">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="ed77b-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-294">Boolean</span></span>|<span data-ttu-id="ed77b-295">Indica se as senhas de compartilhamento devem ou não ser bloqueadas com o recurso de senha de soltura.</span><span class="sxs-lookup"><span data-stu-id="ed77b-295">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="ed77b-296">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="ed77b-296">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="ed77b-297">Int32</span><span class="sxs-lookup"><span data-stu-id="ed77b-297">Int32</span></span>|<span data-ttu-id="ed77b-298">Define o número de dias que uma atualização de software será delyed para um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ed77b-298">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="ed77b-299">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="ed77b-299">Valid values 0 to 90</span></span>|
|<span data-ttu-id="ed77b-300">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="ed77b-300">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="ed77b-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-301">Boolean</span></span>|<span data-ttu-id="ed77b-302">Indica se o usuário deve ou não atrasar a visibilidade de atualizações de software quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ed77b-302">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ed77b-303">contentCachingBlocked</span><span class="sxs-lookup"><span data-stu-id="ed77b-303">contentCachingBlocked</span></span>|<span data-ttu-id="ed77b-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-304">Boolean</span></span>|<span data-ttu-id="ed77b-305">Indica se o cache de conteúdo deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="ed77b-305">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="ed77b-306">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="ed77b-306">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="ed77b-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-307">Boolean</span></span>|<span data-ttu-id="ed77b-308">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ed77b-308">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="ed77b-309">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="ed77b-309">screenCaptureBlocked</span></span>|<span data-ttu-id="ed77b-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-310">Boolean</span></span>|<span data-ttu-id="ed77b-311">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="ed77b-311">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="ed77b-312">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="ed77b-312">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="ed77b-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-313">Boolean</span></span>|<span data-ttu-id="ed77b-314">Indica se a observação de tela remota deve ou não ser permitida por aplicativo de sala de aula.</span><span class="sxs-lookup"><span data-stu-id="ed77b-314">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="ed77b-315">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="ed77b-315">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="ed77b-316">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="ed77b-316">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="ed77b-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-317">Boolean</span></span>|<span data-ttu-id="ed77b-318">Indica se a permissão será ou não automaticamente para o professor de um curso gerenciado no aplicativo da sala de aula para exibir a tela de um aluno sem avisar.</span><span class="sxs-lookup"><span data-stu-id="ed77b-318">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="ed77b-319">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="ed77b-319">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="ed77b-320">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="ed77b-320">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="ed77b-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-321">Boolean</span></span>|<span data-ttu-id="ed77b-322">Indica se a permissão será ou não automaticamente para as solicitações do professor, sem avisar o aluno.</span><span class="sxs-lookup"><span data-stu-id="ed77b-322">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="ed77b-323">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="ed77b-323">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="ed77b-324">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="ed77b-324">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="ed77b-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-325">Boolean</span></span>|<span data-ttu-id="ed77b-326">Indica se um aluno inscrito em um curso não gerenciado via sala de aula será solicitado a solicitar permissão do professor ao tentar sair do curso.</span><span class="sxs-lookup"><span data-stu-id="ed77b-326">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="ed77b-327">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="ed77b-327">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="ed77b-328">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="ed77b-328">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="ed77b-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-329">Boolean</span></span>|<span data-ttu-id="ed77b-330">Indica se o professor deve ou não bloquear aplicativos ou o dispositivo sem avisar o aluno.</span><span class="sxs-lookup"><span data-stu-id="ed77b-330">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="ed77b-331">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="ed77b-331">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="ed77b-332">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="ed77b-332">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="ed77b-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77b-333">Boolean</span></span>|<span data-ttu-id="ed77b-334">Indica se o usuário será ou não impedido de continuar o trabalho que iniciou em um dispositivo MacOS em outro dispositivo iOS ou MacOS (MacOS 10,15 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ed77b-334">Indicates whether or not to block the user from continuing work that they started on a MacOS device on another iOS or MacOS device (MacOS 10.15 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="ed77b-335">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed77b-335">Response</span></span>
<span data-ttu-id="ed77b-336">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed77b-336">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed77b-337">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed77b-337">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed77b-338">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed77b-338">Request</span></span>
<span data-ttu-id="ed77b-339">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed77b-339">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="ed77b-340">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed77b-340">Response</span></span>
<span data-ttu-id="ed77b-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed77b-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



