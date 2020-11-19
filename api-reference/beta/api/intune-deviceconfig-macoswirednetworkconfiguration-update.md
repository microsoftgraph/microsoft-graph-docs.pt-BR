---
title: Atualizar macOSWiredNetworkConfiguration
description: Atualiza as propriedades de um objeto macOSWiredNetworkConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 009fa7036d0e671f84b217aa53ec679627d0828d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49264727"
---
# <a name="update-macoswirednetworkconfiguration"></a><span data-ttu-id="0ff9f-103">Atualizar macOSWiredNetworkConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ff9f-103">Update macOSWiredNetworkConfiguration</span></span>

<span data-ttu-id="0ff9f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ff9f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ff9f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ff9f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ff9f-107">Atualiza as propriedades de um objeto [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0ff9f-107">Update the properties of a [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ff9f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0ff9f-108">Prerequisites</span></span>
<span data-ttu-id="0ff9f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ff9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ff9f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ff9f-111">Permission type</span></span>|<span data-ttu-id="0ff9f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0ff9f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ff9f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ff9f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ff9f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ff9f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ff9f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ff9f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ff9f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-116">Not supported.</span></span>|
|<span data-ttu-id="0ff9f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ff9f-117">Application</span></span>|<span data-ttu-id="0ff9f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ff9f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ff9f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ff9f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0ff9f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ff9f-120">Request headers</span></span>
|<span data-ttu-id="0ff9f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ff9f-121">Header</span></span>|<span data-ttu-id="0ff9f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0ff9f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ff9f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ff9f-123">Authorization</span></span>|<span data-ttu-id="0ff9f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ff9f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0ff9f-125">Accept</span></span>|<span data-ttu-id="0ff9f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ff9f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ff9f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ff9f-127">Request body</span></span>
<span data-ttu-id="0ff9f-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0ff9f-128">In the request body, supply a JSON representation for the [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object.</span></span>

<span data-ttu-id="0ff9f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ff9f-129">The following table shows the properties that are required when you create the [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md).</span></span>

|<span data-ttu-id="0ff9f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ff9f-130">Property</span></span>|<span data-ttu-id="0ff9f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ff9f-131">Type</span></span>|<span data-ttu-id="0ff9f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ff9f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ff9f-133">id</span><span class="sxs-lookup"><span data-stu-id="0ff9f-133">id</span></span>|<span data-ttu-id="0ff9f-134">String</span><span class="sxs-lookup"><span data-stu-id="0ff9f-134">String</span></span>|<span data-ttu-id="0ff9f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-135">Key of the entity.</span></span> <span data-ttu-id="0ff9f-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ff9f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ff9f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ff9f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0ff9f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ff9f-138">DateTimeOffset</span></span>|<span data-ttu-id="0ff9f-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0ff9f-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ff9f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ff9f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0ff9f-141">roleScopeTagIds</span></span>|<span data-ttu-id="0ff9f-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ff9f-142">String collection</span></span>|<span data-ttu-id="0ff9f-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0ff9f-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ff9f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ff9f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0ff9f-145">supportsScopeTags</span></span>|<span data-ttu-id="0ff9f-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ff9f-146">Boolean</span></span>|<span data-ttu-id="0ff9f-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0ff9f-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0ff9f-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0ff9f-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-150">This property is read-only.</span></span> <span data-ttu-id="0ff9f-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ff9f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ff9f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0ff9f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0ff9f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0ff9f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0ff9f-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0ff9f-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ff9f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ff9f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0ff9f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0ff9f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0ff9f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0ff9f-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0ff9f-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ff9f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ff9f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0ff9f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0ff9f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0ff9f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0ff9f-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0ff9f-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ff9f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ff9f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ff9f-164">createdDateTime</span></span>|<span data-ttu-id="0ff9f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ff9f-165">DateTimeOffset</span></span>|<span data-ttu-id="0ff9f-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-166">DateTime the object was created.</span></span> <span data-ttu-id="0ff9f-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ff9f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ff9f-168">description</span><span class="sxs-lookup"><span data-stu-id="0ff9f-168">description</span></span>|<span data-ttu-id="0ff9f-169">String</span><span class="sxs-lookup"><span data-stu-id="0ff9f-169">String</span></span>|<span data-ttu-id="0ff9f-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0ff9f-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ff9f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ff9f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0ff9f-172">displayName</span></span>|<span data-ttu-id="0ff9f-173">String</span><span class="sxs-lookup"><span data-stu-id="0ff9f-173">String</span></span>|<span data-ttu-id="0ff9f-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0ff9f-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ff9f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ff9f-176">versão</span><span class="sxs-lookup"><span data-stu-id="0ff9f-176">version</span></span>|<span data-ttu-id="0ff9f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0ff9f-177">Int32</span></span>|<span data-ttu-id="0ff9f-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-178">Version of the device configuration.</span></span> <span data-ttu-id="0ff9f-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ff9f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ff9f-180">NetworkName</span><span class="sxs-lookup"><span data-stu-id="0ff9f-180">networkName</span></span>|<span data-ttu-id="0ff9f-181">String</span><span class="sxs-lookup"><span data-stu-id="0ff9f-181">String</span></span>|<span data-ttu-id="0ff9f-182">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="0ff9f-182">Network Name</span></span>|
|<span data-ttu-id="0ff9f-183">networkInterface</span><span class="sxs-lookup"><span data-stu-id="0ff9f-183">networkInterface</span></span>|[<span data-ttu-id="0ff9f-184">wiredNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="0ff9f-184">wiredNetworkInterface</span></span>](../resources/intune-deviceconfig-wirednetworkinterface.md)|<span data-ttu-id="0ff9f-185">Interface de rede.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-185">Network interface.</span></span> <span data-ttu-id="0ff9f-186">Os valores possíveis são: `anyEthernet`, `firstActiveEthernet`, `secondActiveEthernet`, `thirdActiveEthernet`, `firstEthernet`, `secondEthernet`, `thirdEthernet`.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-186">Possible values are: `anyEthernet`, `firstActiveEthernet`, `secondActiveEthernet`, `thirdActiveEthernet`, `firstEthernet`, `secondEthernet`, `thirdEthernet`.</span></span>|
|<span data-ttu-id="0ff9f-187">eapType</span><span class="sxs-lookup"><span data-stu-id="0ff9f-187">eapType</span></span>|[<span data-ttu-id="0ff9f-188">eapType</span><span class="sxs-lookup"><span data-stu-id="0ff9f-188">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="0ff9f-189">EAP (protocolo de autenticação extensível).</span><span class="sxs-lookup"><span data-stu-id="0ff9f-189">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="0ff9f-190">Indica o tipo de conjunto de protocolos EAP na rede com fio.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-190">Indicates the type of EAP protocol set on the wired network.</span></span> <span data-ttu-id="0ff9f-191">Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-191">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="0ff9f-192">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ff9f-192">eapFastConfiguration</span></span>|[<span data-ttu-id="0ff9f-193">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ff9f-193">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="0ff9f-194">Opção de configuração EAP-FAST quando EAP-FAST for o tipo de EAP selecionado.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-194">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="0ff9f-195">Os valores possíveis são: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-195">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="0ff9f-196">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="0ff9f-196">trustedServerCertificateNames</span></span>|<span data-ttu-id="0ff9f-197">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ff9f-197">String collection</span></span>|<span data-ttu-id="0ff9f-198">Nomes de certificados de servidor confiáveis quando o tipo EAP é configurado como EAP-TLS/TTLS/FAST ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-198">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="0ff9f-199">Este é o nome comum usado nos certificados emitidos pela autoridade de certificação (CA) confiável.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-199">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="0ff9f-200">Se você fornecer essas informações, poderá ignorar a caixa de diálogo de confiança dinâmica exibida em dispositivos de usuários finais quando eles se conectam a essa rede com fio.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-200">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this wired network.</span></span>|
|<span data-ttu-id="0ff9f-201">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0ff9f-201">authenticationMethod</span></span>|[<span data-ttu-id="0ff9f-202">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0ff9f-202">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="0ff9f-203">Método de autenticação quando o tipo EAP é configurado como PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-203">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="0ff9f-204">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-204">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="0ff9f-205">nonEapAuthenticationMethodForEapTtls</span><span class="sxs-lookup"><span data-stu-id="0ff9f-205">nonEapAuthenticationMethodForEapTtls</span></span>|[<span data-ttu-id="0ff9f-206">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="0ff9f-206">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="0ff9f-207">Método não EAP para autenticação (identidade interna) quando o tipo EAP é EAP-TTLS e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-207">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="0ff9f-208">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-208">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="0ff9f-209">enableOuterIdentityPrivacy</span><span class="sxs-lookup"><span data-stu-id="0ff9f-209">enableOuterIdentityPrivacy</span></span>|<span data-ttu-id="0ff9f-210">String</span><span class="sxs-lookup"><span data-stu-id="0ff9f-210">String</span></span>|<span data-ttu-id="0ff9f-211">Habilitar Privacidade de identidade (identidade externa) quando o tipo EAP é configurado como EAP-TTLS, EAP-FAST ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-211">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="0ff9f-212">Essa propriedade mascara os nomes de usernames com o texto inserido.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-212">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="0ff9f-213">Por exemplo, se você usar ' anônimo ', cada usuário que autenticar com essa rede com fio usando seu nome de usuário real será exibido como ' anônimo '.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-213">For example, if you use 'anonymous', each user that authenticates with this wired network using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="0ff9f-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ff9f-214">Response</span></span>
<span data-ttu-id="0ff9f-215">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-215">If successful, this method returns a `200 OK` response code and an updated [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ff9f-216">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ff9f-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ff9f-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ff9f-217">Request</span></span>
<span data-ttu-id="0ff9f-218">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-218">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1499

{
  "@odata.type": "#microsoft.graph.macOSWiredNetworkConfiguration",
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
  "networkName": "Network Name value",
  "networkInterface": "firstActiveEthernet",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "nonEapAuthenticationMethodForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "enableOuterIdentityPrivacy": "Enable Outer Identity Privacy value"
}
```

### <a name="response"></a><span data-ttu-id="0ff9f-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ff9f-219">Response</span></span>
<span data-ttu-id="0ff9f-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ff9f-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1671

{
  "@odata.type": "#microsoft.graph.macOSWiredNetworkConfiguration",
  "id": "e5a57519-7519-e5a5-1975-a5e51975a5e5",
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
  "networkName": "Network Name value",
  "networkInterface": "firstActiveEthernet",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "nonEapAuthenticationMethodForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "enableOuterIdentityPrivacy": "Enable Outer Identity Privacy value"
}
```




