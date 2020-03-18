---
title: Atualizar macOSEndpointProtectionConfiguration
description: Atualiza as propriedades de um objeto macOSEndpointProtectionConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 32c304b4ac704709a5ed3542580125aea79fcdf6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42746504"
---
# <a name="update-macosendpointprotectionconfiguration"></a><span data-ttu-id="64e72-103">Atualizar macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="64e72-103">Update macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="64e72-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64e72-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64e72-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64e72-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64e72-106">Atualiza as propriedades de um objeto [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="64e72-106">Update the properties of a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64e72-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64e72-107">Prerequisites</span></span>
<span data-ttu-id="64e72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64e72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64e72-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64e72-110">Permission type</span></span>|<span data-ttu-id="64e72-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="64e72-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64e72-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64e72-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64e72-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64e72-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64e72-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64e72-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64e72-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64e72-115">Not supported.</span></span>|
|<span data-ttu-id="64e72-116">Application</span><span class="sxs-lookup"><span data-stu-id="64e72-116">Application</span></span>|<span data-ttu-id="64e72-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64e72-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64e72-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64e72-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="64e72-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64e72-119">Request headers</span></span>
|<span data-ttu-id="64e72-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64e72-120">Header</span></span>|<span data-ttu-id="64e72-121">Valor</span><span class="sxs-lookup"><span data-stu-id="64e72-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64e72-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="64e72-122">Authorization</span></span>|<span data-ttu-id="64e72-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64e72-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64e72-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="64e72-124">Accept</span></span>|<span data-ttu-id="64e72-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64e72-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64e72-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64e72-126">Request body</span></span>
<span data-ttu-id="64e72-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="64e72-127">In the request body, supply a JSON representation for the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="64e72-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64e72-128">The following table shows the properties that are required when you create the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="64e72-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64e72-129">Property</span></span>|<span data-ttu-id="64e72-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="64e72-130">Type</span></span>|<span data-ttu-id="64e72-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="64e72-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64e72-132">id</span><span class="sxs-lookup"><span data-stu-id="64e72-132">id</span></span>|<span data-ttu-id="64e72-133">String</span><span class="sxs-lookup"><span data-stu-id="64e72-133">String</span></span>|<span data-ttu-id="64e72-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="64e72-134">Key of the entity.</span></span> <span data-ttu-id="64e72-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e72-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e72-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64e72-136">lastModifiedDateTime</span></span>|<span data-ttu-id="64e72-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64e72-137">DateTimeOffset</span></span>|<span data-ttu-id="64e72-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="64e72-138">DateTime the object was last modified.</span></span> <span data-ttu-id="64e72-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e72-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e72-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="64e72-140">roleScopeTagIds</span></span>|<span data-ttu-id="64e72-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="64e72-141">String collection</span></span>|<span data-ttu-id="64e72-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="64e72-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="64e72-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e72-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e72-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="64e72-144">supportsScopeTags</span></span>|<span data-ttu-id="64e72-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="64e72-145">Boolean</span></span>|<span data-ttu-id="64e72-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="64e72-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="64e72-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="64e72-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="64e72-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="64e72-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="64e72-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="64e72-149">This property is read-only.</span></span> <span data-ttu-id="64e72-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e72-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e72-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="64e72-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="64e72-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="64e72-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="64e72-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="64e72-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="64e72-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e72-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e72-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="64e72-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="64e72-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="64e72-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="64e72-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="64e72-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="64e72-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e72-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e72-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="64e72-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="64e72-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="64e72-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="64e72-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="64e72-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="64e72-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e72-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e72-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64e72-163">createdDateTime</span></span>|<span data-ttu-id="64e72-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64e72-164">DateTimeOffset</span></span>|<span data-ttu-id="64e72-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="64e72-165">DateTime the object was created.</span></span> <span data-ttu-id="64e72-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e72-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e72-167">description</span><span class="sxs-lookup"><span data-stu-id="64e72-167">description</span></span>|<span data-ttu-id="64e72-168">String</span><span class="sxs-lookup"><span data-stu-id="64e72-168">String</span></span>|<span data-ttu-id="64e72-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="64e72-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="64e72-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e72-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e72-171">displayName</span><span class="sxs-lookup"><span data-stu-id="64e72-171">displayName</span></span>|<span data-ttu-id="64e72-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64e72-172">String</span></span>|<span data-ttu-id="64e72-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="64e72-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="64e72-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e72-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e72-175">versão</span><span class="sxs-lookup"><span data-stu-id="64e72-175">version</span></span>|<span data-ttu-id="64e72-176">Int32</span><span class="sxs-lookup"><span data-stu-id="64e72-176">Int32</span></span>|<span data-ttu-id="64e72-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="64e72-177">Version of the device configuration.</span></span> <span data-ttu-id="64e72-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e72-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e72-179">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="64e72-179">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="64e72-180">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="64e72-180">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="64e72-181">Configuração de sistema e privacidade que determina quais locais de download os aplicativos podem ser executados em um dispositivo macOS.</span><span class="sxs-lookup"><span data-stu-id="64e72-181">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="64e72-182">Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="64e72-182">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="64e72-183">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="64e72-183">gatekeeperBlockOverride</span></span>|<span data-ttu-id="64e72-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="64e72-184">Boolean</span></span>|<span data-ttu-id="64e72-185">Se definido como true, a substituição do usuário para gatekeeper será desabilitada.</span><span class="sxs-lookup"><span data-stu-id="64e72-185">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="64e72-186">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="64e72-186">firewallEnabled</span></span>|<span data-ttu-id="64e72-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="64e72-187">Boolean</span></span>|<span data-ttu-id="64e72-188">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="64e72-188">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="64e72-189">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="64e72-189">firewallBlockAllIncoming</span></span>|<span data-ttu-id="64e72-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="64e72-190">Boolean</span></span>|<span data-ttu-id="64e72-191">Corresponde à opção "bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="64e72-191">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="64e72-192">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="64e72-192">firewallEnableStealthMode</span></span>|<span data-ttu-id="64e72-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="64e72-193">Boolean</span></span>|<span data-ttu-id="64e72-194">Corresponde a "Habilitar modo oculto".</span><span class="sxs-lookup"><span data-stu-id="64e72-194">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="64e72-195">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="64e72-195">firewallApplications</span></span>|<span data-ttu-id="64e72-196">coleção [macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)</span><span class="sxs-lookup"><span data-stu-id="64e72-196">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="64e72-197">Lista de aplicativos com configurações de firewall.</span><span class="sxs-lookup"><span data-stu-id="64e72-197">List of applications with firewall settings.</span></span> <span data-ttu-id="64e72-198">As configurações de firewall para aplicativos que não estão nessa lista são determinadas pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="64e72-198">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="64e72-199">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="64e72-199">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="64e72-200">fileVaultEnabled</span><span class="sxs-lookup"><span data-stu-id="64e72-200">fileVaultEnabled</span></span>|<span data-ttu-id="64e72-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="64e72-201">Boolean</span></span>|<span data-ttu-id="64e72-202">Se o FileVault deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="64e72-202">Whether FileVault should be enabled or not.</span></span>|
|<span data-ttu-id="64e72-203">fileVaultSelectedRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="64e72-203">fileVaultSelectedRecoveryKeyTypes</span></span>|[<span data-ttu-id="64e72-204">macOSFileVaultRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="64e72-204">macOSFileVaultRecoveryKeyTypes</span></span>](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|<span data-ttu-id="64e72-205">Obrigatório se FileVault estiver habilitado, determina o (s) tipo (s) de chave de recuperação a ser usado.</span><span class="sxs-lookup"><span data-stu-id="64e72-205">Required if FileVault is enabled, determines the type(s) of recovery key to use.</span></span> <span data-ttu-id="64e72-206">.</span><span class="sxs-lookup"><span data-stu-id="64e72-206">.</span></span> <span data-ttu-id="64e72-207">Os valores possíveis são: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span><span class="sxs-lookup"><span data-stu-id="64e72-207">Possible values are: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span></span>|
|<span data-ttu-id="64e72-208">fileVaultInstitutionalRecoveryKeyCertificate</span><span class="sxs-lookup"><span data-stu-id="64e72-208">fileVaultInstitutionalRecoveryKeyCertificate</span></span>|<span data-ttu-id="64e72-209">Binária</span><span class="sxs-lookup"><span data-stu-id="64e72-209">Binary</span></span>|<span data-ttu-id="64e72-210">Obrigatório se os tipos de chave de recuperação selecionados incluem InstitutionalRecoveryKey.</span><span class="sxs-lookup"><span data-stu-id="64e72-210">Required if selected recovery key type(s) include InstitutionalRecoveryKey.</span></span> <span data-ttu-id="64e72-211">O arquivo de certificado codificado por DER usado para definir uma chave de recuperação institucional.</span><span class="sxs-lookup"><span data-stu-id="64e72-211">The DER Encoded certificate file used to set an institutional recovery key.</span></span>|
|<span data-ttu-id="64e72-212">fileVaultInstitutionalRecoveryKeyCertificateFileName</span><span class="sxs-lookup"><span data-stu-id="64e72-212">fileVaultInstitutionalRecoveryKeyCertificateFileName</span></span>|<span data-ttu-id="64e72-213">String</span><span class="sxs-lookup"><span data-stu-id="64e72-213">String</span></span>|<span data-ttu-id="64e72-214">Nome do arquivo do certificado de chave de recuperação institucional a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="64e72-214">File name of the institutional recovery key certificate to display in UI.</span></span> <span data-ttu-id="64e72-215">(\*. der).</span><span class="sxs-lookup"><span data-stu-id="64e72-215">(\*.der).</span></span>|
|<span data-ttu-id="64e72-216">fileVaultPersonalRecoveryKeyHelpMessage</span><span class="sxs-lookup"><span data-stu-id="64e72-216">fileVaultPersonalRecoveryKeyHelpMessage</span></span>|<span data-ttu-id="64e72-217">String</span><span class="sxs-lookup"><span data-stu-id="64e72-217">String</span></span>|<span data-ttu-id="64e72-218">Obrigatório se os tipos de chave de recuperação selecionados incluem PersonalRecoveryKey.</span><span class="sxs-lookup"><span data-stu-id="64e72-218">Required if selected recovery key type(s) include PersonalRecoveryKey.</span></span> <span data-ttu-id="64e72-219">Uma mensagem curta exibida para o usuário que explica como eles podem recuperar sua chave de recuperação pessoal.</span><span class="sxs-lookup"><span data-stu-id="64e72-219">A short message displayed to the user that explains how they can retrieve their personal recovery key.</span></span>|
|<span data-ttu-id="64e72-220">fileVaultAllowDeferralUntilSignOut</span><span class="sxs-lookup"><span data-stu-id="64e72-220">fileVaultAllowDeferralUntilSignOut</span></span>|<span data-ttu-id="64e72-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="64e72-221">Boolean</span></span>|<span data-ttu-id="64e72-222">Opcional.</span><span class="sxs-lookup"><span data-stu-id="64e72-222">Optional.</span></span> <span data-ttu-id="64e72-223">Se for definido como true, o usuário poderá adiar a habilitação do FileVault até que ele saia.</span><span class="sxs-lookup"><span data-stu-id="64e72-223">If set to true, the user can defer the enabling of FileVault until they sign out.</span></span>|
|<span data-ttu-id="64e72-224">fileVaultNumberOfTimesUserCanIgnore</span><span class="sxs-lookup"><span data-stu-id="64e72-224">fileVaultNumberOfTimesUserCanIgnore</span></span>|<span data-ttu-id="64e72-225">Int32</span><span class="sxs-lookup"><span data-stu-id="64e72-225">Int32</span></span>|<span data-ttu-id="64e72-226">Opcional.</span><span class="sxs-lookup"><span data-stu-id="64e72-226">Optional.</span></span> <span data-ttu-id="64e72-227">Ao usar a opção Defer, este é o número máximo de vezes que o usuário pode ignorar as solicitações para habilitar o FileVault antes que o usuário entre no FileVault será necessário para entrar.</span><span class="sxs-lookup"><span data-stu-id="64e72-227">When using the Defer option, this is the maximum number of times the user can ignore prompts to enable FileVault before FileVault will be required for the user to sign in.</span></span> <span data-ttu-id="64e72-228">Se for definido como-1, ele sempre solicitará a habilitação do FileVault até que o FileVault esteja habilitado, embora permita que o usuário ignore a habilitação de FileVault.</span><span class="sxs-lookup"><span data-stu-id="64e72-228">If set to -1, it will always prompt to enable FileVault until FileVault is enabled, though it will allow the user to bypass enabling FileVault.</span></span> <span data-ttu-id="64e72-229">Configurar como 0 desativará o recurso.</span><span class="sxs-lookup"><span data-stu-id="64e72-229">Setting this to 0 will disable the feature.</span></span>|
|<span data-ttu-id="64e72-230">fileVaultDisablePromptAtSignOut</span><span class="sxs-lookup"><span data-stu-id="64e72-230">fileVaultDisablePromptAtSignOut</span></span>|<span data-ttu-id="64e72-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="64e72-231">Boolean</span></span>|<span data-ttu-id="64e72-232">Opcional.</span><span class="sxs-lookup"><span data-stu-id="64e72-232">Optional.</span></span> <span data-ttu-id="64e72-233">Ao usar a opção Defer, se definida como true, o usuário não será solicitado a habilitar o FileVault ao sair.</span><span class="sxs-lookup"><span data-stu-id="64e72-233">When using the Defer option, if set to true, the user is not prompted to enable FileVault at sign-out.</span></span>|
|<span data-ttu-id="64e72-234">fileVaultPersonalRecoveryKeyRotationInMonths</span><span class="sxs-lookup"><span data-stu-id="64e72-234">fileVaultPersonalRecoveryKeyRotationInMonths</span></span>|<span data-ttu-id="64e72-235">Int32</span><span class="sxs-lookup"><span data-stu-id="64e72-235">Int32</span></span>|<span data-ttu-id="64e72-236">Opcional.</span><span class="sxs-lookup"><span data-stu-id="64e72-236">Optional.</span></span> <span data-ttu-id="64e72-237">Se os tipos de chave de recuperação selecionados incluírem PersonalRecoveryKey, a frequência de rotação dessa chave, em meses.</span><span class="sxs-lookup"><span data-stu-id="64e72-237">If selected recovery key type(s) include PersonalRecoveryKey, the frequency to rotate that key, in months.</span></span>|
|<span data-ttu-id="64e72-238">fileVaultHidePersonalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="64e72-238">fileVaultHidePersonalRecoveryKey</span></span>|<span data-ttu-id="64e72-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="64e72-239">Boolean</span></span>|<span data-ttu-id="64e72-240">Opcional.</span><span class="sxs-lookup"><span data-stu-id="64e72-240">Optional.</span></span> <span data-ttu-id="64e72-241">Uma chave de recuperação pessoal oculta não aparece na tela do usuário durante a criptografia FileVault, reduzindo o risco de ela ser terminada nas mãos erradas.</span><span class="sxs-lookup"><span data-stu-id="64e72-241">A hidden personal recovery key does not appear on the user's screen during FileVault encryption, reducing the risk of it ending up in the wrong hands.</span></span>|
|<span data-ttu-id="64e72-242">advancedThreatProtectionRealTime</span><span class="sxs-lookup"><span data-stu-id="64e72-242">advancedThreatProtectionRealTime</span></span>|[<span data-ttu-id="64e72-243">habilitação</span><span class="sxs-lookup"><span data-stu-id="64e72-243">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="64e72-244">Determina se a proteção em tempo real para proteção avançada contra ameaças do Microsoft defender deve ou não ser habilitada no macOS.</span><span class="sxs-lookup"><span data-stu-id="64e72-244">Determines whether or not to enable real-time protection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="64e72-245">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="64e72-245">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="64e72-246">advancedThreatProtectionCloudDelivered</span><span class="sxs-lookup"><span data-stu-id="64e72-246">advancedThreatProtectionCloudDelivered</span></span>|[<span data-ttu-id="64e72-247">habilitação</span><span class="sxs-lookup"><span data-stu-id="64e72-247">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="64e72-248">Determina se a proteção do Microsoft defender para proteção avançada contra ameaças deve ou não ser habilitada no macOS.</span><span class="sxs-lookup"><span data-stu-id="64e72-248">Determines whether or not to enable cloud-delivered protection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="64e72-249">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="64e72-249">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="64e72-250">advancedThreatProtectionAutomaticSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="64e72-250">advancedThreatProtectionAutomaticSampleSubmission</span></span>|[<span data-ttu-id="64e72-251">habilitação</span><span class="sxs-lookup"><span data-stu-id="64e72-251">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="64e72-252">Determina se o envio automático de exemplo de arquivo para a proteção avançada contra ameaças do Microsoft defender deve ou não ser habilitado no macOS.</span><span class="sxs-lookup"><span data-stu-id="64e72-252">Determines whether or not to enable automatic file sample submission for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="64e72-253">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="64e72-253">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="64e72-254">advancedThreatProtectionDiagnosticDataCollection</span><span class="sxs-lookup"><span data-stu-id="64e72-254">advancedThreatProtectionDiagnosticDataCollection</span></span>|[<span data-ttu-id="64e72-255">habilitação</span><span class="sxs-lookup"><span data-stu-id="64e72-255">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="64e72-256">Determina se o diagnóstico e a coleta de dados de uso devem ou não ser habilitados para a proteção avançada contra ameaças do Microsoft defender no macOS.</span><span class="sxs-lookup"><span data-stu-id="64e72-256">Determines whether or not to enable diagnostic and usage data collection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="64e72-257">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="64e72-257">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="64e72-258">advancedThreatProtectionExcludedFolders</span><span class="sxs-lookup"><span data-stu-id="64e72-258">advancedThreatProtectionExcludedFolders</span></span>|<span data-ttu-id="64e72-259">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="64e72-259">String collection</span></span>|<span data-ttu-id="64e72-260">Uma lista de caminhos para pastas a serem excluídos da verificação de antivírus para proteção avançada contra ameaças do Microsoft defender no macOS.</span><span class="sxs-lookup"><span data-stu-id="64e72-260">A list of paths to folders to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="64e72-261">advancedThreatProtectionExcludedFiles</span><span class="sxs-lookup"><span data-stu-id="64e72-261">advancedThreatProtectionExcludedFiles</span></span>|<span data-ttu-id="64e72-262">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="64e72-262">String collection</span></span>|<span data-ttu-id="64e72-263">Uma lista de caminhos para arquivos a serem excluídos da verificação de antivírus para proteção avançada contra ameaças do Microsoft defender no macOS.</span><span class="sxs-lookup"><span data-stu-id="64e72-263">A list of paths to files to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="64e72-264">advancedThreatProtectionExcludedExtensions</span><span class="sxs-lookup"><span data-stu-id="64e72-264">advancedThreatProtectionExcludedExtensions</span></span>|<span data-ttu-id="64e72-265">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="64e72-265">String collection</span></span>|<span data-ttu-id="64e72-266">Uma lista de extensões de arquivo para excluir da verificação antivírus para proteção avançada contra ameaças do Microsoft defender no macOS.</span><span class="sxs-lookup"><span data-stu-id="64e72-266">A list of file extensions to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="64e72-267">advancedThreatProtectionExcludedProcesses</span><span class="sxs-lookup"><span data-stu-id="64e72-267">advancedThreatProtectionExcludedProcesses</span></span>|<span data-ttu-id="64e72-268">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="64e72-268">String collection</span></span>|<span data-ttu-id="64e72-269">Uma lista de nomes de processos a serem excluídos da verificação de antivírus para proteção avançada contra ameaças do Microsoft defender no macOS.</span><span class="sxs-lookup"><span data-stu-id="64e72-269">A list of process names to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|



## <a name="response"></a><span data-ttu-id="64e72-270">Resposta</span><span class="sxs-lookup"><span data-stu-id="64e72-270">Response</span></span>
<span data-ttu-id="64e72-271">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64e72-271">If successful, this method returns a `200 OK` response code and an updated [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64e72-272">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64e72-272">Example</span></span>

### <a name="request"></a><span data-ttu-id="64e72-273">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64e72-273">Request</span></span>
<span data-ttu-id="64e72-274">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64e72-274">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2786

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
  "fileVaultPersonalRecoveryKeyRotationInMonths": 12,
  "fileVaultHidePersonalRecoveryKey": true,
  "advancedThreatProtectionRealTime": "enabled",
  "advancedThreatProtectionCloudDelivered": "enabled",
  "advancedThreatProtectionAutomaticSampleSubmission": "enabled",
  "advancedThreatProtectionDiagnosticDataCollection": "enabled",
  "advancedThreatProtectionExcludedFolders": [
    "Advanced Threat Protection Excluded Folders value"
  ],
  "advancedThreatProtectionExcludedFiles": [
    "Advanced Threat Protection Excluded Files value"
  ],
  "advancedThreatProtectionExcludedExtensions": [
    "Advanced Threat Protection Excluded Extensions value"
  ],
  "advancedThreatProtectionExcludedProcesses": [
    "Advanced Threat Protection Excluded Processes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="64e72-275">Resposta</span><span class="sxs-lookup"><span data-stu-id="64e72-275">Response</span></span>
<span data-ttu-id="64e72-p128">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64e72-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2958

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
  "fileVaultPersonalRecoveryKeyRotationInMonths": 12,
  "fileVaultHidePersonalRecoveryKey": true,
  "advancedThreatProtectionRealTime": "enabled",
  "advancedThreatProtectionCloudDelivered": "enabled",
  "advancedThreatProtectionAutomaticSampleSubmission": "enabled",
  "advancedThreatProtectionDiagnosticDataCollection": "enabled",
  "advancedThreatProtectionExcludedFolders": [
    "Advanced Threat Protection Excluded Folders value"
  ],
  "advancedThreatProtectionExcludedFiles": [
    "Advanced Threat Protection Excluded Files value"
  ],
  "advancedThreatProtectionExcludedExtensions": [
    "Advanced Threat Protection Excluded Extensions value"
  ],
  "advancedThreatProtectionExcludedProcesses": [
    "Advanced Threat Protection Excluded Processes value"
  ]
}
```




