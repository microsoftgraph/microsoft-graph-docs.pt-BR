---
title: Criar macOSWiredNetworkConfiguration
description: Crie um novo objeto macOSWiredNetworkConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 91003cdb7b48da0271dcf83651628b4a3b5dde47
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131201"
---
# <a name="create-macoswirednetworkconfiguration"></a><span data-ttu-id="22439-103">Criar macOSWiredNetworkConfiguration</span><span class="sxs-lookup"><span data-stu-id="22439-103">Create macOSWiredNetworkConfiguration</span></span>

<span data-ttu-id="22439-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22439-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22439-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22439-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22439-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22439-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22439-107">Crie um novo [objeto macOSWiredNetworkConfiguration.](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22439-107">Create a new [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22439-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22439-108">Prerequisites</span></span>
<span data-ttu-id="22439-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22439-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22439-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22439-111">Permission type</span></span>|<span data-ttu-id="22439-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22439-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22439-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22439-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22439-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22439-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22439-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22439-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22439-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22439-116">Not supported.</span></span>|
|<span data-ttu-id="22439-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22439-117">Application</span></span>|<span data-ttu-id="22439-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22439-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22439-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22439-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="22439-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22439-120">Request headers</span></span>
|<span data-ttu-id="22439-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22439-121">Header</span></span>|<span data-ttu-id="22439-122">Valor</span><span class="sxs-lookup"><span data-stu-id="22439-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22439-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="22439-123">Authorization</span></span>|<span data-ttu-id="22439-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22439-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22439-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22439-125">Accept</span></span>|<span data-ttu-id="22439-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22439-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22439-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22439-127">Request body</span></span>
<span data-ttu-id="22439-128">No corpo da solicitação, fornece uma representação JSON para o objeto macOSWiredNetworkConfiguration.</span><span class="sxs-lookup"><span data-stu-id="22439-128">In the request body, supply a JSON representation for the macOSWiredNetworkConfiguration object.</span></span>

<span data-ttu-id="22439-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o macOSWiredNetworkConfiguration.</span><span class="sxs-lookup"><span data-stu-id="22439-129">The following table shows the properties that are required when you create the macOSWiredNetworkConfiguration.</span></span>

|<span data-ttu-id="22439-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22439-130">Property</span></span>|<span data-ttu-id="22439-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="22439-131">Type</span></span>|<span data-ttu-id="22439-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="22439-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22439-133">id</span><span class="sxs-lookup"><span data-stu-id="22439-133">id</span></span>|<span data-ttu-id="22439-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22439-134">String</span></span>|<span data-ttu-id="22439-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="22439-135">Key of the entity.</span></span> <span data-ttu-id="22439-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22439-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22439-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22439-137">lastModifiedDateTime</span></span>|<span data-ttu-id="22439-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22439-138">DateTimeOffset</span></span>|<span data-ttu-id="22439-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="22439-139">DateTime the object was last modified.</span></span> <span data-ttu-id="22439-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22439-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22439-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="22439-141">roleScopeTagIds</span></span>|<span data-ttu-id="22439-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="22439-142">String collection</span></span>|<span data-ttu-id="22439-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="22439-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="22439-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22439-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22439-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="22439-145">supportsScopeTags</span></span>|<span data-ttu-id="22439-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="22439-146">Boolean</span></span>|<span data-ttu-id="22439-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="22439-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="22439-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="22439-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="22439-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="22439-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="22439-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22439-150">This property is read-only.</span></span> <span data-ttu-id="22439-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22439-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22439-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="22439-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="22439-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="22439-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="22439-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="22439-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="22439-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22439-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22439-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="22439-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="22439-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="22439-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="22439-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="22439-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="22439-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22439-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22439-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="22439-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="22439-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="22439-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="22439-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="22439-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="22439-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22439-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22439-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22439-164">createdDateTime</span></span>|<span data-ttu-id="22439-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22439-165">DateTimeOffset</span></span>|<span data-ttu-id="22439-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="22439-166">DateTime the object was created.</span></span> <span data-ttu-id="22439-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22439-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22439-168">descrição</span><span class="sxs-lookup"><span data-stu-id="22439-168">description</span></span>|<span data-ttu-id="22439-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22439-169">String</span></span>|<span data-ttu-id="22439-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22439-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="22439-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22439-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22439-172">displayName</span><span class="sxs-lookup"><span data-stu-id="22439-172">displayName</span></span>|<span data-ttu-id="22439-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22439-173">String</span></span>|<span data-ttu-id="22439-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22439-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="22439-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22439-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22439-176">versão</span><span class="sxs-lookup"><span data-stu-id="22439-176">version</span></span>|<span data-ttu-id="22439-177">Int32</span><span class="sxs-lookup"><span data-stu-id="22439-177">Int32</span></span>|<span data-ttu-id="22439-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22439-178">Version of the device configuration.</span></span> <span data-ttu-id="22439-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22439-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22439-180">networkName</span><span class="sxs-lookup"><span data-stu-id="22439-180">networkName</span></span>|<span data-ttu-id="22439-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22439-181">String</span></span>|<span data-ttu-id="22439-182">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="22439-182">Network Name</span></span>|
|<span data-ttu-id="22439-183">networkInterface</span><span class="sxs-lookup"><span data-stu-id="22439-183">networkInterface</span></span>|[<span data-ttu-id="22439-184">wiredNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="22439-184">wiredNetworkInterface</span></span>](../resources/intune-deviceconfig-wirednetworkinterface.md)|<span data-ttu-id="22439-185">Interface de rede.</span><span class="sxs-lookup"><span data-stu-id="22439-185">Network interface.</span></span> <span data-ttu-id="22439-186">Os valores possíveis são: `anyEthernet`, `firstActiveEthernet`, `secondActiveEthernet`, `thirdActiveEthernet`, `firstEthernet`, `secondEthernet`, `thirdEthernet`.</span><span class="sxs-lookup"><span data-stu-id="22439-186">Possible values are: `anyEthernet`, `firstActiveEthernet`, `secondActiveEthernet`, `thirdActiveEthernet`, `firstEthernet`, `secondEthernet`, `thirdEthernet`.</span></span>|
|<span data-ttu-id="22439-187">eapType</span><span class="sxs-lookup"><span data-stu-id="22439-187">eapType</span></span>|[<span data-ttu-id="22439-188">eapType</span><span class="sxs-lookup"><span data-stu-id="22439-188">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="22439-189">Protocolo de Autenticação Extensível (EAP).</span><span class="sxs-lookup"><span data-stu-id="22439-189">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="22439-190">Indica o tipo de conjunto de protocoloSAP na rede com fio.</span><span class="sxs-lookup"><span data-stu-id="22439-190">Indicates the type of EAP protocol set on the wired network.</span></span> <span data-ttu-id="22439-191">Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="22439-191">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="22439-192">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="22439-192">eapFastConfiguration</span></span>|[<span data-ttu-id="22439-193">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="22439-193">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="22439-194">Opção de Configuração EAP-FAST quando EAP-FAST é o Tipo EAP selecionado.</span><span class="sxs-lookup"><span data-stu-id="22439-194">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="22439-195">Os valores possíveis são: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="22439-195">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="22439-196">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="22439-196">trustedServerCertificateNames</span></span>|<span data-ttu-id="22439-197">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="22439-197">String collection</span></span>|<span data-ttu-id="22439-198">Nomes de certificados de servidor confiáveis quando Tipo de EAP é configurado para EAP-TLS/TTLS/FAST ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="22439-198">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="22439-199">Esse é o nome comum usado nos certificados emitidos pela autoridade de certificação confiável (CA).</span><span class="sxs-lookup"><span data-stu-id="22439-199">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="22439-200">Se você fornecer essas informações, poderá ignorar a caixa de diálogo de confiança dinâmica exibida em dispositivos de usuários finais quando eles se conectarem a essa rede com fio.</span><span class="sxs-lookup"><span data-stu-id="22439-200">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this wired network.</span></span>|
|<span data-ttu-id="22439-201">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="22439-201">authenticationMethod</span></span>|[<span data-ttu-id="22439-202">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="22439-202">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="22439-203">Método de autenticação quando Tipo de EAP é configurado para PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="22439-203">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="22439-204">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="22439-204">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="22439-205">nonEapAuthenticationMethodForEapTtls</span><span class="sxs-lookup"><span data-stu-id="22439-205">nonEapAuthenticationMethodForEapTtls</span></span>|[<span data-ttu-id="22439-206">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="22439-206">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="22439-207">Método não EAP para Autenticação (Identidade Interna) quando Tipo de EAP é EAP-TTLS e Authenticationmethod é Nome de Usuário e Senha.</span><span class="sxs-lookup"><span data-stu-id="22439-207">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="22439-208">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="22439-208">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="22439-209">enableOuterIdentityPrivacy</span><span class="sxs-lookup"><span data-stu-id="22439-209">enableOuterIdentityPrivacy</span></span>|<span data-ttu-id="22439-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22439-210">String</span></span>|<span data-ttu-id="22439-211">Habilita a privacidade de identidade (Identidade Externa) quando o Tipo EAP estiver configurado para EAP-TTLS, EAP-FAST ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="22439-211">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="22439-212">Essa propriedade mascara os nomes de usuário com o texto que você inserir.</span><span class="sxs-lookup"><span data-stu-id="22439-212">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="22439-213">Por exemplo, se você usar "anônimo", cada usuário que se autentica com essa rede com fio usando seu nome de usuário real será exibido como "anônimo".</span><span class="sxs-lookup"><span data-stu-id="22439-213">For example, if you use 'anonymous', each user that authenticates with this wired network using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="22439-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="22439-214">Response</span></span>
<span data-ttu-id="22439-215">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22439-215">If successful, this method returns a `201 Created` response code and a [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22439-216">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22439-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="22439-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22439-217">Request</span></span>
<span data-ttu-id="22439-218">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22439-218">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="22439-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="22439-219">Response</span></span>
<span data-ttu-id="22439-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22439-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




