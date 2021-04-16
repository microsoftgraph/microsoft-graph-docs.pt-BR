---
title: Listar microsoftTunnelConfigurations
description: Listar propriedades e relações dos objetos microsoftTunnelConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f8306e73e96c555e0f88a134bf854a19be5180c7
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863882"
---
# <a name="list-microsofttunnelconfigurations"></a><span data-ttu-id="a6cdd-103">Listar microsoftTunnelConfigurations</span><span class="sxs-lookup"><span data-stu-id="a6cdd-103">List microsoftTunnelConfigurations</span></span>

<span data-ttu-id="a6cdd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6cdd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6cdd-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a6cdd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6cdd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6cdd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6cdd-107">Listar propriedades e relações dos [objetos microsoftTunnelConfiguration.](../resources/intune-mstunnel-microsofttunnelconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6cdd-107">List properties and relationships of the [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6cdd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6cdd-108">Prerequisites</span></span>
<span data-ttu-id="a6cdd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6cdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6cdd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6cdd-111">Permission type</span></span>|<span data-ttu-id="a6cdd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6cdd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6cdd-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6cdd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6cdd-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6cdd-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|
|<span data-ttu-id="a6cdd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6cdd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6cdd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6cdd-116">Not supported.</span></span>|
|<span data-ttu-id="a6cdd-117">Application</span><span class="sxs-lookup"><span data-stu-id="a6cdd-117">Application</span></span>|<span data-ttu-id="a6cdd-118">MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6cdd-118">MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6cdd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6cdd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a6cdd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6cdd-120">Request headers</span></span>
|<span data-ttu-id="a6cdd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6cdd-121">Header</span></span>|<span data-ttu-id="a6cdd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a6cdd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6cdd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6cdd-123">Authorization</span></span>|<span data-ttu-id="a6cdd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6cdd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6cdd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6cdd-125">Accept</span></span>|<span data-ttu-id="a6cdd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6cdd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6cdd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6cdd-127">Request body</span></span>
<span data-ttu-id="a6cdd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6cdd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6cdd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6cdd-129">Response</span></span>
<span data-ttu-id="a6cdd-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6cdd-130">If successful, this method returns a `200 OK` response code and a collection of [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6cdd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6cdd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6cdd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6cdd-132">Request</span></span>
<span data-ttu-id="a6cdd-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6cdd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelConfigurations
```

### <a name="response"></a><span data-ttu-id="a6cdd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6cdd-134">Response</span></span>
<span data-ttu-id="a6cdd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6cdd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 950

{
  "value": [
    {
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
  ]
}
```




