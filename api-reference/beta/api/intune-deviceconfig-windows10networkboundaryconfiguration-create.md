---
title: Criar windows10NetworkBoundaryConfiguration
description: Criar um novo objeto windows10NetworkBoundaryConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 94af228fe3a888e421dcd3e44ac64eeb7db9264e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43430570"
---
# <a name="create-windows10networkboundaryconfiguration"></a><span data-ttu-id="71dfb-103">Criar windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="71dfb-103">Create windows10NetworkBoundaryConfiguration</span></span>

<span data-ttu-id="71dfb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71dfb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71dfb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71dfb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71dfb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71dfb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71dfb-107">Criar um novo objeto [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="71dfb-107">Create a new [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71dfb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71dfb-108">Prerequisites</span></span>
<span data-ttu-id="71dfb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71dfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71dfb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71dfb-111">Permission type</span></span>|<span data-ttu-id="71dfb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="71dfb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71dfb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71dfb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71dfb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71dfb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71dfb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71dfb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71dfb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71dfb-116">Not supported.</span></span>|
|<span data-ttu-id="71dfb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71dfb-117">Application</span></span>|<span data-ttu-id="71dfb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71dfb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71dfb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71dfb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="71dfb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71dfb-120">Request headers</span></span>
|<span data-ttu-id="71dfb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71dfb-121">Header</span></span>|<span data-ttu-id="71dfb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="71dfb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71dfb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="71dfb-123">Authorization</span></span>|<span data-ttu-id="71dfb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71dfb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71dfb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="71dfb-125">Accept</span></span>|<span data-ttu-id="71dfb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71dfb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71dfb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71dfb-127">Request body</span></span>
<span data-ttu-id="71dfb-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10NetworkBoundaryConfiguration.</span><span class="sxs-lookup"><span data-stu-id="71dfb-128">In the request body, supply a JSON representation for the windows10NetworkBoundaryConfiguration object.</span></span>

<span data-ttu-id="71dfb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10NetworkBoundaryConfiguration.</span><span class="sxs-lookup"><span data-stu-id="71dfb-129">The following table shows the properties that are required when you create the windows10NetworkBoundaryConfiguration.</span></span>

|<span data-ttu-id="71dfb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71dfb-130">Property</span></span>|<span data-ttu-id="71dfb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="71dfb-131">Type</span></span>|<span data-ttu-id="71dfb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="71dfb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71dfb-133">id</span><span class="sxs-lookup"><span data-stu-id="71dfb-133">id</span></span>|<span data-ttu-id="71dfb-134">String</span><span class="sxs-lookup"><span data-stu-id="71dfb-134">String</span></span>|<span data-ttu-id="71dfb-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="71dfb-135">Key of the entity.</span></span> <span data-ttu-id="71dfb-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71dfb-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71dfb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71dfb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="71dfb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71dfb-138">DateTimeOffset</span></span>|<span data-ttu-id="71dfb-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="71dfb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="71dfb-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71dfb-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71dfb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="71dfb-141">roleScopeTagIds</span></span>|<span data-ttu-id="71dfb-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="71dfb-142">String collection</span></span>|<span data-ttu-id="71dfb-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="71dfb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="71dfb-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71dfb-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71dfb-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="71dfb-145">supportsScopeTags</span></span>|<span data-ttu-id="71dfb-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="71dfb-146">Boolean</span></span>|<span data-ttu-id="71dfb-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="71dfb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="71dfb-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="71dfb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="71dfb-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="71dfb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="71dfb-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71dfb-150">This property is read-only.</span></span> <span data-ttu-id="71dfb-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71dfb-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71dfb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="71dfb-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="71dfb-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="71dfb-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="71dfb-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="71dfb-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="71dfb-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71dfb-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71dfb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="71dfb-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="71dfb-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="71dfb-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="71dfb-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="71dfb-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="71dfb-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71dfb-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71dfb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="71dfb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="71dfb-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="71dfb-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="71dfb-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="71dfb-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="71dfb-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71dfb-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71dfb-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71dfb-164">createdDateTime</span></span>|<span data-ttu-id="71dfb-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71dfb-165">DateTimeOffset</span></span>|<span data-ttu-id="71dfb-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="71dfb-166">DateTime the object was created.</span></span> <span data-ttu-id="71dfb-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71dfb-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71dfb-168">description</span><span class="sxs-lookup"><span data-stu-id="71dfb-168">description</span></span>|<span data-ttu-id="71dfb-169">String</span><span class="sxs-lookup"><span data-stu-id="71dfb-169">String</span></span>|<span data-ttu-id="71dfb-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="71dfb-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="71dfb-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71dfb-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71dfb-172">displayName</span><span class="sxs-lookup"><span data-stu-id="71dfb-172">displayName</span></span>|<span data-ttu-id="71dfb-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71dfb-173">String</span></span>|<span data-ttu-id="71dfb-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="71dfb-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="71dfb-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71dfb-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71dfb-176">versão</span><span class="sxs-lookup"><span data-stu-id="71dfb-176">version</span></span>|<span data-ttu-id="71dfb-177">Int32</span><span class="sxs-lookup"><span data-stu-id="71dfb-177">Int32</span></span>|<span data-ttu-id="71dfb-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="71dfb-178">Version of the device configuration.</span></span> <span data-ttu-id="71dfb-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71dfb-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71dfb-180">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="71dfb-180">windowsNetworkIsolationPolicy</span></span>|[<span data-ttu-id="71dfb-181">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="71dfb-181">windowsNetworkIsolationPolicy</span></span>](../resources/intune-deviceconfig-windowsnetworkisolationpolicy.md)|<span data-ttu-id="71dfb-182">Política de isolamento de rede do Windows</span><span class="sxs-lookup"><span data-stu-id="71dfb-182">Windows Network Isolation Policy</span></span>|



## <a name="response"></a><span data-ttu-id="71dfb-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="71dfb-183">Response</span></span>
<span data-ttu-id="71dfb-184">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71dfb-184">If successful, this method returns a `201 Created` response code and a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71dfb-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71dfb-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="71dfb-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71dfb-186">Request</span></span>
<span data-ttu-id="71dfb-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71dfb-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2017

{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
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
  "windowsNetworkIsolationPolicy": {
    "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
    "enterpriseNetworkDomainNames": [
      "Enterprise Network Domain Names value"
    ],
    "enterpriseCloudResources": [
      {
        "@odata.type": "microsoft.graph.proxiedDomain",
        "ipAddressOrFQDN": "Ip Address Or FQDN value",
        "proxy": "Proxy value"
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.iPv6Range",
        "lowerAddress": "Lower Address value",
        "upperAddress": "Upper Address value"
      }
    ],
    "enterpriseInternalProxyServers": [
      "Enterprise Internal Proxy Servers value"
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      "Enterprise Proxy Servers value"
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      "Neutral Domain Resources value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="71dfb-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="71dfb-188">Response</span></span>
<span data-ttu-id="71dfb-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71dfb-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2189

{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
  "id": "afbc9e01-9e01-afbc-019e-bcaf019ebcaf",
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
  "windowsNetworkIsolationPolicy": {
    "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
    "enterpriseNetworkDomainNames": [
      "Enterprise Network Domain Names value"
    ],
    "enterpriseCloudResources": [
      {
        "@odata.type": "microsoft.graph.proxiedDomain",
        "ipAddressOrFQDN": "Ip Address Or FQDN value",
        "proxy": "Proxy value"
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.iPv6Range",
        "lowerAddress": "Lower Address value",
        "upperAddress": "Upper Address value"
      }
    ],
    "enterpriseInternalProxyServers": [
      "Enterprise Internal Proxy Servers value"
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      "Enterprise Proxy Servers value"
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      "Neutral Domain Resources value"
    ]
  }
}
```



