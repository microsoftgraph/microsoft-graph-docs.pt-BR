---
title: Atualizar windowsDeliveryOptimizationConfiguration
description: Atualiza as propriedades de um objeto windowsDeliveryOptimizationConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6a22af14d9cb9991f144c6df22680a1bcb0747b9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49286566"
---
# <a name="update-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="a09f2-103">Atualizar windowsDeliveryOptimizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a09f2-103">Update windowsDeliveryOptimizationConfiguration</span></span>

<span data-ttu-id="a09f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a09f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a09f2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a09f2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a09f2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a09f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a09f2-107">Atualiza as propriedades de um objeto [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a09f2-107">Update the properties of a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a09f2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a09f2-108">Prerequisites</span></span>
<span data-ttu-id="a09f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a09f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a09f2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a09f2-111">Permission type</span></span>|<span data-ttu-id="a09f2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a09f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a09f2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a09f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a09f2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a09f2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a09f2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a09f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a09f2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a09f2-116">Not supported.</span></span>|
|<span data-ttu-id="a09f2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a09f2-117">Application</span></span>|<span data-ttu-id="a09f2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a09f2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a09f2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a09f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a09f2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a09f2-120">Request headers</span></span>
|<span data-ttu-id="a09f2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a09f2-121">Header</span></span>|<span data-ttu-id="a09f2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a09f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a09f2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a09f2-123">Authorization</span></span>|<span data-ttu-id="a09f2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a09f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a09f2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a09f2-125">Accept</span></span>|<span data-ttu-id="a09f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a09f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a09f2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a09f2-127">Request body</span></span>
<span data-ttu-id="a09f2-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a09f2-128">In the request body, supply a JSON representation for the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

<span data-ttu-id="a09f2-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a09f2-129">The following table shows the properties that are required when you create the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md).</span></span>

|<span data-ttu-id="a09f2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a09f2-130">Property</span></span>|<span data-ttu-id="a09f2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a09f2-131">Type</span></span>|<span data-ttu-id="a09f2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a09f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a09f2-133">id</span><span class="sxs-lookup"><span data-stu-id="a09f2-133">id</span></span>|<span data-ttu-id="a09f2-134">String</span><span class="sxs-lookup"><span data-stu-id="a09f2-134">String</span></span>|<span data-ttu-id="a09f2-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a09f2-135">Key of the entity.</span></span> <span data-ttu-id="a09f2-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a09f2-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09f2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a09f2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a09f2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a09f2-138">DateTimeOffset</span></span>|<span data-ttu-id="a09f2-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a09f2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a09f2-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a09f2-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09f2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a09f2-141">roleScopeTagIds</span></span>|<span data-ttu-id="a09f2-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a09f2-142">String collection</span></span>|<span data-ttu-id="a09f2-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a09f2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a09f2-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a09f2-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09f2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a09f2-145">supportsScopeTags</span></span>|<span data-ttu-id="a09f2-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="a09f2-146">Boolean</span></span>|<span data-ttu-id="a09f2-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a09f2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a09f2-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a09f2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a09f2-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a09f2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a09f2-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a09f2-150">This property is read-only.</span></span> <span data-ttu-id="a09f2-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a09f2-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09f2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a09f2-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a09f2-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a09f2-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a09f2-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="a09f2-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a09f2-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a09f2-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09f2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a09f2-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a09f2-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a09f2-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a09f2-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="a09f2-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a09f2-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a09f2-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09f2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a09f2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a09f2-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a09f2-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a09f2-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="a09f2-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a09f2-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a09f2-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09f2-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a09f2-164">createdDateTime</span></span>|<span data-ttu-id="a09f2-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a09f2-165">DateTimeOffset</span></span>|<span data-ttu-id="a09f2-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a09f2-166">DateTime the object was created.</span></span> <span data-ttu-id="a09f2-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a09f2-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09f2-168">description</span><span class="sxs-lookup"><span data-stu-id="a09f2-168">description</span></span>|<span data-ttu-id="a09f2-169">String</span><span class="sxs-lookup"><span data-stu-id="a09f2-169">String</span></span>|<span data-ttu-id="a09f2-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a09f2-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a09f2-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a09f2-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09f2-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a09f2-172">displayName</span></span>|<span data-ttu-id="a09f2-173">String</span><span class="sxs-lookup"><span data-stu-id="a09f2-173">String</span></span>|<span data-ttu-id="a09f2-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a09f2-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a09f2-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a09f2-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09f2-176">versão</span><span class="sxs-lookup"><span data-stu-id="a09f2-176">version</span></span>|<span data-ttu-id="a09f2-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a09f2-177">Int32</span></span>|<span data-ttu-id="a09f2-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a09f2-178">Version of the device configuration.</span></span> <span data-ttu-id="a09f2-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a09f2-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09f2-180">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="a09f2-180">deliveryOptimizationMode</span></span>|[<span data-ttu-id="a09f2-181">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="a09f2-181">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="a09f2-182">Especifica o método de download que a otimização de entrega pode usar para gerenciar o consumo de largura de banda de rede para grandes cenários de distribuição de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="a09f2-182">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="a09f2-183">Os valores possíveis são: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="a09f2-183">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="a09f2-184">restrictPeerSelectionBy</span><span class="sxs-lookup"><span data-stu-id="a09f2-184">restrictPeerSelectionBy</span></span>|[<span data-ttu-id="a09f2-185">deliveryOptimizationRestrictPeerSelectionByOptions</span><span class="sxs-lookup"><span data-stu-id="a09f2-185">deliveryOptimizationRestrictPeerSelectionByOptions</span></span>](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|<span data-ttu-id="a09f2-186">Especifica a restrição da seleção de pares por meio da opção selecionada.</span><span class="sxs-lookup"><span data-stu-id="a09f2-186">Specifies to restrict peer selection via selected option.</span></span>
<span data-ttu-id="a09f2-187">A opção 1 (máscara de sub-rede) só se aplica aos modos de otimização de entrega LAN do modo de download (1) e grupo (2).</span><span class="sxs-lookup"><span data-stu-id="a09f2-187">Option 1 (Subnet mask) only applies to Delivery Optimization modes Download Mode LAN (1) and Group (2).</span></span> <span data-ttu-id="a09f2-188">Os valores possíveis são: `notConfigured` e `subnetMask`.</span><span class="sxs-lookup"><span data-stu-id="a09f2-188">Possible values are: `notConfigured`, `subnetMask`.</span></span>|
|<span data-ttu-id="a09f2-189">groupIdSource</span><span class="sxs-lookup"><span data-stu-id="a09f2-189">groupIdSource</span></span>|[<span data-ttu-id="a09f2-190">deliveryOptimizationGroupIdSource</span><span class="sxs-lookup"><span data-stu-id="a09f2-190">deliveryOptimizationGroupIdSource</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|<span data-ttu-id="a09f2-191">Especifica a restrição da seleção de par para uma fonte específicas.</span><span class="sxs-lookup"><span data-stu-id="a09f2-191">Specifies to restrict peer selection to a specfic source.</span></span>
<span data-ttu-id="a09f2-192">As opções definidas nesta política se aplicam apenas ao modo de download grupo (2) do modo de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="a09f2-192">The options set in this policy only apply to Delivery Optimization mode Group (2) download mode.</span></span> <span data-ttu-id="a09f2-193">Se o grupo (2) não estiver definido como modo de download, esta política será ignorada.</span><span class="sxs-lookup"><span data-stu-id="a09f2-193">If Group (2) isn't set as Download mode, this policy will be ignored.</span></span> <span data-ttu-id="a09f2-194">Para a opção 3-ID de opção DHCP, o cliente consultará a ID de opção de DHCP 234 e usará o valor de GUID retornado como a ID de grupo.</span><span class="sxs-lookup"><span data-stu-id="a09f2-194">For option 3 - DHCP Option ID, the client will query DHCP Option ID 234 and use the returned GUID value as the Group ID.</span></span>|
|<span data-ttu-id="a09f2-195">bandwidthmode</span><span class="sxs-lookup"><span data-stu-id="a09f2-195">bandwidthMode</span></span>|[<span data-ttu-id="a09f2-196">deliveryOptimizationBandwidth</span><span class="sxs-lookup"><span data-stu-id="a09f2-196">deliveryOptimizationBandwidth</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|<span data-ttu-id="a09f2-197">Especifica o uso de largura de banda em primeiro plano e plano de fundo usando porcentagens, absolutas ou horas.</span><span class="sxs-lookup"><span data-stu-id="a09f2-197">Specifies foreground and background bandwidth usage using percentages, absolutes, or hours.</span></span>|
|<span data-ttu-id="a09f2-198">backgroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="a09f2-198">backgroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="a09f2-199">Int64</span><span class="sxs-lookup"><span data-stu-id="a09f2-199">Int64</span></span>|<span data-ttu-id="a09f2-200">Especifica o número de segundos para atrasar uma origem HTTP em um download em segundo plano que tenha permissão para usar ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="a09f2-200">Specifies number of seconds to delay an HTTP source in a background download that is allowed to use peer-to-peer.</span></span> <span data-ttu-id="a09f2-201">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="a09f2-201">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="a09f2-202">foregroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="a09f2-202">foregroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="a09f2-203">Int64</span><span class="sxs-lookup"><span data-stu-id="a09f2-203">Int64</span></span>|<span data-ttu-id="a09f2-204">Especifica o número de segundos para atrasar uma origem HTTP em um download de primeiro plano que tenha permissão para usar ponto a ponto (0-86400).</span><span class="sxs-lookup"><span data-stu-id="a09f2-204">Specifies number of seconds to delay an HTTP source in a foreground download that is allowed to use peer-to-peer (0-86400).</span></span> <span data-ttu-id="a09f2-205">Valores válidos de 0 a 86400</span><span class="sxs-lookup"><span data-stu-id="a09f2-205">Valid values 0 to 86400</span></span>
<span data-ttu-id="a09f2-206">A especificação de 0 define a otimização de entrega para gerenciar essa configuração usando o serviço de nuvem.</span><span class="sxs-lookup"><span data-stu-id="a09f2-206">Specifying 0 sets Delivery Optimization to manage this setting using the cloud service.</span></span> <span data-ttu-id="a09f2-207">Valores válidos de 0 a 86400</span><span class="sxs-lookup"><span data-stu-id="a09f2-207">Valid values 0 to 86400</span></span>|
|<span data-ttu-id="a09f2-208">minimumRamAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="a09f2-208">minimumRamAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="a09f2-209">Int32</span><span class="sxs-lookup"><span data-stu-id="a09f2-209">Int32</span></span>|<span data-ttu-id="a09f2-210">Especifica o tamanho mínimo de RAM em GB para usar o cache de par (1-100000).</span><span class="sxs-lookup"><span data-stu-id="a09f2-210">Specifies the minimum RAM size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="a09f2-211">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="a09f2-211">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="a09f2-212">minimumDiskSizeAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="a09f2-212">minimumDiskSizeAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="a09f2-213">Int32</span><span class="sxs-lookup"><span data-stu-id="a09f2-213">Int32</span></span>|<span data-ttu-id="a09f2-214">Especifica o tamanho mínimo do disco em GB para usar o cache de par (1-100000).</span><span class="sxs-lookup"><span data-stu-id="a09f2-214">Specifies the minimum disk size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="a09f2-215">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="a09f2-215">Valid values 1 to 100000</span></span>
<span data-ttu-id="a09f2-216">Valores recomendados: 64 GB a 256 GB.</span><span class="sxs-lookup"><span data-stu-id="a09f2-216">Recommended values: 64 GB to 256 GB.</span></span> <span data-ttu-id="a09f2-217">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="a09f2-217">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="a09f2-218">minimumFileSizeToCacheInMegabytes</span><span class="sxs-lookup"><span data-stu-id="a09f2-218">minimumFileSizeToCacheInMegabytes</span></span>|<span data-ttu-id="a09f2-219">Int32</span><span class="sxs-lookup"><span data-stu-id="a09f2-219">Int32</span></span>|<span data-ttu-id="a09f2-220">Especifica o tamanho mínimo do arquivo de conteúdo em MB habilitado para usar o cache de ponto (1-100000).</span><span class="sxs-lookup"><span data-stu-id="a09f2-220">Specifies the minimum content file size in MB enabled to use Peer Caching (1-100000).</span></span> <span data-ttu-id="a09f2-221">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="a09f2-221">Valid values 1 to 100000</span></span>
<span data-ttu-id="a09f2-222">Valores recomendados: 1 MB a 100.000 MB.</span><span class="sxs-lookup"><span data-stu-id="a09f2-222">Recommended values: 1 MB to 100,000 MB.</span></span> <span data-ttu-id="a09f2-223">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="a09f2-223">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="a09f2-224">minimumBatteryPercentageAllowedToUpload</span><span class="sxs-lookup"><span data-stu-id="a09f2-224">minimumBatteryPercentageAllowedToUpload</span></span>|<span data-ttu-id="a09f2-225">Int32</span><span class="sxs-lookup"><span data-stu-id="a09f2-225">Int32</span></span>|<span data-ttu-id="a09f2-226">Especifica a porcentagem de bateria mínima para permitir que o dispositivo carregue dados (0-100).</span><span class="sxs-lookup"><span data-stu-id="a09f2-226">Specifies the minimum battery percentage to allow the device to upload data (0-100).</span></span> <span data-ttu-id="a09f2-227">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="a09f2-227">Valid values 0 to 100</span></span>
<span data-ttu-id="a09f2-228">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="a09f2-228">The default value is 0.</span></span> <span data-ttu-id="a09f2-229">O valor 0 (zero) significa "não limitado" e o valor padrão do serviço de nuvem será usado.</span><span class="sxs-lookup"><span data-stu-id="a09f2-229">The value 0 (zero) means "not limited" and the cloud service default value will be used.</span></span> <span data-ttu-id="a09f2-230">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="a09f2-230">Valid values 0 to 100</span></span>|
|<span data-ttu-id="a09f2-231">modifyCacheLocation</span><span class="sxs-lookup"><span data-stu-id="a09f2-231">modifyCacheLocation</span></span>|<span data-ttu-id="a09f2-232">String</span><span class="sxs-lookup"><span data-stu-id="a09f2-232">String</span></span>|<span data-ttu-id="a09f2-233">Especifica a unidade que a otimização de entrega deve usar para seu cache.</span><span class="sxs-lookup"><span data-stu-id="a09f2-233">Specifies the drive that Delivery Optimization should use for its cache.</span></span>|
|<span data-ttu-id="a09f2-234">maximumCacheAgeInDays</span><span class="sxs-lookup"><span data-stu-id="a09f2-234">maximumCacheAgeInDays</span></span>|<span data-ttu-id="a09f2-235">Int32</span><span class="sxs-lookup"><span data-stu-id="a09f2-235">Int32</span></span>|<span data-ttu-id="a09f2-236">Especifica o tempo máximo, em dias, em que cada arquivo é mantido no cache de otimização de entrega após o download bem-sucedido (0-3650).</span><span class="sxs-lookup"><span data-stu-id="a09f2-236">Specifies the maximum time in days that each file is held in the Delivery Optimization cache after downloading successfully (0-3650).</span></span> <span data-ttu-id="a09f2-237">Valores válidos de 0 a 3650</span><span class="sxs-lookup"><span data-stu-id="a09f2-237">Valid values 0 to 3650</span></span>|
|<span data-ttu-id="a09f2-238">maximumCacheSize</span><span class="sxs-lookup"><span data-stu-id="a09f2-238">maximumCacheSize</span></span>|[<span data-ttu-id="a09f2-239">deliveryOptimizationMaxCacheSize</span><span class="sxs-lookup"><span data-stu-id="a09f2-239">deliveryOptimizationMaxCacheSize</span></span>](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|<span data-ttu-id="a09f2-240">Especifica o tamanho máximo de cache que a otimização de entrega como uma porcentagem ou em GB.</span><span class="sxs-lookup"><span data-stu-id="a09f2-240">Specifies the maximum cache size that Delivery Optimization either as a percentage or in GB.</span></span>|
|<span data-ttu-id="a09f2-241">vpnPeerCaching</span><span class="sxs-lookup"><span data-stu-id="a09f2-241">vpnPeerCaching</span></span>|[<span data-ttu-id="a09f2-242">habilitação</span><span class="sxs-lookup"><span data-stu-id="a09f2-242">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a09f2-243">Especifica se o dispositivo tem permissão para participar do cache de mesmo nível enquanto conectado via VPN à rede de domínio.</span><span class="sxs-lookup"><span data-stu-id="a09f2-243">Specifies whether the device is allowed to participate in Peer Caching while connected via VPN to the domain network.</span></span> <span data-ttu-id="a09f2-244">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="a09f2-244">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a09f2-245">cacheServerHostNames</span><span class="sxs-lookup"><span data-stu-id="a09f2-245">cacheServerHostNames</span></span>|<span data-ttu-id="a09f2-246">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a09f2-246">String collection</span></span>|<span data-ttu-id="a09f2-247">Especifica nomes de host dos servidores de cache.</span><span class="sxs-lookup"><span data-stu-id="a09f2-247">Specifies cache servers host names.</span></span>|
|<span data-ttu-id="a09f2-248">cacheServerForegroundDownloadFallbackToHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="a09f2-248">cacheServerForegroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="a09f2-249">Int32</span><span class="sxs-lookup"><span data-stu-id="a09f2-249">Int32</span></span>|<span data-ttu-id="a09f2-250">Especifica o número de segundos para atrasar um retorno dos servidores de cache para uma fonte HTTP para um download de primeiro plano.</span><span class="sxs-lookup"><span data-stu-id="a09f2-250">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a foreground download.</span></span> <span data-ttu-id="a09f2-251">Valores válidos de 0 a 2592000.</span><span class="sxs-lookup"><span data-stu-id="a09f2-251">Valid values 0 to 2592000.</span></span>|
|<span data-ttu-id="a09f2-252">cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="a09f2-252">cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="a09f2-253">Int32</span><span class="sxs-lookup"><span data-stu-id="a09f2-253">Int32</span></span>|<span data-ttu-id="a09f2-254">Especifica o número de segundos para atrasar um retorno dos servidores de cache para uma origem HTTP para um download em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="a09f2-254">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a background download.</span></span> <span data-ttu-id="a09f2-255">Valores válidos de 0 a 2592000.</span><span class="sxs-lookup"><span data-stu-id="a09f2-255">Valid values 0 to 2592000.</span></span>|



## <a name="response"></a><span data-ttu-id="a09f2-256">Resposta</span><span class="sxs-lookup"><span data-stu-id="a09f2-256">Response</span></span>
<span data-ttu-id="a09f2-257">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a09f2-257">If successful, this method returns a `200 OK` response code and an updated [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a09f2-258">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a09f2-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="a09f2-259">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a09f2-259">Request</span></span>
<span data-ttu-id="a09f2-260">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a09f2-260">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2039

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
  "vpnPeerCaching": "enabled",
  "cacheServerHostNames": [
    "Cache Server Host Names value"
  ],
  "cacheServerForegroundDownloadFallbackToHttpDelayInSeconds": 9,
  "cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds": 9
}
```

### <a name="response"></a><span data-ttu-id="a09f2-261">Resposta</span><span class="sxs-lookup"><span data-stu-id="a09f2-261">Response</span></span>
<span data-ttu-id="a09f2-p130">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a09f2-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2211

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
  "vpnPeerCaching": "enabled",
  "cacheServerHostNames": [
    "Cache Server Host Names value"
  ],
  "cacheServerForegroundDownloadFallbackToHttpDelayInSeconds": 9,
  "cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds": 9
}
```




