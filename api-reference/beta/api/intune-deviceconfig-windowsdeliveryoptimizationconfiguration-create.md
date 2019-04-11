---
title: Criar windowsDeliveryOptimizationConfiguration
description: Criar um novo objeto windowsDeliveryOptimizationConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c6f28105f10f412f9e289136d23a92377e7e38fe
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789168"
---
# <a name="create-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="39491-103">Criar windowsDeliveryOptimizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="39491-103">Create windowsDeliveryOptimizationConfiguration</span></span>

> <span data-ttu-id="39491-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="39491-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39491-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="39491-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39491-106">Criar um novo objeto [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="39491-106">Create a new [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39491-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="39491-107">Prerequisites</span></span>
<span data-ttu-id="39491-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39491-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39491-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39491-110">Permission type</span></span>|<span data-ttu-id="39491-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="39491-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39491-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39491-112">Delegated (work or school account)</span></span>|<span data-ttu-id="39491-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39491-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="39491-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39491-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39491-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39491-115">Not supported.</span></span>|
|<span data-ttu-id="39491-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39491-116">Application</span></span>|<span data-ttu-id="39491-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39491-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39491-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39491-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="39491-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39491-119">Request headers</span></span>
|<span data-ttu-id="39491-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="39491-120">Header</span></span>|<span data-ttu-id="39491-121">Valor</span><span class="sxs-lookup"><span data-stu-id="39491-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39491-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="39491-122">Authorization</span></span>|<span data-ttu-id="39491-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39491-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39491-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="39491-124">Accept</span></span>|<span data-ttu-id="39491-125">application/json</span><span class="sxs-lookup"><span data-stu-id="39491-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39491-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39491-126">Request body</span></span>
<span data-ttu-id="39491-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsDeliveryOptimizationConfiguration.</span><span class="sxs-lookup"><span data-stu-id="39491-127">In the request body, supply a JSON representation for the windowsDeliveryOptimizationConfiguration object.</span></span>

<span data-ttu-id="39491-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDeliveryOptimizationConfiguration.</span><span class="sxs-lookup"><span data-stu-id="39491-128">The following table shows the properties that are required when you create the windowsDeliveryOptimizationConfiguration.</span></span>

|<span data-ttu-id="39491-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39491-129">Property</span></span>|<span data-ttu-id="39491-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="39491-130">Type</span></span>|<span data-ttu-id="39491-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="39491-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39491-132">id</span><span class="sxs-lookup"><span data-stu-id="39491-132">id</span></span>|<span data-ttu-id="39491-133">String</span><span class="sxs-lookup"><span data-stu-id="39491-133">String</span></span>|<span data-ttu-id="39491-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="39491-134">Key of the entity.</span></span> <span data-ttu-id="39491-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39491-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39491-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39491-136">lastModifiedDateTime</span></span>|<span data-ttu-id="39491-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39491-137">DateTimeOffset</span></span>|<span data-ttu-id="39491-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="39491-138">DateTime the object was last modified.</span></span> <span data-ttu-id="39491-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39491-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39491-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="39491-140">roleScopeTagIds</span></span>|<span data-ttu-id="39491-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="39491-141">String collection</span></span>|<span data-ttu-id="39491-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="39491-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="39491-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39491-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39491-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="39491-144">supportsScopeTags</span></span>|<span data-ttu-id="39491-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="39491-145">Boolean</span></span>|<span data-ttu-id="39491-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="39491-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="39491-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="39491-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="39491-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="39491-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="39491-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="39491-149">This property is read-only.</span></span> <span data-ttu-id="39491-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39491-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39491-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39491-151">createdDateTime</span></span>|<span data-ttu-id="39491-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39491-152">DateTimeOffset</span></span>|<span data-ttu-id="39491-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="39491-153">DateTime the object was created.</span></span> <span data-ttu-id="39491-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39491-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39491-155">description</span><span class="sxs-lookup"><span data-stu-id="39491-155">description</span></span>|<span data-ttu-id="39491-156">String</span><span class="sxs-lookup"><span data-stu-id="39491-156">String</span></span>|<span data-ttu-id="39491-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="39491-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="39491-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39491-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39491-159">displayName</span><span class="sxs-lookup"><span data-stu-id="39491-159">displayName</span></span>|<span data-ttu-id="39491-160">String</span><span class="sxs-lookup"><span data-stu-id="39491-160">String</span></span>|<span data-ttu-id="39491-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="39491-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="39491-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39491-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39491-163">versão</span><span class="sxs-lookup"><span data-stu-id="39491-163">version</span></span>|<span data-ttu-id="39491-164">Int32</span><span class="sxs-lookup"><span data-stu-id="39491-164">Int32</span></span>|<span data-ttu-id="39491-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="39491-165">Version of the device configuration.</span></span> <span data-ttu-id="39491-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39491-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39491-167">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="39491-167">deliveryOptimizationMode</span></span>|[<span data-ttu-id="39491-168">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="39491-168">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="39491-169">Especifica o método de download que a otimização de entrega pode usar para gerenciar o consumo de largura de banda de rede para grandes cenários de distribuição de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="39491-169">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="39491-170">Os valores possíveis são: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="39491-170">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="39491-171">restrictPeerSelectionBy</span><span class="sxs-lookup"><span data-stu-id="39491-171">restrictPeerSelectionBy</span></span>|[<span data-ttu-id="39491-172">deliveryOptimizationRestrictPeerSelectionByOptions</span><span class="sxs-lookup"><span data-stu-id="39491-172">deliveryOptimizationRestrictPeerSelectionByOptions</span></span>](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|<span data-ttu-id="39491-173">Especifica a restrição da seleção de pares por meio da opção selecionada.</span><span class="sxs-lookup"><span data-stu-id="39491-173">Specifies to restrict peer selection via selected option.</span></span>
<span data-ttu-id="39491-174">A opção 1 (máscara de sub-rede) só se aplica aos modos de otimização de entrega LAN do modo de download (1) e grupo (2).</span><span class="sxs-lookup"><span data-stu-id="39491-174">Option 1 (Subnet mask) only applies to Delivery Optimization modes Download Mode LAN (1) and Group (2).</span></span> <span data-ttu-id="39491-175">Os valores possíveis são: `notConfigured` e `subnetMask`.</span><span class="sxs-lookup"><span data-stu-id="39491-175">Possible values are: `notConfigured`, `subnetMask`.</span></span>|
|<span data-ttu-id="39491-176">groupIdSource</span><span class="sxs-lookup"><span data-stu-id="39491-176">groupIdSource</span></span>|[<span data-ttu-id="39491-177">deliveryOptimizationGroupIdSource</span><span class="sxs-lookup"><span data-stu-id="39491-177">deliveryOptimizationGroupIdSource</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|<span data-ttu-id="39491-178">Especifica a restrição da seleção de par para uma fonte específicas.</span><span class="sxs-lookup"><span data-stu-id="39491-178">Specifies to restrict peer selection to a specfic source.</span></span>
<span data-ttu-id="39491-179">As opções definidas nesta política se aplicam apenas ao modo de download grupo (2) do modo de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="39491-179">The options set in this policy only apply to Delivery Optimization mode Group (2) download mode.</span></span> <span data-ttu-id="39491-180">Se o grupo (2) não estiver definido como modo de download, esta política será ignorada.</span><span class="sxs-lookup"><span data-stu-id="39491-180">If Group (2) isn't set as Download mode, this policy will be ignored.</span></span> <span data-ttu-id="39491-181">Para a opção 3-ID de opção DHCP, o cliente consultará a ID de opção de DHCP 234 e usará o valor de GUID retornado como a ID de grupo.</span><span class="sxs-lookup"><span data-stu-id="39491-181">For option 3 - DHCP Option ID, the client will query DHCP Option ID 234 and use the returned GUID value as the Group ID.</span></span>|
|<span data-ttu-id="39491-182">bandwidthmode</span><span class="sxs-lookup"><span data-stu-id="39491-182">bandwidthMode</span></span>|[<span data-ttu-id="39491-183">deliveryOptimizationBandwidth</span><span class="sxs-lookup"><span data-stu-id="39491-183">deliveryOptimizationBandwidth</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|<span data-ttu-id="39491-184">Especifica o uso de largura de banda em primeiro plano e plano de fundo usando porcentagens, absolutas ou horas.</span><span class="sxs-lookup"><span data-stu-id="39491-184">Specifies foreground and background bandwidth usage using percentages, absolutes, or hours.</span></span>|
|<span data-ttu-id="39491-185">backgroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="39491-185">backgroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="39491-186">Int64</span><span class="sxs-lookup"><span data-stu-id="39491-186">Int64</span></span>|<span data-ttu-id="39491-187">Especifica o número de segundos para atrasar uma origem HTTP em um download em segundo plano que tenha permissão para usar ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="39491-187">Specifies number of seconds to delay an HTTP source in a background download that is allowed to use peer-to-peer.</span></span> <span data-ttu-id="39491-188">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="39491-188">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="39491-189">foregroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="39491-189">foregroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="39491-190">Int64</span><span class="sxs-lookup"><span data-stu-id="39491-190">Int64</span></span>|<span data-ttu-id="39491-191">Especifica o número de segundos para atrasar uma origem HTTP em um download de primeiro plano que tenha permissão para usar ponto a ponto (0-86400).</span><span class="sxs-lookup"><span data-stu-id="39491-191">Specifies number of seconds to delay an HTTP source in a foreground download that is allowed to use peer-to-peer (0-86400).</span></span> <span data-ttu-id="39491-192">Valores válidos de 0 a 86400</span><span class="sxs-lookup"><span data-stu-id="39491-192">Valid values 0 to 86400</span></span>
<span data-ttu-id="39491-193">A especificação de 0 define a otimização de entrega para gerenciar essa configuração usando o serviço de nuvem.</span><span class="sxs-lookup"><span data-stu-id="39491-193">Specifying 0 sets Delivery Optimization to manage this setting using the cloud service.</span></span> <span data-ttu-id="39491-194">Valores válidos de 0 a 86400</span><span class="sxs-lookup"><span data-stu-id="39491-194">Valid values 0 to 86400</span></span>|
|<span data-ttu-id="39491-195">minimumRamAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="39491-195">minimumRamAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="39491-196">Int32</span><span class="sxs-lookup"><span data-stu-id="39491-196">Int32</span></span>|<span data-ttu-id="39491-197">Especifica o tamanho mínimo de RAM em GB para usar o cache de par (1-100000).</span><span class="sxs-lookup"><span data-stu-id="39491-197">Specifies the minimum RAM size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="39491-198">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="39491-198">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="39491-199">minimumDiskSizeAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="39491-199">minimumDiskSizeAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="39491-200">Int32</span><span class="sxs-lookup"><span data-stu-id="39491-200">Int32</span></span>|<span data-ttu-id="39491-201">Especifica o tamanho mínimo do disco em GB para usar o cache de par (1-100000).</span><span class="sxs-lookup"><span data-stu-id="39491-201">Specifies the minimum disk size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="39491-202">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="39491-202">Valid values 1 to 100000</span></span>
<span data-ttu-id="39491-203">Valores recomendados: 64 GB a 256 GB.</span><span class="sxs-lookup"><span data-stu-id="39491-203">Recommended values: 64 GB to 256 GB.</span></span> <span data-ttu-id="39491-204">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="39491-204">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="39491-205">minimumFileSizeToCacheInMegabytes</span><span class="sxs-lookup"><span data-stu-id="39491-205">minimumFileSizeToCacheInMegabytes</span></span>|<span data-ttu-id="39491-206">Int32</span><span class="sxs-lookup"><span data-stu-id="39491-206">Int32</span></span>|<span data-ttu-id="39491-207">Especifica o tamanho mínimo do arquivo de conteúdo em MB habilitado para usar o cache de ponto (1-100000).</span><span class="sxs-lookup"><span data-stu-id="39491-207">Specifies the minimum content file size in MB enabled to use Peer Caching (1-100000).</span></span> <span data-ttu-id="39491-208">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="39491-208">Valid values 1 to 100000</span></span>
<span data-ttu-id="39491-209">Valores recomendados: 1 MB a 100.000 MB.</span><span class="sxs-lookup"><span data-stu-id="39491-209">Recommended values: 1 MB to 100,000 MB.</span></span> <span data-ttu-id="39491-210">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="39491-210">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="39491-211">minimumBatteryPercentageAllowedToUpload</span><span class="sxs-lookup"><span data-stu-id="39491-211">minimumBatteryPercentageAllowedToUpload</span></span>|<span data-ttu-id="39491-212">Int32</span><span class="sxs-lookup"><span data-stu-id="39491-212">Int32</span></span>|<span data-ttu-id="39491-213">Especifica a porcentagem de bateria mínima para permitir que o dispositivo carregue dados (0-100).</span><span class="sxs-lookup"><span data-stu-id="39491-213">Specifies the minimum battery percentage to allow the device to upload data (0-100).</span></span> <span data-ttu-id="39491-214">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="39491-214">Valid values 0 to 100</span></span>
<span data-ttu-id="39491-215">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="39491-215">The default value is 0.</span></span> <span data-ttu-id="39491-216">O valor 0 (zero) significa "não limitado" e o valor padrão do serviço de nuvem será usado.</span><span class="sxs-lookup"><span data-stu-id="39491-216">The value 0 (zero) means "not limited" and the cloud service default value will be used.</span></span> <span data-ttu-id="39491-217">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="39491-217">Valid values 0 to 100</span></span>|
|<span data-ttu-id="39491-218">modifyCacheLocation</span><span class="sxs-lookup"><span data-stu-id="39491-218">modifyCacheLocation</span></span>|<span data-ttu-id="39491-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39491-219">String</span></span>|<span data-ttu-id="39491-220">Especifica a unidade que a otimização de entrega deve usar para seu cache.</span><span class="sxs-lookup"><span data-stu-id="39491-220">Specifies the drive that Delivery Optimization should use for its cache.</span></span>|
|<span data-ttu-id="39491-221">maximumCacheAgeInDays</span><span class="sxs-lookup"><span data-stu-id="39491-221">maximumCacheAgeInDays</span></span>|<span data-ttu-id="39491-222">Int32</span><span class="sxs-lookup"><span data-stu-id="39491-222">Int32</span></span>|<span data-ttu-id="39491-223">Especifica o tempo máximo, em dias, em que cada arquivo é mantido no cache de otimização de entrega após o download bem-sucedido (0-49710).</span><span class="sxs-lookup"><span data-stu-id="39491-223">Specifies the maximum time in days that each file is held in the Delivery Optimization cache after downloading successfully (0-49710).</span></span> <span data-ttu-id="39491-224">Valores válidos de 0 a 49710</span><span class="sxs-lookup"><span data-stu-id="39491-224">Valid values 0 to 49710</span></span>|
|<span data-ttu-id="39491-225">maximumCacheSize</span><span class="sxs-lookup"><span data-stu-id="39491-225">maximumCacheSize</span></span>|[<span data-ttu-id="39491-226">deliveryOptimizationMaxCacheSize</span><span class="sxs-lookup"><span data-stu-id="39491-226">deliveryOptimizationMaxCacheSize</span></span>](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|<span data-ttu-id="39491-227">Especifica o tamanho máximo de cache que a otimização de entrega como uma porcentagem ou em GB.</span><span class="sxs-lookup"><span data-stu-id="39491-227">Specifies the maximum cache size that Delivery Optimization either as a percentage or in GB.</span></span>|
|<span data-ttu-id="39491-228">vpnPeerCaching</span><span class="sxs-lookup"><span data-stu-id="39491-228">vpnPeerCaching</span></span>|[<span data-ttu-id="39491-229">habilitação</span><span class="sxs-lookup"><span data-stu-id="39491-229">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="39491-230">Especifica se o dispositivo tem permissão para participar do cache de mesmo nível enquanto conectado via VPN à rede de domínio.</span><span class="sxs-lookup"><span data-stu-id="39491-230">Specifies whether the device is allowed to participate in Peer Caching while connected via VPN to the domain network.</span></span> <span data-ttu-id="39491-231">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="39491-231">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="39491-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="39491-232">Response</span></span>
<span data-ttu-id="39491-233">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39491-233">If successful, this method returns a `201 Created` response code and a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39491-234">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39491-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="39491-235">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39491-235">Request</span></span>
<span data-ttu-id="39491-236">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="39491-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1060

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="39491-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="39491-237">Response</span></span>
<span data-ttu-id="39491-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="39491-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1232

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
  "id": "5954ee9b-ee9b-5954-9bee-54599bee5459",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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





