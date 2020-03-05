---
title: Criar macOSEndpointProtectionConfiguration
description: Criar um novo objeto macOSEndpointProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bfd96698582c247a34fdd602f74acbb71ce8708a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442366"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="05e27-103">Criar macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="05e27-103">Create macOSEndpointProtectionConfiguration</span></span>

<span data-ttu-id="05e27-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="05e27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05e27-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="05e27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05e27-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="05e27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05e27-107">Criar um novo objeto [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="05e27-107">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05e27-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="05e27-108">Prerequisites</span></span>
<span data-ttu-id="05e27-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05e27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05e27-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05e27-111">Permission type</span></span>|<span data-ttu-id="05e27-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="05e27-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05e27-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05e27-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05e27-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05e27-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="05e27-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05e27-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05e27-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05e27-116">Not supported.</span></span>|
|<span data-ttu-id="05e27-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05e27-117">Application</span></span>|<span data-ttu-id="05e27-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05e27-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05e27-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05e27-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="05e27-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05e27-120">Request headers</span></span>
|<span data-ttu-id="05e27-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05e27-121">Header</span></span>|<span data-ttu-id="05e27-122">Valor</span><span class="sxs-lookup"><span data-stu-id="05e27-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05e27-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="05e27-123">Authorization</span></span>|<span data-ttu-id="05e27-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05e27-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05e27-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="05e27-125">Accept</span></span>|<span data-ttu-id="05e27-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05e27-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05e27-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05e27-127">Request body</span></span>
<span data-ttu-id="05e27-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSEndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="05e27-128">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="05e27-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSEndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="05e27-129">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="05e27-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05e27-130">Property</span></span>|<span data-ttu-id="05e27-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="05e27-131">Type</span></span>|<span data-ttu-id="05e27-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="05e27-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05e27-133">id</span><span class="sxs-lookup"><span data-stu-id="05e27-133">id</span></span>|<span data-ttu-id="05e27-134">String</span><span class="sxs-lookup"><span data-stu-id="05e27-134">String</span></span>|<span data-ttu-id="05e27-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="05e27-135">Key of the entity.</span></span> <span data-ttu-id="05e27-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05e27-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05e27-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05e27-137">lastModifiedDateTime</span></span>|<span data-ttu-id="05e27-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05e27-138">DateTimeOffset</span></span>|<span data-ttu-id="05e27-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="05e27-139">DateTime the object was last modified.</span></span> <span data-ttu-id="05e27-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05e27-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05e27-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="05e27-141">roleScopeTagIds</span></span>|<span data-ttu-id="05e27-142">String collection</span><span class="sxs-lookup"><span data-stu-id="05e27-142">String collection</span></span>|<span data-ttu-id="05e27-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="05e27-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="05e27-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05e27-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05e27-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="05e27-145">supportsScopeTags</span></span>|<span data-ttu-id="05e27-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="05e27-146">Boolean</span></span>|<span data-ttu-id="05e27-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="05e27-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="05e27-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="05e27-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="05e27-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="05e27-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="05e27-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05e27-150">This property is read-only.</span></span> <span data-ttu-id="05e27-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05e27-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05e27-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="05e27-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="05e27-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="05e27-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="05e27-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="05e27-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="05e27-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05e27-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05e27-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="05e27-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="05e27-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="05e27-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="05e27-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="05e27-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="05e27-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05e27-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05e27-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="05e27-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="05e27-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="05e27-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="05e27-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="05e27-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="05e27-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05e27-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05e27-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="05e27-164">createdDateTime</span></span>|<span data-ttu-id="05e27-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05e27-165">DateTimeOffset</span></span>|<span data-ttu-id="05e27-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="05e27-166">DateTime the object was created.</span></span> <span data-ttu-id="05e27-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05e27-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05e27-168">description</span><span class="sxs-lookup"><span data-stu-id="05e27-168">description</span></span>|<span data-ttu-id="05e27-169">String</span><span class="sxs-lookup"><span data-stu-id="05e27-169">String</span></span>|<span data-ttu-id="05e27-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="05e27-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="05e27-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05e27-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05e27-172">displayName</span><span class="sxs-lookup"><span data-stu-id="05e27-172">displayName</span></span>|<span data-ttu-id="05e27-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05e27-173">String</span></span>|<span data-ttu-id="05e27-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="05e27-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="05e27-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05e27-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05e27-176">versão</span><span class="sxs-lookup"><span data-stu-id="05e27-176">version</span></span>|<span data-ttu-id="05e27-177">Int32</span><span class="sxs-lookup"><span data-stu-id="05e27-177">Int32</span></span>|<span data-ttu-id="05e27-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="05e27-178">Version of the device configuration.</span></span> <span data-ttu-id="05e27-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05e27-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05e27-180">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="05e27-180">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="05e27-181">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="05e27-181">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="05e27-182">Configuração de sistema e privacidade que determina quais locais de download os aplicativos podem ser executados em um dispositivo macOS.</span><span class="sxs-lookup"><span data-stu-id="05e27-182">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="05e27-183">Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="05e27-183">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="05e27-184">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="05e27-184">gatekeeperBlockOverride</span></span>|<span data-ttu-id="05e27-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="05e27-185">Boolean</span></span>|<span data-ttu-id="05e27-186">Se definido como true, a substituição do usuário para gatekeeper será desabilitada.</span><span class="sxs-lookup"><span data-stu-id="05e27-186">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="05e27-187">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="05e27-187">firewallEnabled</span></span>|<span data-ttu-id="05e27-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="05e27-188">Boolean</span></span>|<span data-ttu-id="05e27-189">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="05e27-189">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="05e27-190">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="05e27-190">firewallBlockAllIncoming</span></span>|<span data-ttu-id="05e27-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="05e27-191">Boolean</span></span>|<span data-ttu-id="05e27-192">Corresponde à opção "bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="05e27-192">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="05e27-193">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="05e27-193">firewallEnableStealthMode</span></span>|<span data-ttu-id="05e27-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="05e27-194">Boolean</span></span>|<span data-ttu-id="05e27-195">Corresponde a "Habilitar modo oculto".</span><span class="sxs-lookup"><span data-stu-id="05e27-195">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="05e27-196">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="05e27-196">firewallApplications</span></span>|<span data-ttu-id="05e27-197">coleção [macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)</span><span class="sxs-lookup"><span data-stu-id="05e27-197">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="05e27-198">Lista de aplicativos com configurações de firewall.</span><span class="sxs-lookup"><span data-stu-id="05e27-198">List of applications with firewall settings.</span></span> <span data-ttu-id="05e27-199">As configurações de firewall para aplicativos que não estão nessa lista são determinadas pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="05e27-199">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="05e27-200">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="05e27-200">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="05e27-201">fileVaultEnabled</span><span class="sxs-lookup"><span data-stu-id="05e27-201">fileVaultEnabled</span></span>|<span data-ttu-id="05e27-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="05e27-202">Boolean</span></span>|<span data-ttu-id="05e27-203">Se o FileVault deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="05e27-203">Whether FileVault should be enabled or not.</span></span>|
|<span data-ttu-id="05e27-204">fileVaultSelectedRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="05e27-204">fileVaultSelectedRecoveryKeyTypes</span></span>|[<span data-ttu-id="05e27-205">macOSFileVaultRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="05e27-205">macOSFileVaultRecoveryKeyTypes</span></span>](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|<span data-ttu-id="05e27-206">Obrigatório se FileVault estiver habilitado, determina o (s) tipo (s) de chave de recuperação a ser usado.</span><span class="sxs-lookup"><span data-stu-id="05e27-206">Required if FileVault is enabled, determines the type(s) of recovery key to use.</span></span> <span data-ttu-id="05e27-207">.</span><span class="sxs-lookup"><span data-stu-id="05e27-207">.</span></span> <span data-ttu-id="05e27-208">Os valores possíveis são: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span><span class="sxs-lookup"><span data-stu-id="05e27-208">Possible values are: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span></span>|
|<span data-ttu-id="05e27-209">fileVaultInstitutionalRecoveryKeyCertificate</span><span class="sxs-lookup"><span data-stu-id="05e27-209">fileVaultInstitutionalRecoveryKeyCertificate</span></span>|<span data-ttu-id="05e27-210">Binária</span><span class="sxs-lookup"><span data-stu-id="05e27-210">Binary</span></span>|<span data-ttu-id="05e27-211">Obrigatório se os tipos de chave de recuperação selecionados incluem InstitutionalRecoveryKey.</span><span class="sxs-lookup"><span data-stu-id="05e27-211">Required if selected recovery key type(s) include InstitutionalRecoveryKey.</span></span> <span data-ttu-id="05e27-212">O arquivo de certificado codificado por DER usado para definir uma chave de recuperação institucional.</span><span class="sxs-lookup"><span data-stu-id="05e27-212">The DER Encoded certificate file used to set an institutional recovery key.</span></span>|
|<span data-ttu-id="05e27-213">fileVaultInstitutionalRecoveryKeyCertificateFileName</span><span class="sxs-lookup"><span data-stu-id="05e27-213">fileVaultInstitutionalRecoveryKeyCertificateFileName</span></span>|<span data-ttu-id="05e27-214">String</span><span class="sxs-lookup"><span data-stu-id="05e27-214">String</span></span>|<span data-ttu-id="05e27-215">Nome do arquivo do certificado de chave de recuperação institucional a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="05e27-215">File name of the institutional recovery key certificate to display in UI.</span></span> <span data-ttu-id="05e27-216">(\*. der).</span><span class="sxs-lookup"><span data-stu-id="05e27-216">(\*.der).</span></span>|
|<span data-ttu-id="05e27-217">fileVaultPersonalRecoveryKeyHelpMessage</span><span class="sxs-lookup"><span data-stu-id="05e27-217">fileVaultPersonalRecoveryKeyHelpMessage</span></span>|<span data-ttu-id="05e27-218">String</span><span class="sxs-lookup"><span data-stu-id="05e27-218">String</span></span>|<span data-ttu-id="05e27-219">Obrigatório se os tipos de chave de recuperação selecionados incluem PersonalRecoveryKey.</span><span class="sxs-lookup"><span data-stu-id="05e27-219">Required if selected recovery key type(s) include PersonalRecoveryKey.</span></span> <span data-ttu-id="05e27-220">Uma mensagem curta exibida para o usuário que explica como eles podem recuperar sua chave de recuperação pessoal.</span><span class="sxs-lookup"><span data-stu-id="05e27-220">A short message displayed to the user that explains how they can retrieve their personal recovery key.</span></span>|
|<span data-ttu-id="05e27-221">fileVaultAllowDeferralUntilSignOut</span><span class="sxs-lookup"><span data-stu-id="05e27-221">fileVaultAllowDeferralUntilSignOut</span></span>|<span data-ttu-id="05e27-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="05e27-222">Boolean</span></span>|<span data-ttu-id="05e27-223">Opcional.</span><span class="sxs-lookup"><span data-stu-id="05e27-223">Optional.</span></span> <span data-ttu-id="05e27-224">Se for definido como true, o usuário poderá adiar a habilitação do FileVault até que ele saia.</span><span class="sxs-lookup"><span data-stu-id="05e27-224">If set to true, the user can defer the enabling of FileVault until they sign out.</span></span>|
|<span data-ttu-id="05e27-225">fileVaultNumberOfTimesUserCanIgnore</span><span class="sxs-lookup"><span data-stu-id="05e27-225">fileVaultNumberOfTimesUserCanIgnore</span></span>|<span data-ttu-id="05e27-226">Int32</span><span class="sxs-lookup"><span data-stu-id="05e27-226">Int32</span></span>|<span data-ttu-id="05e27-227">Opcional.</span><span class="sxs-lookup"><span data-stu-id="05e27-227">Optional.</span></span> <span data-ttu-id="05e27-228">Ao usar a opção Defer, este é o número máximo de vezes que o usuário pode ignorar as solicitações para habilitar o FileVault antes que o usuário entre no FileVault será necessário para entrar.</span><span class="sxs-lookup"><span data-stu-id="05e27-228">When using the Defer option, this is the maximum number of times the user can ignore prompts to enable FileVault before FileVault will be required for the user to sign in.</span></span> <span data-ttu-id="05e27-229">Se for definido como-1, ele sempre solicitará a habilitação do FileVault até que o FileVault esteja habilitado, embora permita que o usuário ignore a habilitação de FileVault.</span><span class="sxs-lookup"><span data-stu-id="05e27-229">If set to -1, it will always prompt to enable FileVault until FileVault is enabled, though it will allow the user to bypass enabling FileVault.</span></span> <span data-ttu-id="05e27-230">Configurar como 0 desativará o recurso.</span><span class="sxs-lookup"><span data-stu-id="05e27-230">Setting this to 0 will disable the feature.</span></span>|
|<span data-ttu-id="05e27-231">fileVaultDisablePromptAtSignOut</span><span class="sxs-lookup"><span data-stu-id="05e27-231">fileVaultDisablePromptAtSignOut</span></span>|<span data-ttu-id="05e27-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="05e27-232">Boolean</span></span>|<span data-ttu-id="05e27-233">Opcional.</span><span class="sxs-lookup"><span data-stu-id="05e27-233">Optional.</span></span> <span data-ttu-id="05e27-234">Ao usar a opção Defer, se definida como true, o usuário não será solicitado a habilitar o FileVault ao sair.</span><span class="sxs-lookup"><span data-stu-id="05e27-234">When using the Defer option, if set to true, the user is not prompted to enable FileVault at sign-out.</span></span>|
|<span data-ttu-id="05e27-235">fileVaultPersonalRecoveryKeyRotationInMonths</span><span class="sxs-lookup"><span data-stu-id="05e27-235">fileVaultPersonalRecoveryKeyRotationInMonths</span></span>|<span data-ttu-id="05e27-236">Int32</span><span class="sxs-lookup"><span data-stu-id="05e27-236">Int32</span></span>|<span data-ttu-id="05e27-237">Opcional.</span><span class="sxs-lookup"><span data-stu-id="05e27-237">Optional.</span></span> <span data-ttu-id="05e27-238">Se os tipos de chave de recuperação selecionados incluírem PersonalRecoveryKey, a frequência de rotação dessa chave, em meses.</span><span class="sxs-lookup"><span data-stu-id="05e27-238">If selected recovery key type(s) include PersonalRecoveryKey, the frequency to rotate that key, in months.</span></span>|



## <a name="response"></a><span data-ttu-id="05e27-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="05e27-239">Response</span></span>
<span data-ttu-id="05e27-240">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05e27-240">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05e27-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05e27-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="05e27-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05e27-242">Request</span></span>
<span data-ttu-id="05e27-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05e27-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2052

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
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
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ],
  "fileVaultEnabled": true,
  "fileVaultSelectedRecoveryKeyTypes": "institutionalRecoveryKey",
  "fileVaultInstitutionalRecoveryKeyCertificate": "ZmlsZVZhdWx0SW5zdGl0dXRpb25hbFJlY292ZXJ5S2V5Q2VydGlmaWNhdGU=",
  "fileVaultInstitutionalRecoveryKeyCertificateFileName": "File Vault Institutional Recovery Key Certificate File Name value",
  "fileVaultPersonalRecoveryKeyHelpMessage": "File Vault Personal Recovery Key Help Message value",
  "fileVaultAllowDeferralUntilSignOut": true,
  "fileVaultNumberOfTimesUserCanIgnore": 3,
  "fileVaultDisablePromptAtSignOut": true,
  "fileVaultPersonalRecoveryKeyRotationInMonths": 12
}
```

### <a name="response"></a><span data-ttu-id="05e27-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="05e27-244">Response</span></span>
<span data-ttu-id="05e27-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05e27-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2224

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "id": "7bf7f3ca-f3ca-7bf7-caf3-f77bcaf3f77b",
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
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ],
  "fileVaultEnabled": true,
  "fileVaultSelectedRecoveryKeyTypes": "institutionalRecoveryKey",
  "fileVaultInstitutionalRecoveryKeyCertificate": "ZmlsZVZhdWx0SW5zdGl0dXRpb25hbFJlY292ZXJ5S2V5Q2VydGlmaWNhdGU=",
  "fileVaultInstitutionalRecoveryKeyCertificateFileName": "File Vault Institutional Recovery Key Certificate File Name value",
  "fileVaultPersonalRecoveryKeyHelpMessage": "File Vault Personal Recovery Key Help Message value",
  "fileVaultAllowDeferralUntilSignOut": true,
  "fileVaultNumberOfTimesUserCanIgnore": 3,
  "fileVaultDisablePromptAtSignOut": true,
  "fileVaultPersonalRecoveryKeyRotationInMonths": 12
}
```





