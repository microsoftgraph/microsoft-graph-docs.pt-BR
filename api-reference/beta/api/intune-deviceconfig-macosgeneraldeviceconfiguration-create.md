---
title: Criar macOSGeneralDeviceConfiguration
description: Cria um novo objeto macOSGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f6f019609885973c16152df9647407e12c41c760
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33922456"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="40e29-103">Criar macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="40e29-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="40e29-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="40e29-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40e29-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40e29-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40e29-106">Cria um novo objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40e29-106">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40e29-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="40e29-107">Prerequisites</span></span>
<span data-ttu-id="40e29-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40e29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40e29-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40e29-110">Permission type</span></span>|<span data-ttu-id="40e29-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="40e29-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40e29-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40e29-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40e29-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40e29-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="40e29-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40e29-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40e29-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40e29-115">Not supported.</span></span>|
|<span data-ttu-id="40e29-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40e29-116">Application</span></span>|<span data-ttu-id="40e29-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40e29-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40e29-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40e29-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="40e29-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40e29-119">Request headers</span></span>
|<span data-ttu-id="40e29-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40e29-120">Header</span></span>|<span data-ttu-id="40e29-121">Valor</span><span class="sxs-lookup"><span data-stu-id="40e29-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40e29-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="40e29-122">Authorization</span></span>|<span data-ttu-id="40e29-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40e29-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40e29-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="40e29-124">Accept</span></span>|<span data-ttu-id="40e29-125">application/json</span><span class="sxs-lookup"><span data-stu-id="40e29-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40e29-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40e29-126">Request body</span></span>
<span data-ttu-id="40e29-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="40e29-127">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="40e29-128">A tabela a seguir mostra as propriedades obrigatórias ao criar macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="40e29-128">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="40e29-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40e29-129">Property</span></span>|<span data-ttu-id="40e29-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="40e29-130">Type</span></span>|<span data-ttu-id="40e29-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="40e29-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40e29-132">id</span><span class="sxs-lookup"><span data-stu-id="40e29-132">id</span></span>|<span data-ttu-id="40e29-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40e29-133">String</span></span>|<span data-ttu-id="40e29-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="40e29-134">Key of the entity.</span></span> <span data-ttu-id="40e29-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40e29-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40e29-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40e29-136">lastModifiedDateTime</span></span>|<span data-ttu-id="40e29-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40e29-137">DateTimeOffset</span></span>|<span data-ttu-id="40e29-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="40e29-138">DateTime the object was last modified.</span></span> <span data-ttu-id="40e29-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40e29-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40e29-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="40e29-140">roleScopeTagIds</span></span>|<span data-ttu-id="40e29-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="40e29-141">String collection</span></span>|<span data-ttu-id="40e29-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="40e29-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="40e29-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40e29-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40e29-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="40e29-144">supportsScopeTags</span></span>|<span data-ttu-id="40e29-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-145">Boolean</span></span>|<span data-ttu-id="40e29-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="40e29-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="40e29-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="40e29-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="40e29-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="40e29-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="40e29-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40e29-149">This property is read-only.</span></span> <span data-ttu-id="40e29-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40e29-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40e29-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40e29-151">createdDateTime</span></span>|<span data-ttu-id="40e29-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40e29-152">DateTimeOffset</span></span>|<span data-ttu-id="40e29-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="40e29-153">DateTime the object was created.</span></span> <span data-ttu-id="40e29-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40e29-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40e29-155">description</span><span class="sxs-lookup"><span data-stu-id="40e29-155">description</span></span>|<span data-ttu-id="40e29-156">String</span><span class="sxs-lookup"><span data-stu-id="40e29-156">String</span></span>|<span data-ttu-id="40e29-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40e29-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="40e29-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40e29-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40e29-159">displayName</span><span class="sxs-lookup"><span data-stu-id="40e29-159">displayName</span></span>|<span data-ttu-id="40e29-160">String</span><span class="sxs-lookup"><span data-stu-id="40e29-160">String</span></span>|<span data-ttu-id="40e29-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40e29-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="40e29-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40e29-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40e29-163">versão</span><span class="sxs-lookup"><span data-stu-id="40e29-163">version</span></span>|<span data-ttu-id="40e29-164">Int32</span><span class="sxs-lookup"><span data-stu-id="40e29-164">Int32</span></span>|<span data-ttu-id="40e29-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40e29-165">Version of the device configuration.</span></span> <span data-ttu-id="40e29-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40e29-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40e29-167">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="40e29-167">compliantAppsList</span></span>|<span data-ttu-id="40e29-168">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="40e29-168">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="40e29-169">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="40e29-169">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="40e29-170">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="40e29-170">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="40e29-171">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="40e29-171">compliantAppListType</span></span>|[<span data-ttu-id="40e29-172">appListType</span><span class="sxs-lookup"><span data-stu-id="40e29-172">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="40e29-173">Lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="40e29-173">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="40e29-174">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="40e29-174">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="40e29-175">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="40e29-175">emailInDomainSuffixes</span></span>|<span data-ttu-id="40e29-176">String collection</span><span class="sxs-lookup"><span data-stu-id="40e29-176">String collection</span></span>|<span data-ttu-id="40e29-177">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="40e29-177">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="40e29-178">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="40e29-178">passwordBlockSimple</span></span>|<span data-ttu-id="40e29-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-179">Boolean</span></span>|<span data-ttu-id="40e29-180">Bloquear senhas simples.</span><span class="sxs-lookup"><span data-stu-id="40e29-180">Block simple passwords.</span></span>|
|<span data-ttu-id="40e29-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="40e29-181">passwordExpirationDays</span></span>|<span data-ttu-id="40e29-182">Int32</span><span class="sxs-lookup"><span data-stu-id="40e29-182">Int32</span></span>|<span data-ttu-id="40e29-183">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="40e29-183">Number of days before the password expires.</span></span>|
|<span data-ttu-id="40e29-184">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="40e29-184">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="40e29-185">Int32</span><span class="sxs-lookup"><span data-stu-id="40e29-185">Int32</span></span>|<span data-ttu-id="40e29-186">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="40e29-186">Number of character sets a password must contain.</span></span> <span data-ttu-id="40e29-187">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="40e29-187">Valid values 0 to 4</span></span>|
|<span data-ttu-id="40e29-188">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="40e29-188">passwordMinimumLength</span></span>|<span data-ttu-id="40e29-189">Int32</span><span class="sxs-lookup"><span data-stu-id="40e29-189">Int32</span></span>|<span data-ttu-id="40e29-190">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="40e29-190">Minimum length of passwords.</span></span>|
|<span data-ttu-id="40e29-191">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="40e29-191">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="40e29-192">Int32</span><span class="sxs-lookup"><span data-stu-id="40e29-192">Int32</span></span>|<span data-ttu-id="40e29-193">Minutos de inatividade necessários antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="40e29-193">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="40e29-194">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="40e29-194">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="40e29-195">Int32</span><span class="sxs-lookup"><span data-stu-id="40e29-195">Int32</span></span>|<span data-ttu-id="40e29-196">Minutos de inatividade necessários antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="40e29-196">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="40e29-197">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="40e29-197">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="40e29-198">Int32</span><span class="sxs-lookup"><span data-stu-id="40e29-198">Int32</span></span>|<span data-ttu-id="40e29-199">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="40e29-199">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="40e29-200">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="40e29-200">passwordRequiredType</span></span>|[<span data-ttu-id="40e29-201">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="40e29-201">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="40e29-202">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="40e29-202">Type of password that is required.</span></span> <span data-ttu-id="40e29-203">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="40e29-203">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="40e29-204">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="40e29-204">passwordRequired</span></span>|<span data-ttu-id="40e29-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="40e29-205">Boolean</span></span>|<span data-ttu-id="40e29-206">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="40e29-206">Whether or not to require a password.</span></span>|
|<span data-ttu-id="40e29-207">Propriedadeskeychainblockcloudsync</span><span class="sxs-lookup"><span data-stu-id="40e29-207">keychainBlockCloudSync</span></span>|<span data-ttu-id="40e29-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-208">Boolean</span></span>|<span data-ttu-id="40e29-209">Indica se a sincronização de chaves do iCloud está bloqueada (macOS 10,12 e posterior).</span><span class="sxs-lookup"><span data-stu-id="40e29-209">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="40e29-210">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="40e29-210">airPrintBlocked</span></span>|<span data-ttu-id="40e29-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-211">Boolean</span></span>|<span data-ttu-id="40e29-212">Indica se o arquivo de impressão está bloqueado (macOS 10,12 e posterior).</span><span class="sxs-lookup"><span data-stu-id="40e29-212">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="40e29-213">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="40e29-213">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="40e29-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-214">Boolean</span></span>|<span data-ttu-id="40e29-215">Indica se certificados confiáveis são necessários para comunicação de impressão TLS (macOS 10,13 e posterior).</span><span class="sxs-lookup"><span data-stu-id="40e29-215">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="40e29-216">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="40e29-216">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="40e29-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-217">Boolean</span></span>|<span data-ttu-id="40e29-218">Indica se a descoberta de impressoras de impressão do iBeacon está ou não bloqueada.</span><span class="sxs-lookup"><span data-stu-id="40e29-218">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="40e29-219">Isso impede os beacons Bluetooth de impressão de mensagens de phishing para tráfego de rede (macOS 10,3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="40e29-219">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="40e29-220">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="40e29-220">safariBlockAutofill</span></span>|<span data-ttu-id="40e29-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-221">Boolean</span></span>|<span data-ttu-id="40e29-222">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="40e29-222">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="40e29-223">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="40e29-223">cameraBlocked</span></span>|<span data-ttu-id="40e29-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-224">Boolean</span></span>|<span data-ttu-id="40e29-225">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40e29-225">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="40e29-226">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="40e29-226">iTunesBlockMusicService</span></span>|<span data-ttu-id="40e29-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-227">Boolean</span></span>|<span data-ttu-id="40e29-228">Indica se o serviço de música deve ou não ser bloqueado e o aplicativo de música é revertido para o modo clássico.</span><span class="sxs-lookup"><span data-stu-id="40e29-228">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="40e29-229">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="40e29-229">spotlightBlockInternetResults</span></span>|<span data-ttu-id="40e29-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="40e29-230">Boolean</span></span>|<span data-ttu-id="40e29-231">Indica se o Spotlight deve ou não bloquear o retorno de qualquer resultado de uma pesquisa na Internet.</span><span class="sxs-lookup"><span data-stu-id="40e29-231">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="40e29-232">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="40e29-232">keyboardBlockDictation</span></span>|<span data-ttu-id="40e29-233">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-233">Boolean</span></span>|<span data-ttu-id="40e29-234">Indica se o usuário será ou não impedido de usar a entrada de ditado.</span><span class="sxs-lookup"><span data-stu-id="40e29-234">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="40e29-235">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="40e29-235">definitionLookupBlocked</span></span>|<span data-ttu-id="40e29-236">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-236">Boolean</span></span>|<span data-ttu-id="40e29-237">Indica se a pesquisa de definição deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="40e29-237">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="40e29-238">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="40e29-238">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="40e29-239">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-239">Boolean</span></span>|<span data-ttu-id="40e29-240">Indica se os usuários devem ou não bloquear seu Mac com o Apple Watch.</span><span class="sxs-lookup"><span data-stu-id="40e29-240">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="40e29-241">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="40e29-241">iTunesBlockFileSharing</span></span>|<span data-ttu-id="40e29-242">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-242">Boolean</span></span>|<span data-ttu-id="40e29-243">Indica se os arquivos devem ou não ser transferidos usando o iTunes.</span><span class="sxs-lookup"><span data-stu-id="40e29-243">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="40e29-244">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="40e29-244">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="40e29-245">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-245">Boolean</span></span>|<span data-ttu-id="40e29-246">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="40e29-246">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="40e29-247">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="40e29-247">iCloudBlockMail</span></span>|<span data-ttu-id="40e29-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-248">Boolean</span></span>|<span data-ttu-id="40e29-249">Indica se o iCloud deve ou não bloquear emails de sincronização.</span><span class="sxs-lookup"><span data-stu-id="40e29-249">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="40e29-250">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="40e29-250">iCloudBlockAddressBook</span></span>|<span data-ttu-id="40e29-251">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-251">Boolean</span></span>|<span data-ttu-id="40e29-252">Indica se o iCloud deve ou não bloquear os contatos de sincronização.</span><span class="sxs-lookup"><span data-stu-id="40e29-252">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="40e29-253">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="40e29-253">iCloudBlockCalendar</span></span>|<span data-ttu-id="40e29-254">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-254">Boolean</span></span>|<span data-ttu-id="40e29-255">Indica se o iCloud deve ou não bloquear calendários de sincronização.</span><span class="sxs-lookup"><span data-stu-id="40e29-255">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="40e29-256">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="40e29-256">iCloudBlockReminders</span></span>|<span data-ttu-id="40e29-257">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-257">Boolean</span></span>|<span data-ttu-id="40e29-258">Indica se o iCloud deve ou não bloquear lembretes de sincronização.</span><span class="sxs-lookup"><span data-stu-id="40e29-258">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="40e29-259">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="40e29-259">iCloudBlockBookmarks</span></span>|<span data-ttu-id="40e29-260">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-260">Boolean</span></span>|<span data-ttu-id="40e29-261">Indica se o iCloud deve ou não bloquear os indicadores de sincronização.</span><span class="sxs-lookup"><span data-stu-id="40e29-261">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="40e29-262">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="40e29-262">iCloudBlockNotes</span></span>|<span data-ttu-id="40e29-263">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-263">Boolean</span></span>|<span data-ttu-id="40e29-264">Indica se o iCloud deve ou não bloquear as anotações de sincronização.</span><span class="sxs-lookup"><span data-stu-id="40e29-264">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="40e29-265">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="40e29-265">airDropBlocked</span></span>|<span data-ttu-id="40e29-266">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-266">Boolean</span></span>|<span data-ttu-id="40e29-267">Indica se o recurso de recebimento de esficado deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="40e29-267">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="40e29-268">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="40e29-268">passwordBlockModification</span></span>|<span data-ttu-id="40e29-269">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-269">Boolean</span></span>|<span data-ttu-id="40e29-270">Indica se a modificação de senha deve ou não ser permitida.</span><span class="sxs-lookup"><span data-stu-id="40e29-270">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="40e29-271">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="40e29-271">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="40e29-272">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-272">Boolean</span></span>|<span data-ttu-id="40e29-273">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="40e29-273">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="40e29-274">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="40e29-274">passwordBlockAutoFill</span></span>|<span data-ttu-id="40e29-275">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-275">Boolean</span></span>|<span data-ttu-id="40e29-276">Indica se o recurso de senhas de preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="40e29-276">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="40e29-277">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="40e29-277">passwordBlockProximityRequests</span></span>|<span data-ttu-id="40e29-278">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-278">Boolean</span></span>|<span data-ttu-id="40e29-279">Indica se as senhas de solicitação devem ou não ser bloqueadas de dispositivos próximos.</span><span class="sxs-lookup"><span data-stu-id="40e29-279">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="40e29-280">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="40e29-280">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="40e29-281">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-281">Boolean</span></span>|<span data-ttu-id="40e29-282">Indica se as senhas de compartilhamento devem ou não ser bloqueadas com o recurso de senha de soltura.</span><span class="sxs-lookup"><span data-stu-id="40e29-282">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="40e29-283">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="40e29-283">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="40e29-284">Int32</span><span class="sxs-lookup"><span data-stu-id="40e29-284">Int32</span></span>|<span data-ttu-id="40e29-285">Define o número de dias que uma atualização de software será delyed para um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="40e29-285">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="40e29-286">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="40e29-286">Valid values 0 to 90</span></span>|
|<span data-ttu-id="40e29-287">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="40e29-287">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="40e29-288">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-288">Boolean</span></span>|<span data-ttu-id="40e29-289">Indica se o usuário deve ou não atrasar a visibilidade de atualizações de software quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="40e29-289">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="40e29-290">contentCachingBlocked</span><span class="sxs-lookup"><span data-stu-id="40e29-290">contentCachingBlocked</span></span>|<span data-ttu-id="40e29-291">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-291">Boolean</span></span>|<span data-ttu-id="40e29-292">Indica se o cache de conteúdo deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="40e29-292">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="40e29-293">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="40e29-293">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="40e29-294">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-294">Boolean</span></span>|<span data-ttu-id="40e29-295">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="40e29-295">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="40e29-296">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="40e29-296">screenCaptureBlocked</span></span>|<span data-ttu-id="40e29-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="40e29-297">Boolean</span></span>|<span data-ttu-id="40e29-298">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="40e29-298">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="40e29-299">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="40e29-299">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="40e29-300">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-300">Boolean</span></span>|<span data-ttu-id="40e29-301">Indica se a observação de tela remota deve ou não ser permitida por aplicativo de sala de aula.</span><span class="sxs-lookup"><span data-stu-id="40e29-301">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="40e29-302">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="40e29-302">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="40e29-303">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="40e29-303">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="40e29-304">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-304">Boolean</span></span>|<span data-ttu-id="40e29-305">Indica se a permissão será ou não automaticamente para o professor de um curso gerenciado no aplicativo da sala de aula para exibir a tela de um aluno sem avisar.</span><span class="sxs-lookup"><span data-stu-id="40e29-305">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="40e29-306">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="40e29-306">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="40e29-307">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="40e29-307">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="40e29-308">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-308">Boolean</span></span>|<span data-ttu-id="40e29-309">Indica se a permissão será ou não automaticamente para as solicitações do professor, sem avisar o aluno.</span><span class="sxs-lookup"><span data-stu-id="40e29-309">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="40e29-310">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="40e29-310">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="40e29-311">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="40e29-311">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="40e29-312">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-312">Boolean</span></span>|<span data-ttu-id="40e29-313">Indica se um aluno inscrito em um curso não gerenciado via sala de aula será solicitado a solicitar permissão do professor ao tentar sair do curso.</span><span class="sxs-lookup"><span data-stu-id="40e29-313">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="40e29-314">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="40e29-314">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="40e29-315">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="40e29-315">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="40e29-316">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e29-316">Boolean</span></span>|<span data-ttu-id="40e29-317">Indica se o professor deve ou não bloquear aplicativos ou o dispositivo sem avisar o aluno.</span><span class="sxs-lookup"><span data-stu-id="40e29-317">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="40e29-318">Requer o registro de MDM via Apple School Manager ou Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="40e29-318">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|



## <a name="response"></a><span data-ttu-id="40e29-319">Resposta</span><span class="sxs-lookup"><span data-stu-id="40e29-319">Response</span></span>
<span data-ttu-id="40e29-320">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40e29-320">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40e29-321">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40e29-321">Example</span></span>

### <a name="request"></a><span data-ttu-id="40e29-322">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40e29-322">Request</span></span>
<span data-ttu-id="40e29-323">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40e29-323">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2329

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

### <a name="response"></a><span data-ttu-id="40e29-324">Resposta</span><span class="sxs-lookup"><span data-stu-id="40e29-324">Response</span></span>
<span data-ttu-id="40e29-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40e29-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2501

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




