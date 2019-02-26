---
title: Atualizar windows10NetworkBoundaryConfiguration
description: Atualiza as propriedades de um objeto windows10NetworkBoundaryConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48d9a5e8c5cd8e0d4566f99897e059710f58669c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145252"
---
# <a name="update-windows10networkboundaryconfiguration"></a><span data-ttu-id="6b960-103">Atualizar windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="6b960-103">Update windows10NetworkBoundaryConfiguration</span></span>

> <span data-ttu-id="6b960-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6b960-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b960-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b960-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b960-106">Atualiza as propriedades de um objeto [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6b960-106">Update the properties of a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b960-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6b960-107">Prerequisites</span></span>
<span data-ttu-id="6b960-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6b960-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6b960-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b960-110">Permission type</span></span>|<span data-ttu-id="6b960-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6b960-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b960-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b960-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b960-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b960-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b960-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b960-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b960-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b960-115">Not supported.</span></span>|
|<span data-ttu-id="6b960-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b960-116">Application</span></span>|<span data-ttu-id="6b960-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b960-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b960-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b960-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6b960-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b960-119">Request headers</span></span>
|<span data-ttu-id="6b960-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6b960-120">Header</span></span>|<span data-ttu-id="6b960-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6b960-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b960-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b960-122">Authorization</span></span>|<span data-ttu-id="6b960-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b960-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b960-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6b960-124">Accept</span></span>|<span data-ttu-id="6b960-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6b960-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b960-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b960-126">Request body</span></span>
<span data-ttu-id="6b960-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6b960-127">In the request body, supply a JSON representation for the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

<span data-ttu-id="6b960-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b960-128">The following table shows the properties that are required when you create the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md).</span></span>

|<span data-ttu-id="6b960-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b960-129">Property</span></span>|<span data-ttu-id="6b960-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b960-130">Type</span></span>|<span data-ttu-id="6b960-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b960-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b960-132">id</span><span class="sxs-lookup"><span data-stu-id="6b960-132">id</span></span>|<span data-ttu-id="6b960-133">String</span><span class="sxs-lookup"><span data-stu-id="6b960-133">String</span></span>|<span data-ttu-id="6b960-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6b960-134">Key of the entity.</span></span> <span data-ttu-id="6b960-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b960-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b960-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b960-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6b960-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b960-137">DateTimeOffset</span></span>|<span data-ttu-id="6b960-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6b960-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6b960-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b960-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b960-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6b960-140">roleScopeTagIds</span></span>|<span data-ttu-id="6b960-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b960-141">String collection</span></span>|<span data-ttu-id="6b960-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6b960-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6b960-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b960-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b960-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6b960-144">supportsScopeTags</span></span>|<span data-ttu-id="6b960-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b960-145">Boolean</span></span>|<span data-ttu-id="6b960-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6b960-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6b960-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6b960-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6b960-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6b960-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6b960-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6b960-149">This property is read-only.</span></span> <span data-ttu-id="6b960-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b960-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b960-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b960-151">createdDateTime</span></span>|<span data-ttu-id="6b960-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b960-152">DateTimeOffset</span></span>|<span data-ttu-id="6b960-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6b960-153">DateTime the object was created.</span></span> <span data-ttu-id="6b960-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b960-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b960-155">description</span><span class="sxs-lookup"><span data-stu-id="6b960-155">description</span></span>|<span data-ttu-id="6b960-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b960-156">String</span></span>|<span data-ttu-id="6b960-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6b960-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6b960-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b960-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b960-159">displayName</span><span class="sxs-lookup"><span data-stu-id="6b960-159">displayName</span></span>|<span data-ttu-id="6b960-160">String</span><span class="sxs-lookup"><span data-stu-id="6b960-160">String</span></span>|<span data-ttu-id="6b960-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6b960-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6b960-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b960-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b960-163">version</span><span class="sxs-lookup"><span data-stu-id="6b960-163">version</span></span>|<span data-ttu-id="6b960-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6b960-164">Int32</span></span>|<span data-ttu-id="6b960-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6b960-165">Version of the device configuration.</span></span> <span data-ttu-id="6b960-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b960-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b960-167">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="6b960-167">windowsNetworkIsolationPolicy</span></span>|[<span data-ttu-id="6b960-168">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="6b960-168">windowsNetworkIsolationPolicy</span></span>](../resources/intune-deviceconfig-windowsnetworkisolationpolicy.md)|<span data-ttu-id="6b960-169">Política de isolamento de rede do Windows</span><span class="sxs-lookup"><span data-stu-id="6b960-169">Windows Network Isolation Policy</span></span>|



## <a name="response"></a><span data-ttu-id="6b960-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b960-170">Response</span></span>
<span data-ttu-id="6b960-171">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b960-171">If successful, this method returns a `200 OK` response code and an updated [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b960-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b960-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b960-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b960-173">Request</span></span>
<span data-ttu-id="6b960-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b960-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1244

{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="6b960-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b960-175">Response</span></span>
<span data-ttu-id="6b960-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b960-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1416

{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
  "id": "afbc9e01-9e01-afbc-019e-bcaf019ebcaf",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




