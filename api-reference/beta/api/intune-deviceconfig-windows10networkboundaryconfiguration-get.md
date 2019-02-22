---
title: Obter windows10NetworkBoundaryConfiguration
description: Leia as propriedades e as relações do objeto windows10NetworkBoundaryConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b8ae5fe2ce9db335b32f273a64afa7e748b286fa
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160148"
---
# <a name="get-windows10networkboundaryconfiguration"></a><span data-ttu-id="0ee3f-103">Obter windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ee3f-103">Get windows10NetworkBoundaryConfiguration</span></span>

> <span data-ttu-id="0ee3f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0ee3f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ee3f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0ee3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ee3f-106">Leia as propriedades e as relações do objeto [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0ee3f-106">Read properties and relationships of the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ee3f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0ee3f-107">Prerequisites</span></span>
<span data-ttu-id="0ee3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0ee3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0ee3f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ee3f-110">Permission type</span></span>|<span data-ttu-id="0ee3f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0ee3f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ee3f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ee3f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ee3f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ee3f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0ee3f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ee3f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ee3f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ee3f-115">Not supported.</span></span>|
|<span data-ttu-id="0ee3f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ee3f-116">Application</span></span>|<span data-ttu-id="0ee3f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ee3f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ee3f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ee3f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ee3f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0ee3f-119">Optional query parameters</span></span>
<span data-ttu-id="0ee3f-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0ee3f-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ee3f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ee3f-121">Request headers</span></span>
|<span data-ttu-id="0ee3f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ee3f-122">Header</span></span>|<span data-ttu-id="0ee3f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="0ee3f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ee3f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ee3f-124">Authorization</span></span>|<span data-ttu-id="0ee3f-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ee3f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ee3f-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0ee3f-126">Accept</span></span>|<span data-ttu-id="0ee3f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0ee3f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ee3f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ee3f-128">Request body</span></span>
<span data-ttu-id="0ee3f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0ee3f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ee3f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ee3f-130">Response</span></span>
<span data-ttu-id="0ee3f-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ee3f-131">If successful, this method returns a `200 OK` response code and [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ee3f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ee3f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ee3f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ee3f-133">Request</span></span>
<span data-ttu-id="0ee3f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ee3f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="0ee3f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ee3f-135">Response</span></span>
<span data-ttu-id="0ee3f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ee3f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1519

{
  "value": {
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
}
```




