---
title: Atualizar macOSWiredNetworkConfiguration
description: Atualiza as propriedades de um objeto macOSWiredNetworkConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 787348435f34381a56965d7a752fae5fd7222a55
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38084199"
---
# <a name="update-macoswirednetworkconfiguration"></a><span data-ttu-id="47c47-103">Atualizar macOSWiredNetworkConfiguration</span><span class="sxs-lookup"><span data-stu-id="47c47-103">Update macOSWiredNetworkConfiguration</span></span>

> <span data-ttu-id="47c47-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="47c47-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47c47-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47c47-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47c47-106">Atualiza as propriedades de um objeto [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="47c47-106">Update the properties of a [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47c47-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="47c47-107">Prerequisites</span></span>
<span data-ttu-id="47c47-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47c47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47c47-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47c47-110">Permission type</span></span>|<span data-ttu-id="47c47-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="47c47-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47c47-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47c47-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47c47-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47c47-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47c47-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47c47-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47c47-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47c47-115">Not supported.</span></span>|
|<span data-ttu-id="47c47-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47c47-116">Application</span></span>|<span data-ttu-id="47c47-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47c47-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47c47-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47c47-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="47c47-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47c47-119">Request headers</span></span>
|<span data-ttu-id="47c47-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47c47-120">Header</span></span>|<span data-ttu-id="47c47-121">Valor</span><span class="sxs-lookup"><span data-stu-id="47c47-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47c47-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="47c47-122">Authorization</span></span>|<span data-ttu-id="47c47-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47c47-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47c47-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="47c47-124">Accept</span></span>|<span data-ttu-id="47c47-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47c47-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47c47-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47c47-126">Request body</span></span>
<span data-ttu-id="47c47-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="47c47-127">In the request body, supply a JSON representation for the [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object.</span></span>

<span data-ttu-id="47c47-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47c47-128">The following table shows the properties that are required when you create the [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md).</span></span>

|<span data-ttu-id="47c47-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47c47-129">Property</span></span>|<span data-ttu-id="47c47-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="47c47-130">Type</span></span>|<span data-ttu-id="47c47-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="47c47-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47c47-132">id</span><span class="sxs-lookup"><span data-stu-id="47c47-132">id</span></span>|<span data-ttu-id="47c47-133">String</span><span class="sxs-lookup"><span data-stu-id="47c47-133">String</span></span>|<span data-ttu-id="47c47-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="47c47-134">Key of the entity.</span></span> <span data-ttu-id="47c47-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47c47-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47c47-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47c47-136">lastModifiedDateTime</span></span>|<span data-ttu-id="47c47-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47c47-137">DateTimeOffset</span></span>|<span data-ttu-id="47c47-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="47c47-138">DateTime the object was last modified.</span></span> <span data-ttu-id="47c47-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47c47-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47c47-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="47c47-140">roleScopeTagIds</span></span>|<span data-ttu-id="47c47-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="47c47-141">String collection</span></span>|<span data-ttu-id="47c47-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="47c47-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="47c47-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47c47-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47c47-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="47c47-144">supportsScopeTags</span></span>|<span data-ttu-id="47c47-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="47c47-145">Boolean</span></span>|<span data-ttu-id="47c47-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="47c47-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="47c47-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="47c47-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="47c47-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="47c47-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="47c47-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="47c47-149">This property is read-only.</span></span> <span data-ttu-id="47c47-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47c47-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47c47-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="47c47-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="47c47-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="47c47-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="47c47-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="47c47-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="47c47-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47c47-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47c47-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="47c47-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="47c47-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="47c47-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="47c47-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="47c47-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="47c47-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47c47-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47c47-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="47c47-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="47c47-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="47c47-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="47c47-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="47c47-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="47c47-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47c47-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47c47-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47c47-163">createdDateTime</span></span>|<span data-ttu-id="47c47-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47c47-164">DateTimeOffset</span></span>|<span data-ttu-id="47c47-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="47c47-165">DateTime the object was created.</span></span> <span data-ttu-id="47c47-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47c47-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47c47-167">descrição</span><span class="sxs-lookup"><span data-stu-id="47c47-167">description</span></span>|<span data-ttu-id="47c47-168">String</span><span class="sxs-lookup"><span data-stu-id="47c47-168">String</span></span>|<span data-ttu-id="47c47-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47c47-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="47c47-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47c47-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47c47-171">displayName</span><span class="sxs-lookup"><span data-stu-id="47c47-171">displayName</span></span>|<span data-ttu-id="47c47-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47c47-172">String</span></span>|<span data-ttu-id="47c47-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47c47-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="47c47-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47c47-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47c47-175">versão</span><span class="sxs-lookup"><span data-stu-id="47c47-175">version</span></span>|<span data-ttu-id="47c47-176">Int32</span><span class="sxs-lookup"><span data-stu-id="47c47-176">Int32</span></span>|<span data-ttu-id="47c47-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47c47-177">Version of the device configuration.</span></span> <span data-ttu-id="47c47-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47c47-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47c47-179">NetworkName</span><span class="sxs-lookup"><span data-stu-id="47c47-179">networkName</span></span>|<span data-ttu-id="47c47-180">String</span><span class="sxs-lookup"><span data-stu-id="47c47-180">String</span></span>|<span data-ttu-id="47c47-181">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="47c47-181">Network Name</span></span>|
|<span data-ttu-id="47c47-182">networkInterface</span><span class="sxs-lookup"><span data-stu-id="47c47-182">networkInterface</span></span>|[<span data-ttu-id="47c47-183">wiredNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="47c47-183">wiredNetworkInterface</span></span>](../resources/intune-deviceconfig-wirednetworkinterface.md)|<span data-ttu-id="47c47-184">Interface de rede.</span><span class="sxs-lookup"><span data-stu-id="47c47-184">Network interface.</span></span> <span data-ttu-id="47c47-185">Os valores possíveis são: `anyEthernet`, `firstActiveEthernet`, `secondActiveEthernet`, `thirdActiveEthernet`, `firstEthernet`, `secondEthernet`, `thirdEthernet`.</span><span class="sxs-lookup"><span data-stu-id="47c47-185">Possible values are: `anyEthernet`, `firstActiveEthernet`, `secondActiveEthernet`, `thirdActiveEthernet`, `firstEthernet`, `secondEthernet`, `thirdEthernet`.</span></span>|
|<span data-ttu-id="47c47-186">eapType</span><span class="sxs-lookup"><span data-stu-id="47c47-186">eapType</span></span>|[<span data-ttu-id="47c47-187">eapType</span><span class="sxs-lookup"><span data-stu-id="47c47-187">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="47c47-188">EAP (protocolo de autenticação extensível).</span><span class="sxs-lookup"><span data-stu-id="47c47-188">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="47c47-189">Indica o tipo de conjunto de protocolos EAP na rede com fio.</span><span class="sxs-lookup"><span data-stu-id="47c47-189">Indicates the type of EAP protocol set on the wired network.</span></span> <span data-ttu-id="47c47-190">Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="47c47-190">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="47c47-191">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="47c47-191">eapFastConfiguration</span></span>|[<span data-ttu-id="47c47-192">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="47c47-192">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="47c47-193">Opção de configuração EAP-FAST quando EAP-FAST for o tipo de EAP selecionado.</span><span class="sxs-lookup"><span data-stu-id="47c47-193">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="47c47-194">Os valores possíveis são: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="47c47-194">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="47c47-195">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="47c47-195">trustedServerCertificateNames</span></span>|<span data-ttu-id="47c47-196">Coleção String</span><span class="sxs-lookup"><span data-stu-id="47c47-196">String collection</span></span>|<span data-ttu-id="47c47-197">Nomes de certificados de servidor confiáveis quando o tipo EAP é configurado como EAP-TLS/TTLS/FAST ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="47c47-197">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="47c47-198">Este é o nome comum usado nos certificados emitidos pela autoridade de certificação (CA) confiável.</span><span class="sxs-lookup"><span data-stu-id="47c47-198">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="47c47-199">Se você fornecer essas informações, poderá ignorar a caixa de diálogo de confiança dinâmica exibida em dispositivos de usuários finais quando eles se conectam a essa rede com fio.</span><span class="sxs-lookup"><span data-stu-id="47c47-199">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this wired network.</span></span>|
|<span data-ttu-id="47c47-200">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="47c47-200">authenticationMethod</span></span>|[<span data-ttu-id="47c47-201">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="47c47-201">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="47c47-202">Método de autenticação quando o tipo EAP é configurado como PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="47c47-202">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="47c47-203">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="47c47-203">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="47c47-204">nonEapAuthenticationMethodForEapTtls</span><span class="sxs-lookup"><span data-stu-id="47c47-204">nonEapAuthenticationMethodForEapTtls</span></span>|[<span data-ttu-id="47c47-205">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="47c47-205">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="47c47-206">Método não EAP para autenticação (identidade interna) quando o tipo EAP é EAP-TTLS e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="47c47-206">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="47c47-207">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="47c47-207">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="47c47-208">enableOuterIdentityPrivacy</span><span class="sxs-lookup"><span data-stu-id="47c47-208">enableOuterIdentityPrivacy</span></span>|<span data-ttu-id="47c47-209">String</span><span class="sxs-lookup"><span data-stu-id="47c47-209">String</span></span>|<span data-ttu-id="47c47-210">Habilitar Privacidade de identidade (identidade externa) quando o tipo EAP é configurado como EAP-TTLS, EAP-FAST ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="47c47-210">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="47c47-211">Essa propriedade mascara os nomes de usernames com o texto inserido.</span><span class="sxs-lookup"><span data-stu-id="47c47-211">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="47c47-212">Por exemplo, se você usar ' anônimo ', cada usuário que autenticar com essa rede com fio usando seu nome de usuário real será exibido como ' anônimo '.</span><span class="sxs-lookup"><span data-stu-id="47c47-212">For example, if you use 'anonymous', each user that authenticates with this wired network using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="47c47-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="47c47-213">Response</span></span>
<span data-ttu-id="47c47-214">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47c47-214">If successful, this method returns a `200 OK` response code and an updated [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47c47-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47c47-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="47c47-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47c47-216">Request</span></span>
<span data-ttu-id="47c47-217">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47c47-217">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="47c47-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="47c47-218">Response</span></span>
<span data-ttu-id="47c47-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47c47-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






