---
title: Criar windows10NetworkBoundaryConfiguration
description: Crie um novo objeto de windows10NetworkBoundaryConfiguration.
author: tfitzmac
ms.openlocfilehash: f7bfc2bc8acb726a7a6bbf2c6740e6a106052665
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338028"
---
# <a name="create-windows10networkboundaryconfiguration"></a><span data-ttu-id="97e69-103">Criar windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="97e69-103">Create windows10NetworkBoundaryConfiguration</span></span>

> <span data-ttu-id="97e69-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="97e69-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97e69-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="97e69-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97e69-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="97e69-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97e69-107">Crie um novo objeto de [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="97e69-107">Create a new [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="97e69-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97e69-108">Prerequisites</span></span>
<span data-ttu-id="97e69-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97e69-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97e69-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97e69-111">Permission type</span></span>|<span data-ttu-id="97e69-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97e69-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97e69-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97e69-113">Delegated (work or school account)</span></span>|<span data-ttu-id="97e69-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97e69-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="97e69-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97e69-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97e69-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97e69-116">Not supported.</span></span>|
|<span data-ttu-id="97e69-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97e69-117">Application</span></span>|<span data-ttu-id="97e69-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97e69-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97e69-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97e69-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="97e69-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97e69-120">Request headers</span></span>
|<span data-ttu-id="97e69-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97e69-121">Header</span></span>|<span data-ttu-id="97e69-122">Valor</span><span class="sxs-lookup"><span data-stu-id="97e69-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97e69-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="97e69-123">Authorization</span></span>|<span data-ttu-id="97e69-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97e69-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97e69-125">Accept</span><span class="sxs-lookup"><span data-stu-id="97e69-125">Accept</span></span>|<span data-ttu-id="97e69-126">application/json</span><span class="sxs-lookup"><span data-stu-id="97e69-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97e69-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97e69-127">Request body</span></span>
<span data-ttu-id="97e69-128">No corpo da solicitação, fornece uma representação JSON para o objeto windows10NetworkBoundaryConfiguration.</span><span class="sxs-lookup"><span data-stu-id="97e69-128">In the request body, supply a JSON representation for the windows10NetworkBoundaryConfiguration object.</span></span>

<span data-ttu-id="97e69-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windows10NetworkBoundaryConfiguration.</span><span class="sxs-lookup"><span data-stu-id="97e69-129">The following table shows the properties that are required when you create the windows10NetworkBoundaryConfiguration.</span></span>

|<span data-ttu-id="97e69-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97e69-130">Property</span></span>|<span data-ttu-id="97e69-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="97e69-131">Type</span></span>|<span data-ttu-id="97e69-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="97e69-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97e69-133">id</span><span class="sxs-lookup"><span data-stu-id="97e69-133">id</span></span>|<span data-ttu-id="97e69-134">String</span><span class="sxs-lookup"><span data-stu-id="97e69-134">String</span></span>|<span data-ttu-id="97e69-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="97e69-135">Key of the entity.</span></span> <span data-ttu-id="97e69-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97e69-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97e69-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97e69-137">lastModifiedDateTime</span></span>|<span data-ttu-id="97e69-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97e69-138">DateTimeOffset</span></span>|<span data-ttu-id="97e69-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="97e69-139">DateTime the object was last modified.</span></span> <span data-ttu-id="97e69-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97e69-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97e69-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="97e69-141">roleScopeTagIds</span></span>|<span data-ttu-id="97e69-142">String collection</span><span class="sxs-lookup"><span data-stu-id="97e69-142">String collection</span></span>|<span data-ttu-id="97e69-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="97e69-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="97e69-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97e69-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97e69-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="97e69-145">supportsScopeTags</span></span>|<span data-ttu-id="97e69-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="97e69-146">Boolean</span></span>|<span data-ttu-id="97e69-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="97e69-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="97e69-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="97e69-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="97e69-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="97e69-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="97e69-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="97e69-150">This property is read-only.</span></span> <span data-ttu-id="97e69-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97e69-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97e69-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97e69-152">createdDateTime</span></span>|<span data-ttu-id="97e69-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97e69-153">DateTimeOffset</span></span>|<span data-ttu-id="97e69-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="97e69-154">DateTime the object was created.</span></span> <span data-ttu-id="97e69-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97e69-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97e69-156">description</span><span class="sxs-lookup"><span data-stu-id="97e69-156">description</span></span>|<span data-ttu-id="97e69-157">String</span><span class="sxs-lookup"><span data-stu-id="97e69-157">String</span></span>|<span data-ttu-id="97e69-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97e69-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="97e69-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97e69-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97e69-160">displayName</span><span class="sxs-lookup"><span data-stu-id="97e69-160">displayName</span></span>|<span data-ttu-id="97e69-161">String</span><span class="sxs-lookup"><span data-stu-id="97e69-161">String</span></span>|<span data-ttu-id="97e69-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97e69-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="97e69-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97e69-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97e69-164">version</span><span class="sxs-lookup"><span data-stu-id="97e69-164">version</span></span>|<span data-ttu-id="97e69-165">Int32</span><span class="sxs-lookup"><span data-stu-id="97e69-165">Int32</span></span>|<span data-ttu-id="97e69-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97e69-166">Version of the device configuration.</span></span> <span data-ttu-id="97e69-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97e69-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97e69-168">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="97e69-168">windowsNetworkIsolationPolicy</span></span>|[<span data-ttu-id="97e69-169">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="97e69-169">windowsNetworkIsolationPolicy</span></span>](../resources/intune-deviceconfig-windowsnetworkisolationpolicy.md)|<span data-ttu-id="97e69-170">Política de isolamento de rede do Windows</span><span class="sxs-lookup"><span data-stu-id="97e69-170">Windows Network Isolation Policy</span></span>|



## <a name="response"></a><span data-ttu-id="97e69-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="97e69-171">Response</span></span>
<span data-ttu-id="97e69-172">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97e69-172">If successful, this method returns a `201 Created` response code and a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97e69-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97e69-173">Example</span></span>
### <a name="request"></a><span data-ttu-id="97e69-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97e69-174">Request</span></span>
<span data-ttu-id="97e69-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97e69-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1308

{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="97e69-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="97e69-176">Response</span></span>
<span data-ttu-id="97e69-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97e69-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





