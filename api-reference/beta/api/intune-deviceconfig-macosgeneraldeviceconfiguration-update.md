---
title: Atualizar macOSGeneralDeviceConfiguration
description: Atualiza as propriedades de um objeto macOSGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 90dd325d44cd0ac8577ce82aa97ff516180f9cc0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874099"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="80c76-103">Atualizar macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="80c76-103">Update macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="80c76-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="80c76-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80c76-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="80c76-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80c76-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="80c76-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80c76-107">Atualiza as propriedades de um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80c76-107">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="80c76-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="80c76-108">Prerequisites</span></span>
<span data-ttu-id="80c76-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80c76-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80c76-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80c76-111">Permission type</span></span>|<span data-ttu-id="80c76-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="80c76-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80c76-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80c76-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80c76-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80c76-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80c76-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80c76-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80c76-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80c76-116">Not supported.</span></span>|
|<span data-ttu-id="80c76-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80c76-117">Application</span></span>|<span data-ttu-id="80c76-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80c76-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80c76-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80c76-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="80c76-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80c76-120">Request headers</span></span>
|<span data-ttu-id="80c76-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80c76-121">Header</span></span>|<span data-ttu-id="80c76-122">Valor</span><span class="sxs-lookup"><span data-stu-id="80c76-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80c76-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="80c76-123">Authorization</span></span>|<span data-ttu-id="80c76-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80c76-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80c76-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="80c76-125">Accept</span></span>|<span data-ttu-id="80c76-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80c76-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80c76-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80c76-127">Request body</span></span>
<span data-ttu-id="80c76-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80c76-128">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="80c76-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80c76-129">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="80c76-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80c76-130">Property</span></span>|<span data-ttu-id="80c76-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="80c76-131">Type</span></span>|<span data-ttu-id="80c76-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="80c76-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80c76-133">id</span><span class="sxs-lookup"><span data-stu-id="80c76-133">id</span></span>|<span data-ttu-id="80c76-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80c76-134">String</span></span>|<span data-ttu-id="80c76-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="80c76-135">Key of the entity.</span></span> <span data-ttu-id="80c76-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80c76-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80c76-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80c76-137">lastModifiedDateTime</span></span>|<span data-ttu-id="80c76-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80c76-138">DateTimeOffset</span></span>|<span data-ttu-id="80c76-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="80c76-139">DateTime the object was last modified.</span></span> <span data-ttu-id="80c76-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80c76-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80c76-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="80c76-141">roleScopeTagIds</span></span>|<span data-ttu-id="80c76-142">String collection</span><span class="sxs-lookup"><span data-stu-id="80c76-142">String collection</span></span>|<span data-ttu-id="80c76-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="80c76-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="80c76-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80c76-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80c76-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="80c76-145">supportsScopeTags</span></span>|<span data-ttu-id="80c76-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-146">Boolean</span></span>|<span data-ttu-id="80c76-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="80c76-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="80c76-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="80c76-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="80c76-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="80c76-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="80c76-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80c76-150">This property is read-only.</span></span> <span data-ttu-id="80c76-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80c76-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80c76-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80c76-152">createdDateTime</span></span>|<span data-ttu-id="80c76-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80c76-153">DateTimeOffset</span></span>|<span data-ttu-id="80c76-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="80c76-154">DateTime the object was created.</span></span> <span data-ttu-id="80c76-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80c76-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80c76-156">description</span><span class="sxs-lookup"><span data-stu-id="80c76-156">description</span></span>|<span data-ttu-id="80c76-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80c76-157">String</span></span>|<span data-ttu-id="80c76-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80c76-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="80c76-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80c76-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80c76-160">displayName</span><span class="sxs-lookup"><span data-stu-id="80c76-160">displayName</span></span>|<span data-ttu-id="80c76-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80c76-161">String</span></span>|<span data-ttu-id="80c76-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80c76-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="80c76-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80c76-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80c76-164">version</span><span class="sxs-lookup"><span data-stu-id="80c76-164">version</span></span>|<span data-ttu-id="80c76-165">Int32</span><span class="sxs-lookup"><span data-stu-id="80c76-165">Int32</span></span>|<span data-ttu-id="80c76-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80c76-166">Version of the device configuration.</span></span> <span data-ttu-id="80c76-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80c76-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80c76-168">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="80c76-168">compliantAppsList</span></span>|<span data-ttu-id="80c76-169">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="80c76-169">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="80c76-170">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="80c76-170">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="80c76-171">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="80c76-171">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="80c76-172">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="80c76-172">compliantAppListType</span></span>|[<span data-ttu-id="80c76-173">appListType</span><span class="sxs-lookup"><span data-stu-id="80c76-173">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="80c76-174">Lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="80c76-174">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="80c76-175">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="80c76-175">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="80c76-176">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="80c76-176">emailInDomainSuffixes</span></span>|<span data-ttu-id="80c76-177">String collection</span><span class="sxs-lookup"><span data-stu-id="80c76-177">String collection</span></span>|<span data-ttu-id="80c76-178">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="80c76-178">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="80c76-179">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="80c76-179">passwordBlockSimple</span></span>|<span data-ttu-id="80c76-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-180">Boolean</span></span>|<span data-ttu-id="80c76-181">Bloquear senhas simples.</span><span class="sxs-lookup"><span data-stu-id="80c76-181">Block simple passwords.</span></span>|
|<span data-ttu-id="80c76-182">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="80c76-182">passwordExpirationDays</span></span>|<span data-ttu-id="80c76-183">Int32</span><span class="sxs-lookup"><span data-stu-id="80c76-183">Int32</span></span>|<span data-ttu-id="80c76-184">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="80c76-184">Number of days before the password expires.</span></span>|
|<span data-ttu-id="80c76-185">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="80c76-185">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="80c76-186">Int32</span><span class="sxs-lookup"><span data-stu-id="80c76-186">Int32</span></span>|<span data-ttu-id="80c76-187">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="80c76-187">Number of character sets a password must contain.</span></span> <span data-ttu-id="80c76-188">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="80c76-188">Valid values 0 to 4</span></span>|
|<span data-ttu-id="80c76-189">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="80c76-189">passwordMinimumLength</span></span>|<span data-ttu-id="80c76-190">Int32</span><span class="sxs-lookup"><span data-stu-id="80c76-190">Int32</span></span>|<span data-ttu-id="80c76-191">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="80c76-191">Minimum length of passwords.</span></span>|
|<span data-ttu-id="80c76-192">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="80c76-192">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="80c76-193">Int32</span><span class="sxs-lookup"><span data-stu-id="80c76-193">Int32</span></span>|<span data-ttu-id="80c76-194">Minutos de inatividade necessários antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="80c76-194">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="80c76-195">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="80c76-195">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="80c76-196">Int32</span><span class="sxs-lookup"><span data-stu-id="80c76-196">Int32</span></span>|<span data-ttu-id="80c76-197">Minutos de inatividade necessários antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="80c76-197">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="80c76-198">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="80c76-198">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="80c76-199">Int32</span><span class="sxs-lookup"><span data-stu-id="80c76-199">Int32</span></span>|<span data-ttu-id="80c76-200">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="80c76-200">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="80c76-201">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="80c76-201">passwordRequiredType</span></span>|[<span data-ttu-id="80c76-202">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="80c76-202">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="80c76-203">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="80c76-203">Type of password that is required.</span></span> <span data-ttu-id="80c76-204">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="80c76-204">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="80c76-205">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="80c76-205">passwordRequired</span></span>|<span data-ttu-id="80c76-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-206">Boolean</span></span>|<span data-ttu-id="80c76-207">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="80c76-207">Whether or not to require a password.</span></span>|
|<span data-ttu-id="80c76-208">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="80c76-208">keychainBlockCloudSync</span></span>|<span data-ttu-id="80c76-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-209">Boolean</span></span>|<span data-ttu-id="80c76-210">Indica se é ou não iCloud sincronização de conjunto de chaves bloqueado (macOS 10.12 e posterior).</span><span class="sxs-lookup"><span data-stu-id="80c76-210">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="80c76-211">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="80c76-211">airPrintBlocked</span></span>|<span data-ttu-id="80c76-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-212">Boolean</span></span>|<span data-ttu-id="80c76-213">Indica se é ou não AirPrint bloqueados (macOS 10.12 e posterior).</span><span class="sxs-lookup"><span data-stu-id="80c76-213">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="80c76-214">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="80c76-214">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="80c76-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-215">Boolean</span></span>|<span data-ttu-id="80c76-216">Indica se os certificados confiáveis são necessários para a comunicação de impressão de TLS (macOS 10.13 e posterior).</span><span class="sxs-lookup"><span data-stu-id="80c76-216">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="80c76-217">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="80c76-217">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="80c76-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-218">Boolean</span></span>|<span data-ttu-id="80c76-219">Indica se ou não iBeacon descoberta de impressoras AirPrint está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="80c76-219">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="80c76-220">Isso impede que os avisos de AirPrint Bluetooth artificiais contra phishing para tráfego de rede (macOS 10.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="80c76-220">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="80c76-221">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="80c76-221">safariBlockAutofill</span></span>|<span data-ttu-id="80c76-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-222">Boolean</span></span>|<span data-ttu-id="80c76-223">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="80c76-223">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="80c76-224">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="80c76-224">cameraBlocked</span></span>|<span data-ttu-id="80c76-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-225">Boolean</span></span>|<span data-ttu-id="80c76-226">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80c76-226">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="80c76-227">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="80c76-227">iTunesBlockMusicService</span></span>|<span data-ttu-id="80c76-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-228">Boolean</span></span>|<span data-ttu-id="80c76-229">Indica se ou não bloquear o serviço de música e reverter o aplicativo de música para modo clássico.</span><span class="sxs-lookup"><span data-stu-id="80c76-229">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="80c76-230">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="80c76-230">spotlightBlockInternetResults</span></span>|<span data-ttu-id="80c76-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-231">Boolean</span></span>|<span data-ttu-id="80c76-232">Indica se deve ou não bloquear destaque retornando todos os resultados de uma pesquisa na Internet.</span><span class="sxs-lookup"><span data-stu-id="80c76-232">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="80c76-233">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="80c76-233">keyboardBlockDictation</span></span>|<span data-ttu-id="80c76-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-234">Boolean</span></span>|<span data-ttu-id="80c76-235">Indica se deve ou não bloquear o usuário usando a entrada de ditado.</span><span class="sxs-lookup"><span data-stu-id="80c76-235">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="80c76-236">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="80c76-236">definitionLookupBlocked</span></span>|<span data-ttu-id="80c76-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-237">Boolean</span></span>|<span data-ttu-id="80c76-238">Indica se o bloqueio da pesquisa de definição ou não.</span><span class="sxs-lookup"><span data-stu-id="80c76-238">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="80c76-239">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="80c76-239">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="80c76-240">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-240">Boolean</span></span>|<span data-ttu-id="80c76-241">Indica se ou aos usuários de bloco de desbloquear sua Mac com Apple Watch.</span><span class="sxs-lookup"><span data-stu-id="80c76-241">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="80c76-242">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="80c76-242">iTunesBlockFileSharing</span></span>|<span data-ttu-id="80c76-243">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-243">Boolean</span></span>|<span data-ttu-id="80c76-244">Indica se ou não para bloquear arquivos do que está sendo transferido usando iTunes.</span><span class="sxs-lookup"><span data-stu-id="80c76-244">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="80c76-245">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="80c76-245">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="80c76-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-246">Boolean</span></span>|<span data-ttu-id="80c76-247">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="80c76-247">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="80c76-248">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="80c76-248">iCloudBlockMail</span></span>|<span data-ttu-id="80c76-249">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-249">Boolean</span></span>|<span data-ttu-id="80c76-250">Indica se deve ou não bloquear iCloud de email está sincronizando.</span><span class="sxs-lookup"><span data-stu-id="80c76-250">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="80c76-251">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="80c76-251">iCloudBlockAddressBook</span></span>|<span data-ttu-id="80c76-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-252">Boolean</span></span>|<span data-ttu-id="80c76-253">Indica se deve ou não bloquear iCloud da sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="80c76-253">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="80c76-254">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="80c76-254">iCloudBlockCalendar</span></span>|<span data-ttu-id="80c76-255">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-255">Boolean</span></span>|<span data-ttu-id="80c76-256">Indica se deve ou não bloquear iCloud seja sincronizado calendários.</span><span class="sxs-lookup"><span data-stu-id="80c76-256">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="80c76-257">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="80c76-257">iCloudBlockReminders</span></span>|<span data-ttu-id="80c76-258">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-258">Boolean</span></span>|<span data-ttu-id="80c76-259">Indica se deve ou não bloquear iCloud lembretes de sincronização.</span><span class="sxs-lookup"><span data-stu-id="80c76-259">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="80c76-260">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="80c76-260">iCloudBlockBookmarks</span></span>|<span data-ttu-id="80c76-261">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-261">Boolean</span></span>|<span data-ttu-id="80c76-262">Indica se deve ou não bloquear iCloud indicadores de sincronização.</span><span class="sxs-lookup"><span data-stu-id="80c76-262">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="80c76-263">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="80c76-263">iCloudBlockNotes</span></span>|<span data-ttu-id="80c76-264">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-264">Boolean</span></span>|<span data-ttu-id="80c76-265">Indica se deve ou não bloquear iCloud seja sincronizado anotações.</span><span class="sxs-lookup"><span data-stu-id="80c76-265">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="80c76-266">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="80c76-266">airDropBlocked</span></span>|<span data-ttu-id="80c76-267">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-267">Boolean</span></span>|<span data-ttu-id="80c76-268">Indica se deve ou não permitir que AirDrop.</span><span class="sxs-lookup"><span data-stu-id="80c76-268">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="80c76-269">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="80c76-269">passwordBlockModification</span></span>|<span data-ttu-id="80c76-270">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-270">Boolean</span></span>|<span data-ttu-id="80c76-271">Indica se deve ou não permitir a modificação de uma senha.</span><span class="sxs-lookup"><span data-stu-id="80c76-271">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="80c76-272">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="80c76-272">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="80c76-273">Booliano</span><span class="sxs-lookup"><span data-stu-id="80c76-273">Boolean</span></span>|<span data-ttu-id="80c76-274">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="80c76-274">Indicates whether or not to block fingerprint unlock.</span></span>|



## <a name="response"></a><span data-ttu-id="80c76-275">Resposta</span><span class="sxs-lookup"><span data-stu-id="80c76-275">Response</span></span>
<span data-ttu-id="80c76-276">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80c76-276">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80c76-277">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80c76-277">Example</span></span>
### <a name="request"></a><span data-ttu-id="80c76-278">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80c76-278">Request</span></span>
<span data-ttu-id="80c76-279">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80c76-279">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1747

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "passwordBlockFingerprintUnlock": true
}
```

### <a name="response"></a><span data-ttu-id="80c76-280">Resposta</span><span class="sxs-lookup"><span data-stu-id="80c76-280">Response</span></span>
<span data-ttu-id="80c76-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80c76-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1925

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
  "passwordBlockFingerprintUnlock": true
}
```





