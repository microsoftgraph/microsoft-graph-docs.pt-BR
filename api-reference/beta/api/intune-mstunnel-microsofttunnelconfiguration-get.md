---
title: Obter microsoftTunnelConfiguration
description: Leia propriedades e relações do objeto microsoftTunnelConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b9df82d2db35a54842a76ccc3478e3fe6e1ddb96
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867550"
---
# <a name="get-microsofttunnelconfiguration"></a><span data-ttu-id="6c4e7-103">Obter microsoftTunnelConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c4e7-103">Get microsoftTunnelConfiguration</span></span>

<span data-ttu-id="6c4e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c4e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c4e7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c4e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c4e7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c4e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c4e7-107">Leia propriedades e relações do [objeto microsoftTunnelConfiguration.](../resources/intune-mstunnel-microsofttunnelconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c4e7-107">Read properties and relationships of the [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c4e7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c4e7-108">Prerequisites</span></span>
<span data-ttu-id="6c4e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c4e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c4e7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c4e7-111">Permission type</span></span>|<span data-ttu-id="6c4e7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c4e7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c4e7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c4e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c4e7-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c4e7-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|
|<span data-ttu-id="6c4e7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c4e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c4e7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c4e7-116">Not supported.</span></span>|
|<span data-ttu-id="6c4e7-117">Application</span><span class="sxs-lookup"><span data-stu-id="6c4e7-117">Application</span></span>|<span data-ttu-id="6c4e7-118">MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c4e7-118">MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c4e7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c4e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
GET /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c4e7-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6c4e7-120">Optional query parameters</span></span>
<span data-ttu-id="6c4e7-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6c4e7-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c4e7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c4e7-122">Request headers</span></span>
|<span data-ttu-id="6c4e7-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c4e7-123">Header</span></span>|<span data-ttu-id="6c4e7-124">Valor</span><span class="sxs-lookup"><span data-stu-id="6c4e7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c4e7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c4e7-125">Authorization</span></span>|<span data-ttu-id="6c4e7-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c4e7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c4e7-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c4e7-127">Accept</span></span>|<span data-ttu-id="6c4e7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6c4e7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c4e7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c4e7-129">Request body</span></span>
<span data-ttu-id="6c4e7-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6c4e7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c4e7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c4e7-131">Response</span></span>
<span data-ttu-id="6c4e7-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c4e7-132">If successful, this method returns a `200 OK` response code and [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c4e7-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c4e7-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c4e7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c4e7-134">Request</span></span>
<span data-ttu-id="6c4e7-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c4e7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6c4e7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c4e7-136">Response</span></span>
<span data-ttu-id="6c4e7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c4e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 876

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
    "id": "b8bdb469-b469-b8bd-69b4-bdb869b4bdb8",
    "displayName": "Display Name value",
    "description": "Description value",
    "network": "Network value",
    "dnsServers": [
      "Dns Servers value"
    ],
    "defaultDomainSuffix": "Default Domain Suffix value",
    "routesInclude": [
      "Routes Include value"
    ],
    "routesExclude": [
      "Routes Exclude value"
    ],
    "splitDNS": [
      "Split DNS value"
    ],
    "listenPort": 10,
    "advancedSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




