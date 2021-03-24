---
title: Atualizar macOSEndpointProtectionConfiguration
description: Atualize as propriedades de um objeto macOSEndpointProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 23e7bc30a9b5410e6f33e96d628654e1f9f69ebc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131320"
---
# <a name="update-macosendpointprotectionconfiguration"></a><span data-ttu-id="42a2d-103">Atualizar macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="42a2d-103">Update macOSEndpointProtectionConfiguration</span></span>

<span data-ttu-id="42a2d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42a2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42a2d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42a2d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42a2d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42a2d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42a2d-107">Atualize as propriedades de [um objeto macOSEndpointProtectionConfiguration.](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42a2d-107">Update the properties of a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42a2d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42a2d-108">Prerequisites</span></span>
<span data-ttu-id="42a2d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42a2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42a2d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42a2d-111">Permission type</span></span>|<span data-ttu-id="42a2d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42a2d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42a2d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42a2d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42a2d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42a2d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="42a2d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42a2d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42a2d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42a2d-116">Not supported.</span></span>|
|<span data-ttu-id="42a2d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42a2d-117">Application</span></span>|<span data-ttu-id="42a2d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42a2d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42a2d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42a2d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="42a2d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42a2d-120">Request headers</span></span>
|<span data-ttu-id="42a2d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42a2d-121">Header</span></span>|<span data-ttu-id="42a2d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="42a2d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42a2d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="42a2d-123">Authorization</span></span>|<span data-ttu-id="42a2d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42a2d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42a2d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="42a2d-125">Accept</span></span>|<span data-ttu-id="42a2d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42a2d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42a2d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42a2d-127">Request body</span></span>
<span data-ttu-id="42a2d-128">No corpo da solicitação, fornece uma representação JSON para o [objeto macOSEndpointProtectionConfiguration.](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42a2d-128">In the request body, supply a JSON representation for the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="42a2d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42a2d-129">The following table shows the properties that are required when you create the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="42a2d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42a2d-130">Property</span></span>|<span data-ttu-id="42a2d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="42a2d-131">Type</span></span>|<span data-ttu-id="42a2d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="42a2d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42a2d-133">id</span><span class="sxs-lookup"><span data-stu-id="42a2d-133">id</span></span>|<span data-ttu-id="42a2d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42a2d-134">String</span></span>|<span data-ttu-id="42a2d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="42a2d-135">Key of the entity.</span></span> <span data-ttu-id="42a2d-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42a2d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42a2d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42a2d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="42a2d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42a2d-138">DateTimeOffset</span></span>|<span data-ttu-id="42a2d-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="42a2d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="42a2d-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42a2d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42a2d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="42a2d-141">roleScopeTagIds</span></span>|<span data-ttu-id="42a2d-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="42a2d-142">String collection</span></span>|<span data-ttu-id="42a2d-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="42a2d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="42a2d-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42a2d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42a2d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="42a2d-145">supportsScopeTags</span></span>|<span data-ttu-id="42a2d-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="42a2d-146">Boolean</span></span>|<span data-ttu-id="42a2d-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="42a2d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="42a2d-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="42a2d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="42a2d-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="42a2d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="42a2d-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42a2d-150">This property is read-only.</span></span> <span data-ttu-id="42a2d-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42a2d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42a2d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="42a2d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="42a2d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="42a2d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="42a2d-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="42a2d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="42a2d-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42a2d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42a2d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="42a2d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="42a2d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="42a2d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="42a2d-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="42a2d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="42a2d-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42a2d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42a2d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="42a2d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="42a2d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="42a2d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="42a2d-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="42a2d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="42a2d-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42a2d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42a2d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42a2d-164">createdDateTime</span></span>|<span data-ttu-id="42a2d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42a2d-165">DateTimeOffset</span></span>|<span data-ttu-id="42a2d-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="42a2d-166">DateTime the object was created.</span></span> <span data-ttu-id="42a2d-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42a2d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42a2d-168">descrição</span><span class="sxs-lookup"><span data-stu-id="42a2d-168">description</span></span>|<span data-ttu-id="42a2d-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42a2d-169">String</span></span>|<span data-ttu-id="42a2d-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42a2d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="42a2d-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42a2d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42a2d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="42a2d-172">displayName</span></span>|<span data-ttu-id="42a2d-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42a2d-173">String</span></span>|<span data-ttu-id="42a2d-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42a2d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="42a2d-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42a2d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42a2d-176">versão</span><span class="sxs-lookup"><span data-stu-id="42a2d-176">version</span></span>|<span data-ttu-id="42a2d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="42a2d-177">Int32</span></span>|<span data-ttu-id="42a2d-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42a2d-178">Version of the device configuration.</span></span> <span data-ttu-id="42a2d-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42a2d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42a2d-180">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="42a2d-180">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="42a2d-181">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="42a2d-181">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="42a2d-182">Configuração de Sistema e Privacidade que determina de quais locais de download os aplicativos podem ser executados em um dispositivo macOS.</span><span class="sxs-lookup"><span data-stu-id="42a2d-182">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="42a2d-183">Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="42a2d-183">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="42a2d-184">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="42a2d-184">gatekeeperBlockOverride</span></span>|<span data-ttu-id="42a2d-185">Booleano</span><span class="sxs-lookup"><span data-stu-id="42a2d-185">Boolean</span></span>|<span data-ttu-id="42a2d-186">Se definido como true, a substituição do usuário para Gatekeeper será desabilitada.</span><span class="sxs-lookup"><span data-stu-id="42a2d-186">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="42a2d-187">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="42a2d-187">firewallEnabled</span></span>|<span data-ttu-id="42a2d-188">Booleano</span><span class="sxs-lookup"><span data-stu-id="42a2d-188">Boolean</span></span>|<span data-ttu-id="42a2d-189">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="42a2d-189">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="42a2d-190">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="42a2d-190">firewallBlockAllIncoming</span></span>|<span data-ttu-id="42a2d-191">Booleano</span><span class="sxs-lookup"><span data-stu-id="42a2d-191">Boolean</span></span>|<span data-ttu-id="42a2d-192">Corresponde à opção "Bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="42a2d-192">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="42a2d-193">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="42a2d-193">firewallEnableStealthMode</span></span>|<span data-ttu-id="42a2d-194">Booleano</span><span class="sxs-lookup"><span data-stu-id="42a2d-194">Boolean</span></span>|<span data-ttu-id="42a2d-195">Corresponde a "Habilitar o modo de furtividade".</span><span class="sxs-lookup"><span data-stu-id="42a2d-195">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="42a2d-196">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="42a2d-196">firewallApplications</span></span>|<span data-ttu-id="42a2d-197">[Coleção macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)</span><span class="sxs-lookup"><span data-stu-id="42a2d-197">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="42a2d-198">Lista de aplicativos com configurações de firewall.</span><span class="sxs-lookup"><span data-stu-id="42a2d-198">List of applications with firewall settings.</span></span> <span data-ttu-id="42a2d-199">As configurações de firewall para aplicativos que não estão nesta lista são determinadas pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="42a2d-199">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="42a2d-200">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="42a2d-200">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="42a2d-201">fileVaultEnabled</span><span class="sxs-lookup"><span data-stu-id="42a2d-201">fileVaultEnabled</span></span>|<span data-ttu-id="42a2d-202">Booleano</span><span class="sxs-lookup"><span data-stu-id="42a2d-202">Boolean</span></span>|<span data-ttu-id="42a2d-203">Se FileVault deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="42a2d-203">Whether FileVault should be enabled or not.</span></span>|
|<span data-ttu-id="42a2d-204">fileVaultSelectedRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="42a2d-204">fileVaultSelectedRecoveryKeyTypes</span></span>|[<span data-ttu-id="42a2d-205">macOSFileVaultRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="42a2d-205">macOSFileVaultRecoveryKeyTypes</span></span>](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|<span data-ttu-id="42a2d-206">Obrigatório se FileVault estiver habilitado, determina os tipos da chave de recuperação a ser usada.</span><span class="sxs-lookup"><span data-stu-id="42a2d-206">Required if FileVault is enabled, determines the type(s) of recovery key to use.</span></span> <span data-ttu-id="42a2d-207">.</span><span class="sxs-lookup"><span data-stu-id="42a2d-207">.</span></span> <span data-ttu-id="42a2d-208">Os valores possíveis são: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span><span class="sxs-lookup"><span data-stu-id="42a2d-208">Possible values are: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span></span>|
|<span data-ttu-id="42a2d-209">fileVaultInstitutionalRecoveryKeyCertificate</span><span class="sxs-lookup"><span data-stu-id="42a2d-209">fileVaultInstitutionalRecoveryKeyCertificate</span></span>|<span data-ttu-id="42a2d-210">Binário</span><span class="sxs-lookup"><span data-stu-id="42a2d-210">Binary</span></span>|<span data-ttu-id="42a2d-211">Obrigatório se os tipos de teclas de recuperação selecionados incluirEm InstitucionalRecoveryKey.</span><span class="sxs-lookup"><span data-stu-id="42a2d-211">Required if selected recovery key type(s) include InstitutionalRecoveryKey.</span></span> <span data-ttu-id="42a2d-212">O arquivo de certificado codificado por DER usado para definir uma chave de recuperação institucional.</span><span class="sxs-lookup"><span data-stu-id="42a2d-212">The DER Encoded certificate file used to set an institutional recovery key.</span></span>|
|<span data-ttu-id="42a2d-213">fileVaultInstitutionalRecoveryKeyCertificateFileName</span><span class="sxs-lookup"><span data-stu-id="42a2d-213">fileVaultInstitutionalRecoveryKeyCertificateFileName</span></span>|<span data-ttu-id="42a2d-214">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42a2d-214">String</span></span>|<span data-ttu-id="42a2d-215">Nome do arquivo do certificado de chave de recuperação institucional a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="42a2d-215">File name of the institutional recovery key certificate to display in UI.</span></span> <span data-ttu-id="42a2d-216">(\*.der).</span><span class="sxs-lookup"><span data-stu-id="42a2d-216">(\*.der).</span></span>|
|<span data-ttu-id="42a2d-217">fileVaultPersonalRecoveryKeyHelpMessage</span><span class="sxs-lookup"><span data-stu-id="42a2d-217">fileVaultPersonalRecoveryKeyHelpMessage</span></span>|<span data-ttu-id="42a2d-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42a2d-218">String</span></span>|<span data-ttu-id="42a2d-219">Obrigatório se os tipos de teclas de recuperação selecionados incluirEm PersonalRecoveryKey.</span><span class="sxs-lookup"><span data-stu-id="42a2d-219">Required if selected recovery key type(s) include PersonalRecoveryKey.</span></span> <span data-ttu-id="42a2d-220">Uma mensagem curta exibida para o usuário que explica como eles podem recuperar sua chave de recuperação pessoal.</span><span class="sxs-lookup"><span data-stu-id="42a2d-220">A short message displayed to the user that explains how they can retrieve their personal recovery key.</span></span>|
|<span data-ttu-id="42a2d-221">fileVaultAllowDeferralUntilSignOut</span><span class="sxs-lookup"><span data-stu-id="42a2d-221">fileVaultAllowDeferralUntilSignOut</span></span>|<span data-ttu-id="42a2d-222">Booleano</span><span class="sxs-lookup"><span data-stu-id="42a2d-222">Boolean</span></span>|<span data-ttu-id="42a2d-223">Opcional.</span><span class="sxs-lookup"><span data-stu-id="42a2d-223">Optional.</span></span> <span data-ttu-id="42a2d-224">Se for definido como true, o usuário poderá adiar a habilitação de FileVault até sair.</span><span class="sxs-lookup"><span data-stu-id="42a2d-224">If set to true, the user can defer the enabling of FileVault until they sign out.</span></span>|
|<span data-ttu-id="42a2d-225">fileVaultNumberOfTimesUserCanIgnore</span><span class="sxs-lookup"><span data-stu-id="42a2d-225">fileVaultNumberOfTimesUserCanIgnore</span></span>|<span data-ttu-id="42a2d-226">Int32</span><span class="sxs-lookup"><span data-stu-id="42a2d-226">Int32</span></span>|<span data-ttu-id="42a2d-227">Opcional.</span><span class="sxs-lookup"><span data-stu-id="42a2d-227">Optional.</span></span> <span data-ttu-id="42a2d-228">Ao usar a opção Adiar, esse é o número máximo de vezes que o usuário pode ignorar prompts para habilitar FileVault antes que FileVault seja necessário para o usuário entrar.</span><span class="sxs-lookup"><span data-stu-id="42a2d-228">When using the Defer option, this is the maximum number of times the user can ignore prompts to enable FileVault before FileVault will be required for the user to sign in.</span></span> <span data-ttu-id="42a2d-229">Se estiver definido como -1, ele sempre solicitará que FileVault seja habilitado até que FileVault seja habilitado, embora permita que o usuário ignore a habilitação de FileVault.</span><span class="sxs-lookup"><span data-stu-id="42a2d-229">If set to -1, it will always prompt to enable FileVault until FileVault is enabled, though it will allow the user to bypass enabling FileVault.</span></span> <span data-ttu-id="42a2d-230">Definir isso como 0 desabilitará o recurso.</span><span class="sxs-lookup"><span data-stu-id="42a2d-230">Setting this to 0 will disable the feature.</span></span>|
|<span data-ttu-id="42a2d-231">fileVaultDisablePromptAtSignOut</span><span class="sxs-lookup"><span data-stu-id="42a2d-231">fileVaultDisablePromptAtSignOut</span></span>|<span data-ttu-id="42a2d-232">Booleano</span><span class="sxs-lookup"><span data-stu-id="42a2d-232">Boolean</span></span>|<span data-ttu-id="42a2d-233">Opcional.</span><span class="sxs-lookup"><span data-stu-id="42a2d-233">Optional.</span></span> <span data-ttu-id="42a2d-234">Ao usar a opção Adiar, se definido como true, o usuário não é solicitado a habilitar FileVault na saída.</span><span class="sxs-lookup"><span data-stu-id="42a2d-234">When using the Defer option, if set to true, the user is not prompted to enable FileVault at sign-out.</span></span>|
|<span data-ttu-id="42a2d-235">fileVaultPersonalRecoveryKeyRotationInMonths</span><span class="sxs-lookup"><span data-stu-id="42a2d-235">fileVaultPersonalRecoveryKeyRotationInMonths</span></span>|<span data-ttu-id="42a2d-236">Int32</span><span class="sxs-lookup"><span data-stu-id="42a2d-236">Int32</span></span>|<span data-ttu-id="42a2d-237">Opcional.</span><span class="sxs-lookup"><span data-stu-id="42a2d-237">Optional.</span></span> <span data-ttu-id="42a2d-238">Se os tipos de teclas de recuperação selecionados incluirEm PersonalRecoveryKey, a frequência para girar essa chave, em meses.</span><span class="sxs-lookup"><span data-stu-id="42a2d-238">If selected recovery key type(s) include PersonalRecoveryKey, the frequency to rotate that key, in months.</span></span>|
|<span data-ttu-id="42a2d-239">fileVaultHidePersonalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="42a2d-239">fileVaultHidePersonalRecoveryKey</span></span>|<span data-ttu-id="42a2d-240">Booleano</span><span class="sxs-lookup"><span data-stu-id="42a2d-240">Boolean</span></span>|<span data-ttu-id="42a2d-241">Opcional.</span><span class="sxs-lookup"><span data-stu-id="42a2d-241">Optional.</span></span> <span data-ttu-id="42a2d-242">Uma chave de recuperação pessoal oculta não aparece na tela do usuário durante a criptografia FileVault, reduzindo o risco de ela acabar em mãos erradas.</span><span class="sxs-lookup"><span data-stu-id="42a2d-242">A hidden personal recovery key does not appear on the user's screen during FileVault encryption, reducing the risk of it ending up in the wrong hands.</span></span>|
|<span data-ttu-id="42a2d-243">advancedThreatProtectionRealTime</span><span class="sxs-lookup"><span data-stu-id="42a2d-243">advancedThreatProtectionRealTime</span></span>|[<span data-ttu-id="42a2d-244">enablement</span><span class="sxs-lookup"><span data-stu-id="42a2d-244">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="42a2d-245">Determina se a proteção em tempo real do Microsoft Defender Advanced Threat Protection será habilitada ou não no macOS.</span><span class="sxs-lookup"><span data-stu-id="42a2d-245">Determines whether or not to enable real-time protection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="42a2d-246">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="42a2d-246">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="42a2d-247">advancedThreatProtectionCloudDelivered</span><span class="sxs-lookup"><span data-stu-id="42a2d-247">advancedThreatProtectionCloudDelivered</span></span>|[<span data-ttu-id="42a2d-248">enablement</span><span class="sxs-lookup"><span data-stu-id="42a2d-248">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="42a2d-249">Determina se a proteção entregue na nuvem deve ou não ser habilitada para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS.</span><span class="sxs-lookup"><span data-stu-id="42a2d-249">Determines whether or not to enable cloud-delivered protection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="42a2d-250">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="42a2d-250">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="42a2d-251">advancedThreatProtectionAutomaticSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="42a2d-251">advancedThreatProtectionAutomaticSampleSubmission</span></span>|[<span data-ttu-id="42a2d-252">enablement</span><span class="sxs-lookup"><span data-stu-id="42a2d-252">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="42a2d-253">Determina se deve ou não habilitar o envio automático de exemplo de arquivo para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS.</span><span class="sxs-lookup"><span data-stu-id="42a2d-253">Determines whether or not to enable automatic file sample submission for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="42a2d-254">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="42a2d-254">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="42a2d-255">advancedThreatProtectionDiagnosticDataCollection</span><span class="sxs-lookup"><span data-stu-id="42a2d-255">advancedThreatProtectionDiagnosticDataCollection</span></span>|[<span data-ttu-id="42a2d-256">enablement</span><span class="sxs-lookup"><span data-stu-id="42a2d-256">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="42a2d-257">Determina se será ou não possível habilitar a coleta de dados de diagnóstico e uso para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS.</span><span class="sxs-lookup"><span data-stu-id="42a2d-257">Determines whether or not to enable diagnostic and usage data collection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="42a2d-258">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="42a2d-258">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="42a2d-259">advancedThreatProtectionExcludedFolders</span><span class="sxs-lookup"><span data-stu-id="42a2d-259">advancedThreatProtectionExcludedFolders</span></span>|<span data-ttu-id="42a2d-260">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="42a2d-260">String collection</span></span>|<span data-ttu-id="42a2d-261">Uma lista de caminhos para pastas a excluir da verificação de antivírus para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS.</span><span class="sxs-lookup"><span data-stu-id="42a2d-261">A list of paths to folders to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="42a2d-262">advancedThreatProtectionExcludedFiles</span><span class="sxs-lookup"><span data-stu-id="42a2d-262">advancedThreatProtectionExcludedFiles</span></span>|<span data-ttu-id="42a2d-263">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="42a2d-263">String collection</span></span>|<span data-ttu-id="42a2d-264">Uma lista de caminhos para arquivos a ser excluídos da verificação de antivírus para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS.</span><span class="sxs-lookup"><span data-stu-id="42a2d-264">A list of paths to files to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="42a2d-265">advancedThreatProtectionExcludedExtensions</span><span class="sxs-lookup"><span data-stu-id="42a2d-265">advancedThreatProtectionExcludedExtensions</span></span>|<span data-ttu-id="42a2d-266">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="42a2d-266">String collection</span></span>|<span data-ttu-id="42a2d-267">Uma lista de extensões de arquivo a excluir da verificação de antivírus para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS.</span><span class="sxs-lookup"><span data-stu-id="42a2d-267">A list of file extensions to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="42a2d-268">advancedThreatProtectionExcludedProcesses</span><span class="sxs-lookup"><span data-stu-id="42a2d-268">advancedThreatProtectionExcludedProcesses</span></span>|<span data-ttu-id="42a2d-269">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="42a2d-269">String collection</span></span>|<span data-ttu-id="42a2d-270">Uma lista de nomes de processo a ser excluídos da verificação de antivírus para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS.</span><span class="sxs-lookup"><span data-stu-id="42a2d-270">A list of process names to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|



## <a name="response"></a><span data-ttu-id="42a2d-271">Resposta</span><span class="sxs-lookup"><span data-stu-id="42a2d-271">Response</span></span>
<span data-ttu-id="42a2d-272">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42a2d-272">If successful, this method returns a `200 OK` response code and an updated [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42a2d-273">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42a2d-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="42a2d-274">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42a2d-274">Request</span></span>
<span data-ttu-id="42a2d-275">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42a2d-275">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="42a2d-276">Resposta</span><span class="sxs-lookup"><span data-stu-id="42a2d-276">Response</span></span>
<span data-ttu-id="42a2d-p128">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42a2d-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




