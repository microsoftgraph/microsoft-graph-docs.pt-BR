---
title: Obter microsoftTunnelSite
description: Leia propriedades e relações do objeto microsoftTunnelSite.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e08070720f567bcb96587e65825856be1401d21c
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863868"
---
# <a name="get-microsofttunnelsite"></a><span data-ttu-id="7f960-103">Obter microsoftTunnelSite</span><span class="sxs-lookup"><span data-stu-id="7f960-103">Get microsoftTunnelSite</span></span>

<span data-ttu-id="7f960-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f960-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f960-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7f960-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f960-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f960-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f960-107">Leia propriedades e relações do [objeto microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)</span><span class="sxs-lookup"><span data-stu-id="7f960-107">Read properties and relationships of the [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f960-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7f960-108">Prerequisites</span></span>
<span data-ttu-id="7f960-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f960-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f960-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f960-111">Permission type</span></span>|<span data-ttu-id="7f960-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f960-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f960-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f960-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f960-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f960-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|
|<span data-ttu-id="7f960-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f960-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f960-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f960-116">Not supported.</span></span>|
|<span data-ttu-id="7f960-117">Application</span><span class="sxs-lookup"><span data-stu-id="7f960-117">Application</span></span>|<span data-ttu-id="7f960-118">MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f960-118">MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f960-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f960-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f960-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7f960-120">Optional query parameters</span></span>
<span data-ttu-id="7f960-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7f960-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f960-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f960-122">Request headers</span></span>
|<span data-ttu-id="7f960-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7f960-123">Header</span></span>|<span data-ttu-id="7f960-124">Valor</span><span class="sxs-lookup"><span data-stu-id="7f960-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f960-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f960-125">Authorization</span></span>|<span data-ttu-id="7f960-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f960-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f960-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7f960-127">Accept</span></span>|<span data-ttu-id="7f960-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7f960-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f960-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f960-129">Request body</span></span>
<span data-ttu-id="7f960-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7f960-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f960-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f960-131">Response</span></span>
<span data-ttu-id="7f960-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f960-132">If successful, this method returns a `200 OK` response code and [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f960-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f960-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f960-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f960-134">Request</span></span>
<span data-ttu-id="7f960-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f960-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}
```

### <a name="response"></a><span data-ttu-id="7f960-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f960-136">Response</span></span>
<span data-ttu-id="7f960-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f960-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftTunnelSite",
    "id": "b2f7dc3e-dc3e-b2f7-3edc-f7b23edcf7b2",
    "displayName": "Display Name value",
    "description": "Description value",
    "publicAddress": "Public Address value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




