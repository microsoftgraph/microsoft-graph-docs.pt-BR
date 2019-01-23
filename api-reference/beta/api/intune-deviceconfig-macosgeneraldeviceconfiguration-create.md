---
title: Criar macOSGeneralDeviceConfiguration
description: Cria um novo objeto macOSGeneralDeviceConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6dd521646246914508a24f4c9188defff04bad9f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406511"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="57612-103">Criar macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="57612-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="57612-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="57612-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="57612-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="57612-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57612-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="57612-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57612-107">Cria um novo objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="57612-107">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57612-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57612-108">Prerequisites</span></span>
<span data-ttu-id="57612-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="57612-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="57612-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57612-111">Permission type</span></span>|<span data-ttu-id="57612-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57612-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57612-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57612-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57612-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57612-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57612-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57612-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57612-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57612-116">Not supported.</span></span>|
|<span data-ttu-id="57612-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57612-117">Application</span></span>|<span data-ttu-id="57612-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57612-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57612-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57612-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="57612-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57612-120">Request headers</span></span>
|<span data-ttu-id="57612-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57612-121">Header</span></span>|<span data-ttu-id="57612-122">Valor</span><span class="sxs-lookup"><span data-stu-id="57612-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57612-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="57612-123">Authorization</span></span>|<span data-ttu-id="57612-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57612-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57612-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57612-125">Accept</span></span>|<span data-ttu-id="57612-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57612-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57612-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57612-127">Request body</span></span>
<span data-ttu-id="57612-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="57612-128">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="57612-129">A tabela a seguir mostra as propriedades obrigatórias ao criar macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="57612-129">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="57612-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57612-130">Property</span></span>|<span data-ttu-id="57612-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="57612-131">Type</span></span>|<span data-ttu-id="57612-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="57612-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57612-133">id</span><span class="sxs-lookup"><span data-stu-id="57612-133">id</span></span>|<span data-ttu-id="57612-134">String</span><span class="sxs-lookup"><span data-stu-id="57612-134">String</span></span>|<span data-ttu-id="57612-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="57612-135">Key of the entity.</span></span> <span data-ttu-id="57612-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57612-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57612-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="57612-137">lastModifiedDateTime</span></span>|<span data-ttu-id="57612-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57612-138">DateTimeOffset</span></span>|<span data-ttu-id="57612-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="57612-139">DateTime the object was last modified.</span></span> <span data-ttu-id="57612-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57612-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57612-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="57612-141">roleScopeTagIds</span></span>|<span data-ttu-id="57612-142">String collection</span><span class="sxs-lookup"><span data-stu-id="57612-142">String collection</span></span>|<span data-ttu-id="57612-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="57612-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="57612-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57612-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57612-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="57612-145">supportsScopeTags</span></span>|<span data-ttu-id="57612-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-146">Boolean</span></span>|<span data-ttu-id="57612-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="57612-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="57612-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="57612-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="57612-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="57612-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="57612-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="57612-150">This property is read-only.</span></span> <span data-ttu-id="57612-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57612-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57612-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57612-152">createdDateTime</span></span>|<span data-ttu-id="57612-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57612-153">DateTimeOffset</span></span>|<span data-ttu-id="57612-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="57612-154">DateTime the object was created.</span></span> <span data-ttu-id="57612-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57612-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57612-156">description</span><span class="sxs-lookup"><span data-stu-id="57612-156">description</span></span>|<span data-ttu-id="57612-157">String</span><span class="sxs-lookup"><span data-stu-id="57612-157">String</span></span>|<span data-ttu-id="57612-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="57612-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="57612-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57612-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57612-160">displayName</span><span class="sxs-lookup"><span data-stu-id="57612-160">displayName</span></span>|<span data-ttu-id="57612-161">String</span><span class="sxs-lookup"><span data-stu-id="57612-161">String</span></span>|<span data-ttu-id="57612-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="57612-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="57612-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57612-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57612-164">version</span><span class="sxs-lookup"><span data-stu-id="57612-164">version</span></span>|<span data-ttu-id="57612-165">Int32</span><span class="sxs-lookup"><span data-stu-id="57612-165">Int32</span></span>|<span data-ttu-id="57612-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="57612-166">Version of the device configuration.</span></span> <span data-ttu-id="57612-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57612-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57612-168">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="57612-168">compliantAppsList</span></span>|<span data-ttu-id="57612-169">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="57612-169">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="57612-170">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="57612-170">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="57612-171">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="57612-171">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="57612-172">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="57612-172">compliantAppListType</span></span>|[<span data-ttu-id="57612-173">appListType</span><span class="sxs-lookup"><span data-stu-id="57612-173">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="57612-174">Lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="57612-174">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="57612-175">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="57612-175">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="57612-176">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="57612-176">emailInDomainSuffixes</span></span>|<span data-ttu-id="57612-177">String collection</span><span class="sxs-lookup"><span data-stu-id="57612-177">String collection</span></span>|<span data-ttu-id="57612-178">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="57612-178">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="57612-179">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="57612-179">passwordBlockSimple</span></span>|<span data-ttu-id="57612-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-180">Boolean</span></span>|<span data-ttu-id="57612-181">Bloquear senhas simples.</span><span class="sxs-lookup"><span data-stu-id="57612-181">Block simple passwords.</span></span>|
|<span data-ttu-id="57612-182">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="57612-182">passwordExpirationDays</span></span>|<span data-ttu-id="57612-183">Int32</span><span class="sxs-lookup"><span data-stu-id="57612-183">Int32</span></span>|<span data-ttu-id="57612-184">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="57612-184">Number of days before the password expires.</span></span>|
|<span data-ttu-id="57612-185">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="57612-185">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="57612-186">Int32</span><span class="sxs-lookup"><span data-stu-id="57612-186">Int32</span></span>|<span data-ttu-id="57612-187">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="57612-187">Number of character sets a password must contain.</span></span> <span data-ttu-id="57612-188">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="57612-188">Valid values 0 to 4</span></span>|
|<span data-ttu-id="57612-189">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="57612-189">passwordMinimumLength</span></span>|<span data-ttu-id="57612-190">Int32</span><span class="sxs-lookup"><span data-stu-id="57612-190">Int32</span></span>|<span data-ttu-id="57612-191">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="57612-191">Minimum length of passwords.</span></span>|
|<span data-ttu-id="57612-192">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="57612-192">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="57612-193">Int32</span><span class="sxs-lookup"><span data-stu-id="57612-193">Int32</span></span>|<span data-ttu-id="57612-194">Minutos de inatividade necessários antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="57612-194">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="57612-195">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="57612-195">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="57612-196">Int32</span><span class="sxs-lookup"><span data-stu-id="57612-196">Int32</span></span>|<span data-ttu-id="57612-197">Minutos de inatividade necessários antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="57612-197">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="57612-198">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="57612-198">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="57612-199">Int32</span><span class="sxs-lookup"><span data-stu-id="57612-199">Int32</span></span>|<span data-ttu-id="57612-200">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="57612-200">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="57612-201">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="57612-201">passwordRequiredType</span></span>|[<span data-ttu-id="57612-202">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="57612-202">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="57612-203">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="57612-203">Type of password that is required.</span></span> <span data-ttu-id="57612-204">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="57612-204">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="57612-205">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="57612-205">passwordRequired</span></span>|<span data-ttu-id="57612-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-206">Boolean</span></span>|<span data-ttu-id="57612-207">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="57612-207">Whether or not to require a password.</span></span>|
|<span data-ttu-id="57612-208">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="57612-208">keychainBlockCloudSync</span></span>|<span data-ttu-id="57612-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-209">Boolean</span></span>|<span data-ttu-id="57612-210">Indica se é ou não iCloud sincronização de conjunto de chaves bloqueado (macOS 10.12 e posterior).</span><span class="sxs-lookup"><span data-stu-id="57612-210">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="57612-211">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="57612-211">airPrintBlocked</span></span>|<span data-ttu-id="57612-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-212">Boolean</span></span>|<span data-ttu-id="57612-213">Indica se é ou não AirPrint bloqueados (macOS 10.12 e posterior).</span><span class="sxs-lookup"><span data-stu-id="57612-213">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="57612-214">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="57612-214">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="57612-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-215">Boolean</span></span>|<span data-ttu-id="57612-216">Indica se os certificados confiáveis são necessários para a comunicação de impressão de TLS (macOS 10.13 e posterior).</span><span class="sxs-lookup"><span data-stu-id="57612-216">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="57612-217">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="57612-217">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="57612-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-218">Boolean</span></span>|<span data-ttu-id="57612-219">Indica se ou não iBeacon descoberta de impressoras AirPrint está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="57612-219">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="57612-220">Isso impede que os avisos de AirPrint Bluetooth artificiais contra phishing para tráfego de rede (macOS 10.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="57612-220">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="57612-221">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="57612-221">safariBlockAutofill</span></span>|<span data-ttu-id="57612-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-222">Boolean</span></span>|<span data-ttu-id="57612-223">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="57612-223">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="57612-224">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="57612-224">cameraBlocked</span></span>|<span data-ttu-id="57612-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-225">Boolean</span></span>|<span data-ttu-id="57612-226">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="57612-226">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="57612-227">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="57612-227">iTunesBlockMusicService</span></span>|<span data-ttu-id="57612-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-228">Boolean</span></span>|<span data-ttu-id="57612-229">Indica se ou não bloquear o serviço de música e reverter o aplicativo de música para modo clássico.</span><span class="sxs-lookup"><span data-stu-id="57612-229">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="57612-230">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="57612-230">spotlightBlockInternetResults</span></span>|<span data-ttu-id="57612-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-231">Boolean</span></span>|<span data-ttu-id="57612-232">Indica se deve ou não bloquear destaque retornando todos os resultados de uma pesquisa na Internet.</span><span class="sxs-lookup"><span data-stu-id="57612-232">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="57612-233">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="57612-233">keyboardBlockDictation</span></span>|<span data-ttu-id="57612-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-234">Boolean</span></span>|<span data-ttu-id="57612-235">Indica se deve ou não bloquear o usuário usando a entrada de ditado.</span><span class="sxs-lookup"><span data-stu-id="57612-235">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="57612-236">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="57612-236">definitionLookupBlocked</span></span>|<span data-ttu-id="57612-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-237">Boolean</span></span>|<span data-ttu-id="57612-238">Indica se o bloqueio da pesquisa de definição ou não.</span><span class="sxs-lookup"><span data-stu-id="57612-238">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="57612-239">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="57612-239">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="57612-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-240">Boolean</span></span>|<span data-ttu-id="57612-241">Indica se ou aos usuários de bloco de desbloquear sua Mac com Apple Watch.</span><span class="sxs-lookup"><span data-stu-id="57612-241">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="57612-242">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="57612-242">iTunesBlockFileSharing</span></span>|<span data-ttu-id="57612-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-243">Boolean</span></span>|<span data-ttu-id="57612-244">Indica se ou não para bloquear arquivos do que está sendo transferido usando iTunes.</span><span class="sxs-lookup"><span data-stu-id="57612-244">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="57612-245">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="57612-245">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="57612-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-246">Boolean</span></span>|<span data-ttu-id="57612-247">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="57612-247">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="57612-248">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="57612-248">iCloudBlockMail</span></span>|<span data-ttu-id="57612-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-249">Boolean</span></span>|<span data-ttu-id="57612-250">Indica se deve ou não bloquear iCloud de email está sincronizando.</span><span class="sxs-lookup"><span data-stu-id="57612-250">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="57612-251">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="57612-251">iCloudBlockAddressBook</span></span>|<span data-ttu-id="57612-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-252">Boolean</span></span>|<span data-ttu-id="57612-253">Indica se deve ou não bloquear iCloud da sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="57612-253">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="57612-254">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="57612-254">iCloudBlockCalendar</span></span>|<span data-ttu-id="57612-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-255">Boolean</span></span>|<span data-ttu-id="57612-256">Indica se deve ou não bloquear iCloud seja sincronizado calendários.</span><span class="sxs-lookup"><span data-stu-id="57612-256">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="57612-257">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="57612-257">iCloudBlockReminders</span></span>|<span data-ttu-id="57612-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-258">Boolean</span></span>|<span data-ttu-id="57612-259">Indica se deve ou não bloquear iCloud lembretes de sincronização.</span><span class="sxs-lookup"><span data-stu-id="57612-259">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="57612-260">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="57612-260">iCloudBlockBookmarks</span></span>|<span data-ttu-id="57612-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-261">Boolean</span></span>|<span data-ttu-id="57612-262">Indica se deve ou não bloquear iCloud indicadores de sincronização.</span><span class="sxs-lookup"><span data-stu-id="57612-262">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="57612-263">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="57612-263">iCloudBlockNotes</span></span>|<span data-ttu-id="57612-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-264">Boolean</span></span>|<span data-ttu-id="57612-265">Indica se deve ou não bloquear iCloud seja sincronizado anotações.</span><span class="sxs-lookup"><span data-stu-id="57612-265">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="57612-266">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="57612-266">airDropBlocked</span></span>|<span data-ttu-id="57612-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-267">Boolean</span></span>|<span data-ttu-id="57612-268">Indica se deve ou não permitir que AirDrop.</span><span class="sxs-lookup"><span data-stu-id="57612-268">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="57612-269">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="57612-269">passwordBlockModification</span></span>|<span data-ttu-id="57612-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-270">Boolean</span></span>|<span data-ttu-id="57612-271">Indica se deve ou não permitir a modificação de uma senha.</span><span class="sxs-lookup"><span data-stu-id="57612-271">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="57612-272">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="57612-272">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="57612-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-273">Boolean</span></span>|<span data-ttu-id="57612-274">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="57612-274">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="57612-275">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="57612-275">passwordBlockAutoFill</span></span>|<span data-ttu-id="57612-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-276">Boolean</span></span>|<span data-ttu-id="57612-277">Indica se deve ou não bloquear o recurso de preenchimento automático de senhas.</span><span class="sxs-lookup"><span data-stu-id="57612-277">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="57612-278">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="57612-278">passwordBlockProximityRequests</span></span>|<span data-ttu-id="57612-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-279">Boolean</span></span>|<span data-ttu-id="57612-280">Indica se deve ou não bloquear solicitantes senhas de dispositivos próximos.</span><span class="sxs-lookup"><span data-stu-id="57612-280">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="57612-281">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="57612-281">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="57612-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="57612-282">Boolean</span></span>|<span data-ttu-id="57612-283">Indica se deve ou não bloquear as senhas de compartilhamento com o recurso de senhas AirDrop.</span><span class="sxs-lookup"><span data-stu-id="57612-283">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|



## <a name="response"></a><span data-ttu-id="57612-284">Resposta</span><span class="sxs-lookup"><span data-stu-id="57612-284">Response</span></span>
<span data-ttu-id="57612-285">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57612-285">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57612-286">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57612-286">Example</span></span>

### <a name="request"></a><span data-ttu-id="57612-287">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57612-287">Request</span></span>
<span data-ttu-id="57612-288">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57612-288">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1870

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
  "passwordBlockAirDropSharing": true
}
```

### <a name="response"></a><span data-ttu-id="57612-289">Resposta</span><span class="sxs-lookup"><span data-stu-id="57612-289">Response</span></span>
<span data-ttu-id="57612-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57612-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2042

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
  "passwordBlockAirDropSharing": true
}
```




