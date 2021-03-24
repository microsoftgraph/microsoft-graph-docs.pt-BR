---
title: Criar windowsDeliveryOptimizationConfiguration
description: Crie um novo objeto windowsDeliveryOptimizationConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 21298ccc592f2b80868bbe68393f5fdf9223f055
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132419"
---
# <a name="create-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="0e2b5-103">Criar windowsDeliveryOptimizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e2b5-103">Create windowsDeliveryOptimizationConfiguration</span></span>

<span data-ttu-id="0e2b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e2b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e2b5-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e2b5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e2b5-107">Crie um novo [objeto windowsDeliveryOptimizationConfiguration.](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e2b5-107">Create a new [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e2b5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0e2b5-108">Prerequisites</span></span>
<span data-ttu-id="0e2b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e2b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e2b5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e2b5-111">Permission type</span></span>|<span data-ttu-id="0e2b5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e2b5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e2b5-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e2b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e2b5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e2b5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e2b5-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e2b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e2b5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-116">Not supported.</span></span>|
|<span data-ttu-id="0e2b5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e2b5-117">Application</span></span>|<span data-ttu-id="0e2b5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e2b5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e2b5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e2b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0e2b5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e2b5-120">Request headers</span></span>
|<span data-ttu-id="0e2b5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0e2b5-121">Header</span></span>|<span data-ttu-id="0e2b5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0e2b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e2b5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e2b5-123">Authorization</span></span>|<span data-ttu-id="0e2b5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e2b5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0e2b5-125">Accept</span></span>|<span data-ttu-id="0e2b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e2b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e2b5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e2b5-127">Request body</span></span>
<span data-ttu-id="0e2b5-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsDeliveryOptimizationConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-128">In the request body, supply a JSON representation for the windowsDeliveryOptimizationConfiguration object.</span></span>

<span data-ttu-id="0e2b5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDeliveryOptimizationConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-129">The following table shows the properties that are required when you create the windowsDeliveryOptimizationConfiguration.</span></span>

|<span data-ttu-id="0e2b5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e2b5-130">Property</span></span>|<span data-ttu-id="0e2b5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e2b5-131">Type</span></span>|<span data-ttu-id="0e2b5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e2b5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e2b5-133">id</span><span class="sxs-lookup"><span data-stu-id="0e2b5-133">id</span></span>|<span data-ttu-id="0e2b5-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e2b5-134">String</span></span>|<span data-ttu-id="0e2b5-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-135">Key of the entity.</span></span> <span data-ttu-id="0e2b5-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e2b5-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e2b5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e2b5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0e2b5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e2b5-138">DateTimeOffset</span></span>|<span data-ttu-id="0e2b5-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0e2b5-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e2b5-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e2b5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0e2b5-141">roleScopeTagIds</span></span>|<span data-ttu-id="0e2b5-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e2b5-142">String collection</span></span>|<span data-ttu-id="0e2b5-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0e2b5-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e2b5-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e2b5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0e2b5-145">supportsScopeTags</span></span>|<span data-ttu-id="0e2b5-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="0e2b5-146">Boolean</span></span>|<span data-ttu-id="0e2b5-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0e2b5-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0e2b5-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0e2b5-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-150">This property is read-only.</span></span> <span data-ttu-id="0e2b5-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e2b5-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e2b5-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0e2b5-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0e2b5-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0e2b5-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0e2b5-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0e2b5-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e2b5-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e2b5-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0e2b5-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0e2b5-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0e2b5-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0e2b5-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0e2b5-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e2b5-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e2b5-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0e2b5-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0e2b5-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0e2b5-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0e2b5-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0e2b5-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e2b5-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e2b5-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e2b5-164">createdDateTime</span></span>|<span data-ttu-id="0e2b5-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e2b5-165">DateTimeOffset</span></span>|<span data-ttu-id="0e2b5-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-166">DateTime the object was created.</span></span> <span data-ttu-id="0e2b5-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e2b5-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e2b5-168">descrição</span><span class="sxs-lookup"><span data-stu-id="0e2b5-168">description</span></span>|<span data-ttu-id="0e2b5-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e2b5-169">String</span></span>|<span data-ttu-id="0e2b5-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0e2b5-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e2b5-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e2b5-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0e2b5-172">displayName</span></span>|<span data-ttu-id="0e2b5-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e2b5-173">String</span></span>|<span data-ttu-id="0e2b5-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0e2b5-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e2b5-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e2b5-176">versão</span><span class="sxs-lookup"><span data-stu-id="0e2b5-176">version</span></span>|<span data-ttu-id="0e2b5-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0e2b5-177">Int32</span></span>|<span data-ttu-id="0e2b5-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-178">Version of the device configuration.</span></span> <span data-ttu-id="0e2b5-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e2b5-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e2b5-180">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="0e2b5-180">deliveryOptimizationMode</span></span>|[<span data-ttu-id="0e2b5-181">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="0e2b5-181">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="0e2b5-182">Especifica o método de download que a otimização de entrega pode usar para gerenciar o consumo de largura de banda de rede para cenários de distribuição de conteúdo grandes.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-182">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="0e2b5-183">Os valores possíveis são: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-183">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="0e2b5-184">restrictPeerSelectionBy</span><span class="sxs-lookup"><span data-stu-id="0e2b5-184">restrictPeerSelectionBy</span></span>|[<span data-ttu-id="0e2b5-185">deliveryOptimizationRestrictPeerSelectionByOptions</span><span class="sxs-lookup"><span data-stu-id="0e2b5-185">deliveryOptimizationRestrictPeerSelectionByOptions</span></span>](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|<span data-ttu-id="0e2b5-186">Especifica restringir a seleção de pares por meio da opção selecionada.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-186">Specifies to restrict peer selection via selected option.</span></span>
<span data-ttu-id="0e2b5-187">A opção 1 (máscara de sub-rede) só se aplica aos modos de Otimização de Entrega LAN (1) e Grupo (2).</span><span class="sxs-lookup"><span data-stu-id="0e2b5-187">Option 1 (Subnet mask) only applies to Delivery Optimization modes Download Mode LAN (1) and Group (2).</span></span> <span data-ttu-id="0e2b5-188">Os valores possíveis são: `notConfigured` e `subnetMask`.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-188">Possible values are: `notConfigured`, `subnetMask`.</span></span>|
|<span data-ttu-id="0e2b5-189">groupIdSource</span><span class="sxs-lookup"><span data-stu-id="0e2b5-189">groupIdSource</span></span>|[<span data-ttu-id="0e2b5-190">deliveryOptimizationGroupIdSource</span><span class="sxs-lookup"><span data-stu-id="0e2b5-190">deliveryOptimizationGroupIdSource</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|<span data-ttu-id="0e2b5-191">Especifica restringir a seleção de pares a uma fonte especfic.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-191">Specifies to restrict peer selection to a specfic source.</span></span>
<span data-ttu-id="0e2b5-192">As opções definidas nesta política aplicam-se apenas ao modo de download do Modo de Otimização de Entrega (2).</span><span class="sxs-lookup"><span data-stu-id="0e2b5-192">The options set in this policy only apply to Delivery Optimization mode Group (2) download mode.</span></span> <span data-ttu-id="0e2b5-193">Se Group (2) não estiver definido como modo de download, essa política será ignorada.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-193">If Group (2) isn't set as Download mode, this policy will be ignored.</span></span> <span data-ttu-id="0e2b5-194">Para a opção 3 - ID da opção DHCP, o cliente consultará a ID da Opção DHCP 234 e usará o valor GUID retornado como a ID do Grupo.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-194">For option 3 - DHCP Option ID, the client will query DHCP Option ID 234 and use the returned GUID value as the Group ID.</span></span>|
|<span data-ttu-id="0e2b5-195">bandwidthMode</span><span class="sxs-lookup"><span data-stu-id="0e2b5-195">bandwidthMode</span></span>|[<span data-ttu-id="0e2b5-196">deliveryOptimizationBandwidth</span><span class="sxs-lookup"><span data-stu-id="0e2b5-196">deliveryOptimizationBandwidth</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|<span data-ttu-id="0e2b5-197">Especifica o uso da largura de banda em primeiro plano e em segundo plano usando porcentagens, absolutos ou horas.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-197">Specifies foreground and background bandwidth usage using percentages, absolutes, or hours.</span></span>|
|<span data-ttu-id="0e2b5-198">backgroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="0e2b5-198">backgroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="0e2b5-199">Int64</span><span class="sxs-lookup"><span data-stu-id="0e2b5-199">Int64</span></span>|<span data-ttu-id="0e2b5-200">Especifica o número de segundos para atrasar uma fonte HTTP em um download em segundo plano que tem permissão para usar ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-200">Specifies number of seconds to delay an HTTP source in a background download that is allowed to use peer-to-peer.</span></span> <span data-ttu-id="0e2b5-201">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="0e2b5-201">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="0e2b5-202">foregroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="0e2b5-202">foregroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="0e2b5-203">Int64</span><span class="sxs-lookup"><span data-stu-id="0e2b5-203">Int64</span></span>|<span data-ttu-id="0e2b5-204">Especifica o número de segundos para atrasar uma fonte HTTP em um download em primeiro plano que tem permissão para usar ponto a ponto (0-86400).</span><span class="sxs-lookup"><span data-stu-id="0e2b5-204">Specifies number of seconds to delay an HTTP source in a foreground download that is allowed to use peer-to-peer (0-86400).</span></span> <span data-ttu-id="0e2b5-205">Valores válidos de 0 a 86400</span><span class="sxs-lookup"><span data-stu-id="0e2b5-205">Valid values 0 to 86400</span></span>
<span data-ttu-id="0e2b5-206">A especificação 0 define a Otimização de Entrega para gerenciar essa configuração usando o serviço de nuvem.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-206">Specifying 0 sets Delivery Optimization to manage this setting using the cloud service.</span></span> <span data-ttu-id="0e2b5-207">Valores válidos de 0 a 86400</span><span class="sxs-lookup"><span data-stu-id="0e2b5-207">Valid values 0 to 86400</span></span>|
|<span data-ttu-id="0e2b5-208">minimumRamAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="0e2b5-208">minimumRamAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="0e2b5-209">Int32</span><span class="sxs-lookup"><span data-stu-id="0e2b5-209">Int32</span></span>|<span data-ttu-id="0e2b5-210">Especifica o tamanho mínimo de RAM em GB para usar Cache Par (1-100000).</span><span class="sxs-lookup"><span data-stu-id="0e2b5-210">Specifies the minimum RAM size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="0e2b5-211">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="0e2b5-211">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="0e2b5-212">minimumDiskSizeAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="0e2b5-212">minimumDiskSizeAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="0e2b5-213">Int32</span><span class="sxs-lookup"><span data-stu-id="0e2b5-213">Int32</span></span>|<span data-ttu-id="0e2b5-214">Especifica o tamanho mínimo do disco em GB para usar Cache Par (1-100000).</span><span class="sxs-lookup"><span data-stu-id="0e2b5-214">Specifies the minimum disk size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="0e2b5-215">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="0e2b5-215">Valid values 1 to 100000</span></span>
<span data-ttu-id="0e2b5-216">Valores recomendados: 64 GB a 256 GB.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-216">Recommended values: 64 GB to 256 GB.</span></span> <span data-ttu-id="0e2b5-217">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="0e2b5-217">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="0e2b5-218">minimumFileSizeToCacheInMegabytes</span><span class="sxs-lookup"><span data-stu-id="0e2b5-218">minimumFileSizeToCacheInMegabytes</span></span>|<span data-ttu-id="0e2b5-219">Int32</span><span class="sxs-lookup"><span data-stu-id="0e2b5-219">Int32</span></span>|<span data-ttu-id="0e2b5-220">Especifica o tamanho mínimo de arquivo de conteúdo em MB habilitado para usar Cache Par (1-100000).</span><span class="sxs-lookup"><span data-stu-id="0e2b5-220">Specifies the minimum content file size in MB enabled to use Peer Caching (1-100000).</span></span> <span data-ttu-id="0e2b5-221">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="0e2b5-221">Valid values 1 to 100000</span></span>
<span data-ttu-id="0e2b5-222">Valores recomendados: 1 MB a 100.000 MB.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-222">Recommended values: 1 MB to 100,000 MB.</span></span> <span data-ttu-id="0e2b5-223">Valores válidos de 1 a 100000</span><span class="sxs-lookup"><span data-stu-id="0e2b5-223">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="0e2b5-224">minimumBatteryPercentageAllowedToUpload</span><span class="sxs-lookup"><span data-stu-id="0e2b5-224">minimumBatteryPercentageAllowedToUpload</span></span>|<span data-ttu-id="0e2b5-225">Int32</span><span class="sxs-lookup"><span data-stu-id="0e2b5-225">Int32</span></span>|<span data-ttu-id="0e2b5-226">Especifica a porcentagem mínima de bateria para permitir que o dispositivo carregue dados (0-100).</span><span class="sxs-lookup"><span data-stu-id="0e2b5-226">Specifies the minimum battery percentage to allow the device to upload data (0-100).</span></span> <span data-ttu-id="0e2b5-227">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="0e2b5-227">Valid values 0 to 100</span></span>
<span data-ttu-id="0e2b5-228">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-228">The default value is 0.</span></span> <span data-ttu-id="0e2b5-229">O valor 0 (zero) significa "não limitado" e o valor padrão do serviço de nuvem será usado.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-229">The value 0 (zero) means "not limited" and the cloud service default value will be used.</span></span> <span data-ttu-id="0e2b5-230">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="0e2b5-230">Valid values 0 to 100</span></span>|
|<span data-ttu-id="0e2b5-231">modifyCacheLocation</span><span class="sxs-lookup"><span data-stu-id="0e2b5-231">modifyCacheLocation</span></span>|<span data-ttu-id="0e2b5-232">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e2b5-232">String</span></span>|<span data-ttu-id="0e2b5-233">Especifica a unidade que a Otimização de Entrega deve usar para seu cache.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-233">Specifies the drive that Delivery Optimization should use for its cache.</span></span>|
|<span data-ttu-id="0e2b5-234">maximumCacheAgeInDays</span><span class="sxs-lookup"><span data-stu-id="0e2b5-234">maximumCacheAgeInDays</span></span>|<span data-ttu-id="0e2b5-235">Int32</span><span class="sxs-lookup"><span data-stu-id="0e2b5-235">Int32</span></span>|<span data-ttu-id="0e2b5-236">Especifica o tempo máximo em dias em que cada arquivo é mantido no cache de Otimização de Entrega após o download com êxito (0-3650).</span><span class="sxs-lookup"><span data-stu-id="0e2b5-236">Specifies the maximum time in days that each file is held in the Delivery Optimization cache after downloading successfully (0-3650).</span></span> <span data-ttu-id="0e2b5-237">Valores válidos de 0 a 3650</span><span class="sxs-lookup"><span data-stu-id="0e2b5-237">Valid values 0 to 3650</span></span>|
|<span data-ttu-id="0e2b5-238">maximumCacheSize</span><span class="sxs-lookup"><span data-stu-id="0e2b5-238">maximumCacheSize</span></span>|[<span data-ttu-id="0e2b5-239">deliveryOptimizationMaxCacheSize</span><span class="sxs-lookup"><span data-stu-id="0e2b5-239">deliveryOptimizationMaxCacheSize</span></span>](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|<span data-ttu-id="0e2b5-240">Especifica o tamanho máximo de cache que a Otimização de Entrega como porcentagem ou em GB.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-240">Specifies the maximum cache size that Delivery Optimization either as a percentage or in GB.</span></span>|
|<span data-ttu-id="0e2b5-241">vpnPeerCaching</span><span class="sxs-lookup"><span data-stu-id="0e2b5-241">vpnPeerCaching</span></span>|[<span data-ttu-id="0e2b5-242">enablement</span><span class="sxs-lookup"><span data-stu-id="0e2b5-242">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="0e2b5-243">Especifica se o dispositivo tem permissão para participar do Cache Par enquanto estiver conectado via VPN à rede de domínio.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-243">Specifies whether the device is allowed to participate in Peer Caching while connected via VPN to the domain network.</span></span> <span data-ttu-id="0e2b5-244">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-244">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="0e2b5-245">cacheServerHostNames</span><span class="sxs-lookup"><span data-stu-id="0e2b5-245">cacheServerHostNames</span></span>|<span data-ttu-id="0e2b5-246">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e2b5-246">String collection</span></span>|<span data-ttu-id="0e2b5-247">Especifica nomes de host de servidores de cache.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-247">Specifies cache servers host names.</span></span>|
|<span data-ttu-id="0e2b5-248">cacheServerForegroundDownloadFallbackToHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="0e2b5-248">cacheServerForegroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="0e2b5-249">Int32</span><span class="sxs-lookup"><span data-stu-id="0e2b5-249">Int32</span></span>|<span data-ttu-id="0e2b5-250">Especifica o número de segundos para atrasar um retorno de servidores de cache para uma fonte HTTP para um download em primeiro plano.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-250">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a foreground download.</span></span> <span data-ttu-id="0e2b5-251">Valores válidos de 0 a 2592000.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-251">Valid values 0 to 2592000.</span></span>|
|<span data-ttu-id="0e2b5-252">cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="0e2b5-252">cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="0e2b5-253">Int32</span><span class="sxs-lookup"><span data-stu-id="0e2b5-253">Int32</span></span>|<span data-ttu-id="0e2b5-254">Especifica o número de segundos para atrasar um retorno de servidores de cache para uma fonte HTTP para um download em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-254">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a background download.</span></span> <span data-ttu-id="0e2b5-255">Valores válidos de 0 a 2592000.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-255">Valid values 0 to 2592000.</span></span>|



## <a name="response"></a><span data-ttu-id="0e2b5-256">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e2b5-256">Response</span></span>
<span data-ttu-id="0e2b5-257">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-257">If successful, this method returns a `201 Created` response code and a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e2b5-258">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e2b5-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e2b5-259">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e2b5-259">Request</span></span>
<span data-ttu-id="0e2b5-260">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-260">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="0e2b5-261">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e2b5-261">Response</span></span>
<span data-ttu-id="0e2b5-p130">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e2b5-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




