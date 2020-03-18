---
title: Atualizar windows10NetworkBoundaryConfiguration
description: Atualiza as propriedades de um objeto windows10NetworkBoundaryConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4743c0b93ed42dbbbe5ce90aef22f7bbc806bf75
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42739023"
---
# <a name="update-windows10networkboundaryconfiguration"></a><span data-ttu-id="9f6b0-103">Atualizar windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="9f6b0-103">Update windows10NetworkBoundaryConfiguration</span></span>

> <span data-ttu-id="9f6b0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f6b0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f6b0-106">Atualiza as propriedades de um objeto [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9f6b0-106">Update the properties of a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f6b0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9f6b0-107">Prerequisites</span></span>
<span data-ttu-id="9f6b0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f6b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f6b0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f6b0-110">Permission type</span></span>|<span data-ttu-id="9f6b0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9f6b0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f6b0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f6b0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f6b0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f6b0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f6b0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f6b0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f6b0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-115">Not supported.</span></span>|
|<span data-ttu-id="9f6b0-116">Application</span><span class="sxs-lookup"><span data-stu-id="9f6b0-116">Application</span></span>|<span data-ttu-id="9f6b0-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f6b0-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f6b0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f6b0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9f6b0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f6b0-119">Request headers</span></span>
|<span data-ttu-id="9f6b0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9f6b0-120">Header</span></span>|<span data-ttu-id="9f6b0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9f6b0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f6b0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f6b0-122">Authorization</span></span>|<span data-ttu-id="9f6b0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f6b0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9f6b0-124">Accept</span></span>|<span data-ttu-id="9f6b0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f6b0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f6b0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f6b0-126">Request body</span></span>
<span data-ttu-id="9f6b0-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9f6b0-127">In the request body, supply a JSON representation for the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

<span data-ttu-id="9f6b0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f6b0-128">The following table shows the properties that are required when you create the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md).</span></span>

|<span data-ttu-id="9f6b0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f6b0-129">Property</span></span>|<span data-ttu-id="9f6b0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f6b0-130">Type</span></span>|<span data-ttu-id="9f6b0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f6b0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f6b0-132">id</span><span class="sxs-lookup"><span data-stu-id="9f6b0-132">id</span></span>|<span data-ttu-id="9f6b0-133">String</span><span class="sxs-lookup"><span data-stu-id="9f6b0-133">String</span></span>|<span data-ttu-id="9f6b0-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-134">Key of the entity.</span></span> <span data-ttu-id="9f6b0-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6b0-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6b0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f6b0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9f6b0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f6b0-137">DateTimeOffset</span></span>|<span data-ttu-id="9f6b0-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9f6b0-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6b0-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6b0-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9f6b0-140">roleScopeTagIds</span></span>|<span data-ttu-id="9f6b0-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f6b0-141">String collection</span></span>|<span data-ttu-id="9f6b0-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9f6b0-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6b0-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6b0-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9f6b0-144">supportsScopeTags</span></span>|<span data-ttu-id="9f6b0-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f6b0-145">Boolean</span></span>|<span data-ttu-id="9f6b0-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9f6b0-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9f6b0-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9f6b0-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-149">This property is read-only.</span></span> <span data-ttu-id="9f6b0-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6b0-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6b0-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9f6b0-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9f6b0-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9f6b0-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9f6b0-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9f6b0-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6b0-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6b0-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9f6b0-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9f6b0-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9f6b0-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9f6b0-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9f6b0-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6b0-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6b0-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9f6b0-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9f6b0-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9f6b0-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9f6b0-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9f6b0-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6b0-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6b0-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f6b0-163">createdDateTime</span></span>|<span data-ttu-id="9f6b0-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f6b0-164">DateTimeOffset</span></span>|<span data-ttu-id="9f6b0-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-165">DateTime the object was created.</span></span> <span data-ttu-id="9f6b0-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6b0-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6b0-167">description</span><span class="sxs-lookup"><span data-stu-id="9f6b0-167">description</span></span>|<span data-ttu-id="9f6b0-168">String</span><span class="sxs-lookup"><span data-stu-id="9f6b0-168">String</span></span>|<span data-ttu-id="9f6b0-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9f6b0-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6b0-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6b0-171">displayName</span><span class="sxs-lookup"><span data-stu-id="9f6b0-171">displayName</span></span>|<span data-ttu-id="9f6b0-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f6b0-172">String</span></span>|<span data-ttu-id="9f6b0-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9f6b0-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6b0-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6b0-175">versão</span><span class="sxs-lookup"><span data-stu-id="9f6b0-175">version</span></span>|<span data-ttu-id="9f6b0-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9f6b0-176">Int32</span></span>|<span data-ttu-id="9f6b0-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-177">Version of the device configuration.</span></span> <span data-ttu-id="9f6b0-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6b0-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6b0-179">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="9f6b0-179">windowsNetworkIsolationPolicy</span></span>|[<span data-ttu-id="9f6b0-180">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="9f6b0-180">windowsNetworkIsolationPolicy</span></span>](../resources/intune-deviceconfig-windowsnetworkisolationpolicy.md)|<span data-ttu-id="9f6b0-181">Política de isolamento de rede do Windows</span><span class="sxs-lookup"><span data-stu-id="9f6b0-181">Windows Network Isolation Policy</span></span>|



## <a name="response"></a><span data-ttu-id="9f6b0-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f6b0-182">Response</span></span>
<span data-ttu-id="9f6b0-183">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-183">If successful, this method returns a `200 OK` response code and an updated [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f6b0-184">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f6b0-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f6b0-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f6b0-185">Request</span></span>
<span data-ttu-id="9f6b0-186">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-186">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="9f6b0-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f6b0-187">Response</span></span>
<span data-ttu-id="9f6b0-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f6b0-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




