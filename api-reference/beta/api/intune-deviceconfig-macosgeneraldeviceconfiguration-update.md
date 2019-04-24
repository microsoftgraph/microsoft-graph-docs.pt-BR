---
title: Atualizar macOSGeneralDeviceConfiguration
description: Atualiza as propriedades de um objeto macOSGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b58f7606909d5c40777ed37e4b5d49da39f76f0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518608"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="6a100-103">Atualizar macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="6a100-103">Update macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="6a100-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a100-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a100-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a100-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a100-106">Atualiza as propriedades de um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a100-106">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a100-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a100-107">Prerequisites</span></span>
<span data-ttu-id="6a100-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a100-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a100-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a100-110">Permission type</span></span>|<span data-ttu-id="6a100-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6a100-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a100-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a100-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a100-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a100-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6a100-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a100-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a100-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a100-115">Not supported.</span></span>|
|<span data-ttu-id="6a100-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a100-116">Application</span></span>|<span data-ttu-id="6a100-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a100-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a100-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a100-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6a100-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a100-119">Request headers</span></span>
|<span data-ttu-id="6a100-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a100-120">Header</span></span>|<span data-ttu-id="6a100-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6a100-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a100-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a100-122">Authorization</span></span>|<span data-ttu-id="6a100-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a100-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a100-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a100-124">Accept</span></span>|<span data-ttu-id="6a100-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a100-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a100-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a100-126">Request body</span></span>
<span data-ttu-id="6a100-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a100-127">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="6a100-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a100-128">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="6a100-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a100-129">Property</span></span>|<span data-ttu-id="6a100-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a100-130">Type</span></span>|<span data-ttu-id="6a100-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a100-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a100-132">id</span><span class="sxs-lookup"><span data-stu-id="6a100-132">id</span></span>|<span data-ttu-id="6a100-133">String</span><span class="sxs-lookup"><span data-stu-id="6a100-133">String</span></span>|<span data-ttu-id="6a100-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6a100-134">Key of the entity.</span></span> <span data-ttu-id="6a100-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a100-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a100-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a100-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6a100-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a100-137">DateTimeOffset</span></span>|<span data-ttu-id="6a100-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6a100-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6a100-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a100-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a100-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6a100-140">roleScopeTagIds</span></span>|<span data-ttu-id="6a100-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a100-141">String collection</span></span>|<span data-ttu-id="6a100-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6a100-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6a100-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a100-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a100-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6a100-144">supportsScopeTags</span></span>|<span data-ttu-id="6a100-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-145">Boolean</span></span>|<span data-ttu-id="6a100-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6a100-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6a100-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6a100-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6a100-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6a100-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6a100-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a100-149">This property is read-only.</span></span> <span data-ttu-id="6a100-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a100-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a100-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a100-151">createdDateTime</span></span>|<span data-ttu-id="6a100-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a100-152">DateTimeOffset</span></span>|<span data-ttu-id="6a100-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6a100-153">DateTime the object was created.</span></span> <span data-ttu-id="6a100-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a100-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a100-155">description</span><span class="sxs-lookup"><span data-stu-id="6a100-155">description</span></span>|<span data-ttu-id="6a100-156">String</span><span class="sxs-lookup"><span data-stu-id="6a100-156">String</span></span>|<span data-ttu-id="6a100-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a100-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6a100-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a100-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a100-159">displayName</span><span class="sxs-lookup"><span data-stu-id="6a100-159">displayName</span></span>|<span data-ttu-id="6a100-160">String</span><span class="sxs-lookup"><span data-stu-id="6a100-160">String</span></span>|<span data-ttu-id="6a100-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a100-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6a100-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a100-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a100-163">versão</span><span class="sxs-lookup"><span data-stu-id="6a100-163">version</span></span>|<span data-ttu-id="6a100-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6a100-164">Int32</span></span>|<span data-ttu-id="6a100-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a100-165">Version of the device configuration.</span></span> <span data-ttu-id="6a100-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a100-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a100-167">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="6a100-167">compliantAppsList</span></span>|<span data-ttu-id="6a100-168">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6a100-168">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6a100-169">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="6a100-169">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="6a100-170">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="6a100-170">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="6a100-171">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="6a100-171">compliantAppListType</span></span>|[<span data-ttu-id="6a100-172">appListType</span><span class="sxs-lookup"><span data-stu-id="6a100-172">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="6a100-173">Lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="6a100-173">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="6a100-174">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="6a100-174">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="6a100-175">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="6a100-175">emailInDomainSuffixes</span></span>|<span data-ttu-id="6a100-176">String collection</span><span class="sxs-lookup"><span data-stu-id="6a100-176">String collection</span></span>|<span data-ttu-id="6a100-177">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="6a100-177">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="6a100-178">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6a100-178">passwordBlockSimple</span></span>|<span data-ttu-id="6a100-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-179">Boolean</span></span>|<span data-ttu-id="6a100-180">Bloquear senhas simples.</span><span class="sxs-lookup"><span data-stu-id="6a100-180">Block simple passwords.</span></span>|
|<span data-ttu-id="6a100-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6a100-181">passwordExpirationDays</span></span>|<span data-ttu-id="6a100-182">Int32</span><span class="sxs-lookup"><span data-stu-id="6a100-182">Int32</span></span>|<span data-ttu-id="6a100-183">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="6a100-183">Number of days before the password expires.</span></span>|
|<span data-ttu-id="6a100-184">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6a100-184">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="6a100-185">Int32</span><span class="sxs-lookup"><span data-stu-id="6a100-185">Int32</span></span>|<span data-ttu-id="6a100-186">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="6a100-186">Number of character sets a password must contain.</span></span> <span data-ttu-id="6a100-187">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="6a100-187">Valid values 0 to 4</span></span>|
|<span data-ttu-id="6a100-188">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6a100-188">passwordMinimumLength</span></span>|<span data-ttu-id="6a100-189">Int32</span><span class="sxs-lookup"><span data-stu-id="6a100-189">Int32</span></span>|<span data-ttu-id="6a100-190">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="6a100-190">Minimum length of passwords.</span></span>|
|<span data-ttu-id="6a100-191">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6a100-191">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6a100-192">Int32</span><span class="sxs-lookup"><span data-stu-id="6a100-192">Int32</span></span>|<span data-ttu-id="6a100-193">Minutos de inatividade necessários antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="6a100-193">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="6a100-194">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6a100-194">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6a100-195">Int32</span><span class="sxs-lookup"><span data-stu-id="6a100-195">Int32</span></span>|<span data-ttu-id="6a100-196">Minutos de inatividade necessários antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="6a100-196">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="6a100-197">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6a100-197">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6a100-198">Int32</span><span class="sxs-lookup"><span data-stu-id="6a100-198">Int32</span></span>|<span data-ttu-id="6a100-199">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="6a100-199">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="6a100-200">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6a100-200">passwordRequiredType</span></span>|[<span data-ttu-id="6a100-201">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6a100-201">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6a100-202">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="6a100-202">Type of password that is required.</span></span> <span data-ttu-id="6a100-203">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="6a100-203">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6a100-204">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6a100-204">passwordRequired</span></span>|<span data-ttu-id="6a100-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a100-205">Boolean</span></span>|<span data-ttu-id="6a100-206">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="6a100-206">Whether or not to require a password.</span></span>|
|<span data-ttu-id="6a100-207">Propriedadeskeychainblockcloudsync</span><span class="sxs-lookup"><span data-stu-id="6a100-207">keychainBlockCloudSync</span></span>|<span data-ttu-id="6a100-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-208">Boolean</span></span>|<span data-ttu-id="6a100-209">Indica se a sincronização de chaves do iCloud está bloqueada (macOS 10,12 e posterior).</span><span class="sxs-lookup"><span data-stu-id="6a100-209">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="6a100-210">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="6a100-210">airPrintBlocked</span></span>|<span data-ttu-id="6a100-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-211">Boolean</span></span>|<span data-ttu-id="6a100-212">Indica se o arquivo de impressão está bloqueado (macOS 10,12 e posterior).</span><span class="sxs-lookup"><span data-stu-id="6a100-212">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="6a100-213">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="6a100-213">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="6a100-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-214">Boolean</span></span>|<span data-ttu-id="6a100-215">Indica se certificados confiáveis são necessários para comunicação de impressão TLS (macOS 10,13 e posterior).</span><span class="sxs-lookup"><span data-stu-id="6a100-215">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="6a100-216">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="6a100-216">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="6a100-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-217">Boolean</span></span>|<span data-ttu-id="6a100-218">Indica se a descoberta de impressoras de impressão do iBeacon está ou não bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6a100-218">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="6a100-219">Isso impede os beacons Bluetooth de impressão de mensagens de phishing para tráfego de rede (macOS 10,3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="6a100-219">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="6a100-220">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="6a100-220">safariBlockAutofill</span></span>|<span data-ttu-id="6a100-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-221">Boolean</span></span>|<span data-ttu-id="6a100-222">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="6a100-222">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="6a100-223">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="6a100-223">cameraBlocked</span></span>|<span data-ttu-id="6a100-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-224">Boolean</span></span>|<span data-ttu-id="6a100-225">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a100-225">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="6a100-226">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="6a100-226">iTunesBlockMusicService</span></span>|<span data-ttu-id="6a100-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-227">Boolean</span></span>|<span data-ttu-id="6a100-228">Indica se o serviço de música deve ou não ser bloqueado e o aplicativo de música é revertido para o modo clássico.</span><span class="sxs-lookup"><span data-stu-id="6a100-228">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="6a100-229">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="6a100-229">spotlightBlockInternetResults</span></span>|<span data-ttu-id="6a100-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a100-230">Boolean</span></span>|<span data-ttu-id="6a100-231">Indica se o Spotlight deve ou não bloquear o retorno de qualquer resultado de uma pesquisa na Internet.</span><span class="sxs-lookup"><span data-stu-id="6a100-231">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="6a100-232">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="6a100-232">keyboardBlockDictation</span></span>|<span data-ttu-id="6a100-233">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-233">Boolean</span></span>|<span data-ttu-id="6a100-234">Indica se o usuário será ou não impedido de usar a entrada de ditado.</span><span class="sxs-lookup"><span data-stu-id="6a100-234">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="6a100-235">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="6a100-235">definitionLookupBlocked</span></span>|<span data-ttu-id="6a100-236">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-236">Boolean</span></span>|<span data-ttu-id="6a100-237">Indica se a pesquisa de definição deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6a100-237">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="6a100-238">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="6a100-238">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="6a100-239">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-239">Boolean</span></span>|<span data-ttu-id="6a100-240">Indica se os usuários devem ou não bloquear seu Mac com o Apple Watch.</span><span class="sxs-lookup"><span data-stu-id="6a100-240">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="6a100-241">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="6a100-241">iTunesBlockFileSharing</span></span>|<span data-ttu-id="6a100-242">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-242">Boolean</span></span>|<span data-ttu-id="6a100-243">Indica se os arquivos devem ou não ser transferidos usando o iTunes.</span><span class="sxs-lookup"><span data-stu-id="6a100-243">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="6a100-244">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="6a100-244">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="6a100-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a100-245">Boolean</span></span>|<span data-ttu-id="6a100-246">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6a100-246">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="6a100-247">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="6a100-247">iCloudBlockMail</span></span>|<span data-ttu-id="6a100-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-248">Boolean</span></span>|<span data-ttu-id="6a100-249">Indica se o iCloud deve ou não bloquear emails de sincronização.</span><span class="sxs-lookup"><span data-stu-id="6a100-249">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="6a100-250">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="6a100-250">iCloudBlockAddressBook</span></span>|<span data-ttu-id="6a100-251">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-251">Boolean</span></span>|<span data-ttu-id="6a100-252">Indica se o iCloud deve ou não bloquear os contatos de sincronização.</span><span class="sxs-lookup"><span data-stu-id="6a100-252">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="6a100-253">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="6a100-253">iCloudBlockCalendar</span></span>|<span data-ttu-id="6a100-254">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-254">Boolean</span></span>|<span data-ttu-id="6a100-255">Indica se o iCloud deve ou não bloquear calendários de sincronização.</span><span class="sxs-lookup"><span data-stu-id="6a100-255">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="6a100-256">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="6a100-256">iCloudBlockReminders</span></span>|<span data-ttu-id="6a100-257">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-257">Boolean</span></span>|<span data-ttu-id="6a100-258">Indica se o iCloud deve ou não bloquear lembretes de sincronização.</span><span class="sxs-lookup"><span data-stu-id="6a100-258">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="6a100-259">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="6a100-259">iCloudBlockBookmarks</span></span>|<span data-ttu-id="6a100-260">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-260">Boolean</span></span>|<span data-ttu-id="6a100-261">Indica se o iCloud deve ou não bloquear os indicadores de sincronização.</span><span class="sxs-lookup"><span data-stu-id="6a100-261">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="6a100-262">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="6a100-262">iCloudBlockNotes</span></span>|<span data-ttu-id="6a100-263">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-263">Boolean</span></span>|<span data-ttu-id="6a100-264">Indica se o iCloud deve ou não bloquear as anotações de sincronização.</span><span class="sxs-lookup"><span data-stu-id="6a100-264">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="6a100-265">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="6a100-265">airDropBlocked</span></span>|<span data-ttu-id="6a100-266">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-266">Boolean</span></span>|<span data-ttu-id="6a100-267">Indica se o recurso de recebimento de esficado deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="6a100-267">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="6a100-268">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="6a100-268">passwordBlockModification</span></span>|<span data-ttu-id="6a100-269">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-269">Boolean</span></span>|<span data-ttu-id="6a100-270">Indica se a modificação de senha deve ou não ser permitida.</span><span class="sxs-lookup"><span data-stu-id="6a100-270">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="6a100-271">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="6a100-271">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="6a100-272">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-272">Boolean</span></span>|<span data-ttu-id="6a100-273">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6a100-273">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="6a100-274">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="6a100-274">passwordBlockAutoFill</span></span>|<span data-ttu-id="6a100-275">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-275">Boolean</span></span>|<span data-ttu-id="6a100-276">Indica se o recurso de senhas de preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6a100-276">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="6a100-277">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="6a100-277">passwordBlockProximityRequests</span></span>|<span data-ttu-id="6a100-278">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-278">Boolean</span></span>|<span data-ttu-id="6a100-279">Indica se as senhas de solicitação devem ou não ser bloqueadas de dispositivos próximos.</span><span class="sxs-lookup"><span data-stu-id="6a100-279">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="6a100-280">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="6a100-280">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="6a100-281">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-281">Boolean</span></span>|<span data-ttu-id="6a100-282">Indica se as senhas de compartilhamento devem ou não ser bloqueadas com o recurso de senha de soltura.</span><span class="sxs-lookup"><span data-stu-id="6a100-282">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="6a100-283">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="6a100-283">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="6a100-284">Int32</span><span class="sxs-lookup"><span data-stu-id="6a100-284">Int32</span></span>|<span data-ttu-id="6a100-285">Define o número de dias que uma atualização de software será delyed para um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6a100-285">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="6a100-286">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="6a100-286">Valid values 0 to 90</span></span>|
|<span data-ttu-id="6a100-287">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="6a100-287">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="6a100-288">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-288">Boolean</span></span>|<span data-ttu-id="6a100-289">Indica se o usuário deve ou não atrasar a visibilidade de atualizações de software quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6a100-289">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6a100-290">contentCachingBlocked</span><span class="sxs-lookup"><span data-stu-id="6a100-290">contentCachingBlocked</span></span>|<span data-ttu-id="6a100-291">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a100-291">Boolean</span></span>|<span data-ttu-id="6a100-292">Indica se o cache de conteúdo deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="6a100-292">Indicates whether or not to allow content caching.</span></span>|



## <a name="response"></a><span data-ttu-id="6a100-293">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a100-293">Response</span></span>
<span data-ttu-id="6a100-294">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a100-294">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a100-295">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a100-295">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a100-296">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a100-296">Request</span></span>
<span data-ttu-id="6a100-297">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a100-297">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1988

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "contentCachingBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="6a100-298">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a100-298">Response</span></span>
<span data-ttu-id="6a100-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a100-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2160

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "contentCachingBlocked": true
}
```





