---
title: Atualizar windowsDeliveryOptimizationConfiguration
description: Atualiza as propriedades de um objeto windowsDeliveryOptimizationConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ea12634b689b5df13313ae22aaf585eadb0e3659
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961984"
---
# <a name="update-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="62687-103">Atualizar windowsDeliveryOptimizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="62687-103">Update windowsDeliveryOptimizationConfiguration</span></span>

> <span data-ttu-id="62687-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62687-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62687-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62687-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62687-106">Atualiza as propriedades de um objeto [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="62687-106">Update the properties of a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62687-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="62687-107">Prerequisites</span></span>
<span data-ttu-id="62687-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62687-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62687-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62687-110">Permission type</span></span>|<span data-ttu-id="62687-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="62687-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62687-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62687-112">Delegated (work or school account)</span></span>|<span data-ttu-id="62687-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62687-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="62687-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62687-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62687-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62687-115">Not supported.</span></span>|
|<span data-ttu-id="62687-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62687-116">Application</span></span>|<span data-ttu-id="62687-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62687-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62687-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62687-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="62687-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62687-119">Request headers</span></span>
|<span data-ttu-id="62687-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62687-120">Header</span></span>|<span data-ttu-id="62687-121">Valor</span><span class="sxs-lookup"><span data-stu-id="62687-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62687-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="62687-122">Authorization</span></span>|<span data-ttu-id="62687-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62687-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62687-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62687-124">Accept</span></span>|<span data-ttu-id="62687-125">application/json</span><span class="sxs-lookup"><span data-stu-id="62687-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62687-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62687-126">Request body</span></span>
<span data-ttu-id="62687-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="62687-127">In the request body, supply a JSON representation for the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

<span data-ttu-id="62687-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62687-128">The following table shows the properties that are required when you create the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md).</span></span>

|<span data-ttu-id="62687-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62687-129">Property</span></span>|<span data-ttu-id="62687-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="62687-130">Type</span></span>|<span data-ttu-id="62687-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="62687-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62687-132">id</span><span class="sxs-lookup"><span data-stu-id="62687-132">id</span></span>|<span data-ttu-id="62687-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62687-133">String</span></span>|<span data-ttu-id="62687-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="62687-134">Key of the entity.</span></span> <span data-ttu-id="62687-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62687-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62687-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62687-136">lastModifiedDateTime</span></span>|<span data-ttu-id="62687-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62687-137">DateTimeOffset</span></span>|<span data-ttu-id="62687-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="62687-138">DateTime the object was last modified.</span></span> <span data-ttu-id="62687-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62687-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62687-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="62687-140">roleScopeTagIds</span></span>|<span data-ttu-id="62687-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="62687-141">String collection</span></span>|<span data-ttu-id="62687-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="62687-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="62687-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62687-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62687-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="62687-144">supportsScopeTags</span></span>|<span data-ttu-id="62687-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="62687-145">Boolean</span></span>|<span data-ttu-id="62687-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="62687-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="62687-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="62687-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="62687-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="62687-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="62687-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="62687-149">This property is read-only.</span></span> <span data-ttu-id="62687-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62687-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62687-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="62687-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="62687-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="62687-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="62687-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="62687-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="62687-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62687-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62687-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="62687-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="62687-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="62687-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="62687-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="62687-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="62687-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62687-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62687-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="62687-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="62687-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="62687-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="62687-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="62687-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="62687-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62687-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62687-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62687-163">createdDateTime</span></span>|<span data-ttu-id="62687-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62687-164">DateTimeOffset</span></span>|<span data-ttu-id="62687-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="62687-165">DateTime the object was created.</span></span> <span data-ttu-id="62687-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62687-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62687-167">descrição</span><span class="sxs-lookup"><span data-stu-id="62687-167">description</span></span>|<span data-ttu-id="62687-168">String</span><span class="sxs-lookup"><span data-stu-id="62687-168">String</span></span>|<span data-ttu-id="62687-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="62687-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="62687-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62687-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62687-171">displayName</span><span class="sxs-lookup"><span data-stu-id="62687-171">displayName</span></span>|<span data-ttu-id="62687-172">String</span><span class="sxs-lookup"><span data-stu-id="62687-172">String</span></span>|<span data-ttu-id="62687-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="62687-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="62687-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62687-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62687-175">versão</span><span class="sxs-lookup"><span data-stu-id="62687-175">version</span></span>|<span data-ttu-id="62687-176">Int32</span><span class="sxs-lookup"><span data-stu-id="62687-176">Int32</span></span>|<span data-ttu-id="62687-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="62687-177">Version of the device configuration.</span></span> <span data-ttu-id="62687-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62687-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62687-179">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="62687-179">deliveryOptimizationMode</span></span>|[<span data-ttu-id="62687-180">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="62687-180">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="62687-181">Especifica o método de download que a otimização de entrega pode usar para gerenciar o consumo de largura de banda de rede para grandes cenários de distribuição de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="62687-181">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="62687-182">Os valores possíveis são: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="62687-182">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="62687-183">restrictPeerSelectionBy</span><span class="sxs-lookup"><span data-stu-id="62687-183">restrictPeerSelectionBy</span></span>|[<span data-ttu-id="62687-184">deliveryOptimizationRestrictPeerSelectionByOptions</span><span class="sxs-lookup"><span data-stu-id="62687-184">deliveryOptimizationRestrictPeerSelectionByOptions</span></span>](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|<span data-ttu-id="62687-185">Especifica a restrição da seleção de pares por meio da opção selecionada.</span><span class="sxs-lookup"><span data-stu-id="62687-185">Specifies to restrict peer selection via selected option.</span></span>
<span data-ttu-id="62687-186">A opção 1 (máscara de sub-rede) só se aplica aos modos de otimização de entrega LAN do modo de download (1) e grupo (2).</span><span class="sxs-lookup"><span data-stu-id="62687-186">Option 1 (Subnet mask) only applies to Delivery Optimization modes Download Mode LAN (1) and Group (2).</span></span> <span data-ttu-id="62687-187">Os valores possíveis são: `notConfigured` e `subnetMask`.</span><span class="sxs-lookup"><span data-stu-id="62687-187">Possible values are: `notConfigured`, `subnetMask`.</span></span>|
|<span data-ttu-id="62687-188">groupIdSource</span><span class="sxs-lookup"><span data-stu-id="62687-188">groupIdSource</span></span>|[<span data-ttu-id="62687-189">deliveryOptimizationGroupIdSource</span><span class="sxs-lookup"><span data-stu-id="62687-189">deliveryOptimizationGroupIdSource</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|<span data-ttu-id="62687-190">Especifica a restrição da seleção de par para uma fonte específicas.</span><span class="sxs-lookup"><span data-stu-id="62687-190">Specifies to restrict peer selection to a specfic source.</span></span>
<span data-ttu-id="62687-191">As opções definidas nesta política se aplicam apenas ao modo de download grupo (2) do modo de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="62687-191">The options set in this policy only apply to Delivery Optimization mode Group (2) download mode.</span></span> <span data-ttu-id="62687-192">Se o grupo (2) não estiver definido como modo de download, esta política será ignorada.</span><span class="sxs-lookup"><span data-stu-id="62687-192">If Group (2) isn't set as Download mode, this policy will be ignored.</span></span> <span data-ttu-id="62687-193">Para a opção 3-ID de opção DHCP, o cliente consultará a ID de opção de DHCP 234 e usará o valor de GUID retornado como a ID de grupo.</span><span class="sxs-lookup"><span data-stu-id="62687-193">For option 3 - DHCP Option ID, the client will query DHCP Option ID 234 and use the returned GUID value as the Group ID.</span></span>|
|<span data-ttu-id="62687-194">bandwidthmode</span><span class="sxs-lookup"><span data-stu-id="62687-194">bandwidthMode</span></span>|[<span data-ttu-id="62687-195">deliveryOptimizationBandwidth</span><span class="sxs-lookup"><span data-stu-id="62687-195">deliveryOptimizationBandwidth</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|<span data-ttu-id="62687-196">Especifica o uso de largura de banda em primeiro plano e plano de fundo usando porcentagens, absolutas ou horas.</span><span class="sxs-lookup"><span data-stu-id="62687-196">Specifies foreground and background bandwidth usage using percentages, absolutes, or hours.</span></span>|
|<span data-ttu-id="62687-197">backgroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="62687-197">backgroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="62687-198">Int64</span><span class="sxs-lookup"><span data-stu-id="62687-198">Int64</span></span>|<span data-ttu-id="62687-199">Especifica o número de segundos para atrasar uma origem HTTP em um download em segundo plano que tenha permissão para usar ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="62687-199">Specifies number of seconds to delay an HTTP source in a background download that is allowed to use peer-to-peer.</span></span> <span data-ttu-id="62687-200">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="62687-200">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="62687-201">foregroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="62687-201">foregroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="62687-202">Int64</span><span class="sxs-lookup"><span data-stu-id="62687-202">Int64</span></span>|<span data-ttu-id="62687-203">Especifica o número de segundos para atrasar uma origem HTTP em um download de primeiro plano que tenha permissão para usar ponto a ponto (0-86400).</span><span class="sxs-lookup"><span data-stu-id="62687-203">Specifies number of seconds to delay an HTTP source in a foreground download that is allowed to use peer-to-peer (0-86400).</span></span> <span data-ttu-id="62687-204">Valores válidos de 0 a 86400</span><span class="sxs-lookup"><span data-stu-id="62687-204">Valid values 0 to 86400</span></span>
<span data-ttu-id="62687-205">A especificação de 0 define a otimização de entrega para gerenciar essa configuração usando o serviço de nuvem.</span><span class="sxs-lookup"><span data-stu-id="62687-205">Specifying 0 sets Delivery Optimization to manage this setting using the cloud service.</span></span> <span data-ttu-id="62687-206">Valores válidos de 0 a 86400</span><span class="sxs-lookup"><span data-stu-id="62687-206">Valid values 0 to 86400</span></span>|
|<span data-ttu-id="62687-207">minimumRamAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="62687-207">minimumRamAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="62687-208">Int32</span><span class="sxs-lookup"><span data-stu-id="62687-208">Int32</span></span>|<span data-ttu-id="62687-209">Especifica o tamanho mínimo de RAM em GB para usar o cache de par (1-100000).</span><span class="sxs-lookup"><span data-stu-id="62687-209">Specifies the minimum RAM size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="62687-210">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="62687-210">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="62687-211">minimumDiskSizeAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="62687-211">minimumDiskSizeAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="62687-212">Int32</span><span class="sxs-lookup"><span data-stu-id="62687-212">Int32</span></span>|<span data-ttu-id="62687-213">Especifica o tamanho mínimo do disco em GB para usar o cache de par (1-100000).</span><span class="sxs-lookup"><span data-stu-id="62687-213">Specifies the minimum disk size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="62687-214">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="62687-214">Valid values 1 to 100000</span></span>
<span data-ttu-id="62687-215">Valores recomendados: 64 GB a 256 GB.</span><span class="sxs-lookup"><span data-stu-id="62687-215">Recommended values: 64 GB to 256 GB.</span></span> <span data-ttu-id="62687-216">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="62687-216">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="62687-217">minimumFileSizeToCacheInMegabytes</span><span class="sxs-lookup"><span data-stu-id="62687-217">minimumFileSizeToCacheInMegabytes</span></span>|<span data-ttu-id="62687-218">Int32</span><span class="sxs-lookup"><span data-stu-id="62687-218">Int32</span></span>|<span data-ttu-id="62687-219">Especifica o tamanho mínimo do arquivo de conteúdo em MB habilitado para usar o cache de ponto (1-100000).</span><span class="sxs-lookup"><span data-stu-id="62687-219">Specifies the minimum content file size in MB enabled to use Peer Caching (1-100000).</span></span> <span data-ttu-id="62687-220">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="62687-220">Valid values 1 to 100000</span></span>
<span data-ttu-id="62687-221">Valores recomendados: 1 MB a 100.000 MB.</span><span class="sxs-lookup"><span data-stu-id="62687-221">Recommended values: 1 MB to 100,000 MB.</span></span> <span data-ttu-id="62687-222">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="62687-222">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="62687-223">minimumBatteryPercentageAllowedToUpload</span><span class="sxs-lookup"><span data-stu-id="62687-223">minimumBatteryPercentageAllowedToUpload</span></span>|<span data-ttu-id="62687-224">Int32</span><span class="sxs-lookup"><span data-stu-id="62687-224">Int32</span></span>|<span data-ttu-id="62687-225">Especifica a porcentagem de bateria mínima para permitir que o dispositivo carregue dados (0-100).</span><span class="sxs-lookup"><span data-stu-id="62687-225">Specifies the minimum battery percentage to allow the device to upload data (0-100).</span></span> <span data-ttu-id="62687-226">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="62687-226">Valid values 0 to 100</span></span>
<span data-ttu-id="62687-227">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="62687-227">The default value is 0.</span></span> <span data-ttu-id="62687-228">O valor 0 (zero) significa "não limitado" e o valor padrão do serviço de nuvem será usado.</span><span class="sxs-lookup"><span data-stu-id="62687-228">The value 0 (zero) means "not limited" and the cloud service default value will be used.</span></span> <span data-ttu-id="62687-229">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="62687-229">Valid values 0 to 100</span></span>|
|<span data-ttu-id="62687-230">modifyCacheLocation</span><span class="sxs-lookup"><span data-stu-id="62687-230">modifyCacheLocation</span></span>|<span data-ttu-id="62687-231">String</span><span class="sxs-lookup"><span data-stu-id="62687-231">String</span></span>|<span data-ttu-id="62687-232">Especifica a unidade que a otimização de entrega deve usar para seu cache.</span><span class="sxs-lookup"><span data-stu-id="62687-232">Specifies the drive that Delivery Optimization should use for its cache.</span></span>|
|<span data-ttu-id="62687-233">maximumCacheAgeInDays</span><span class="sxs-lookup"><span data-stu-id="62687-233">maximumCacheAgeInDays</span></span>|<span data-ttu-id="62687-234">Int32</span><span class="sxs-lookup"><span data-stu-id="62687-234">Int32</span></span>|<span data-ttu-id="62687-235">Especifica o tempo máximo, em dias, em que cada arquivo é mantido no cache de otimização de entrega após o download bem-sucedido (0-3650).</span><span class="sxs-lookup"><span data-stu-id="62687-235">Specifies the maximum time in days that each file is held in the Delivery Optimization cache after downloading successfully (0-3650).</span></span> <span data-ttu-id="62687-236">Valores válidos de 0 a 3650</span><span class="sxs-lookup"><span data-stu-id="62687-236">Valid values 0 to 3650</span></span>|
|<span data-ttu-id="62687-237">maximumCacheSize</span><span class="sxs-lookup"><span data-stu-id="62687-237">maximumCacheSize</span></span>|[<span data-ttu-id="62687-238">deliveryOptimizationMaxCacheSize</span><span class="sxs-lookup"><span data-stu-id="62687-238">deliveryOptimizationMaxCacheSize</span></span>](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|<span data-ttu-id="62687-239">Especifica o tamanho máximo de cache que a otimização de entrega como uma porcentagem ou em GB.</span><span class="sxs-lookup"><span data-stu-id="62687-239">Specifies the maximum cache size that Delivery Optimization either as a percentage or in GB.</span></span>|
|<span data-ttu-id="62687-240">vpnPeerCaching</span><span class="sxs-lookup"><span data-stu-id="62687-240">vpnPeerCaching</span></span>|[<span data-ttu-id="62687-241">habilitação</span><span class="sxs-lookup"><span data-stu-id="62687-241">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="62687-242">Especifica se o dispositivo tem permissão para participar do cache de mesmo nível enquanto conectado via VPN à rede de domínio.</span><span class="sxs-lookup"><span data-stu-id="62687-242">Specifies whether the device is allowed to participate in Peer Caching while connected via VPN to the domain network.</span></span> <span data-ttu-id="62687-243">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="62687-243">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="62687-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="62687-244">Response</span></span>
<span data-ttu-id="62687-245">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62687-245">If successful, this method returns a `200 OK` response code and an updated [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62687-246">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62687-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="62687-247">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62687-247">Request</span></span>
<span data-ttu-id="62687-248">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62687-248">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1833

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
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
  "deliveryOptimizationMode": "httpOnly",
  "restrictPeerSelectionBy": "subnetMask",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 8,
  "foregroundDownloadFromHttpDelayInSeconds": 8,
  "minimumRamAllowedToPeerInGigabytes": 2,
  "minimumDiskSizeAllowedToPeerInGigabytes": 7,
  "minimumFileSizeToCacheInMegabytes": 1,
  "minimumBatteryPercentageAllowedToUpload": 7,
  "modifyCacheLocation": "Modify Cache Location value",
  "maximumCacheAgeInDays": 5,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="62687-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="62687-249">Response</span></span>
<span data-ttu-id="62687-p128">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62687-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2005

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
  "id": "5954ee9b-ee9b-5954-9bee-54599bee5459",
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
  "deliveryOptimizationMode": "httpOnly",
  "restrictPeerSelectionBy": "subnetMask",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 8,
  "foregroundDownloadFromHttpDelayInSeconds": 8,
  "minimumRamAllowedToPeerInGigabytes": 2,
  "minimumDiskSizeAllowedToPeerInGigabytes": 7,
  "minimumFileSizeToCacheInMegabytes": 1,
  "minimumBatteryPercentageAllowedToUpload": 7,
  "modifyCacheLocation": "Modify Cache Location value",
  "maximumCacheAgeInDays": 5,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "enabled"
}
```





