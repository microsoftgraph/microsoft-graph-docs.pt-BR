---
title: Listar microsoftTunnelSites
description: Listar Propriedades e relações dos objetos microsoftTunnelSite.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: edefc1f378a3f80eecfd10131712b39fc3a3e186
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301388"
---
# <a name="list-microsofttunnelsites"></a><span data-ttu-id="63a73-103">Listar microsoftTunnelSites</span><span class="sxs-lookup"><span data-stu-id="63a73-103">List microsoftTunnelSites</span></span>

<span data-ttu-id="63a73-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63a73-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63a73-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63a73-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63a73-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63a73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63a73-107">Listar Propriedades e relações dos objetos [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) .</span><span class="sxs-lookup"><span data-stu-id="63a73-107">List properties and relationships of the [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63a73-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63a73-108">Prerequisites</span></span>
<span data-ttu-id="63a73-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63a73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63a73-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63a73-111">Permission type</span></span>|<span data-ttu-id="63a73-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63a73-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63a73-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63a73-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63a73-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="63a73-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="63a73-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63a73-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63a73-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63a73-116">Not supported.</span></span>|
|<span data-ttu-id="63a73-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63a73-117">Application</span></span>|<span data-ttu-id="63a73-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="63a73-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63a73-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63a73-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelSites
```

## <a name="request-headers"></a><span data-ttu-id="63a73-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63a73-120">Request headers</span></span>
|<span data-ttu-id="63a73-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63a73-121">Header</span></span>|<span data-ttu-id="63a73-122">Valor</span><span class="sxs-lookup"><span data-stu-id="63a73-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63a73-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="63a73-123">Authorization</span></span>|<span data-ttu-id="63a73-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63a73-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63a73-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63a73-125">Accept</span></span>|<span data-ttu-id="63a73-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63a73-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63a73-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63a73-127">Request body</span></span>
<span data-ttu-id="63a73-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63a73-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63a73-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="63a73-129">Response</span></span>
<span data-ttu-id="63a73-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63a73-130">If successful, this method returns a `200 OK` response code and a collection of [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63a73-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63a73-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="63a73-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63a73-132">Request</span></span>
<span data-ttu-id="63a73-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63a73-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites
```

### <a name="response"></a><span data-ttu-id="63a73-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="63a73-134">Response</span></span>
<span data-ttu-id="63a73-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63a73-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 360

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftTunnelSite",
      "id": "b2f7dc3e-dc3e-b2f7-3edc-f7b23edcf7b2",
      "displayName": "Display Name value",
      "description": "Description value",
      "publicAddress": "Public Address value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




