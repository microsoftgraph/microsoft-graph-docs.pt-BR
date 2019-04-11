---
title: Acessar mobileAppContent
description: Leia as propriedades e as relações do objeto mobileAppContent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 58316fa897683ec968a1aa2e9a0112b671c616a8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804232"
---
# <a name="get-mobileappcontent"></a><span data-ttu-id="7dcfa-103">Acessar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="7dcfa-103">Get mobileAppContent</span></span>

> <span data-ttu-id="7dcfa-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7dcfa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7dcfa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7dcfa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dcfa-106">Leia as propriedades e as relações do objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="7dcfa-106">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7dcfa-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7dcfa-107">Prerequisites</span></span>
<span data-ttu-id="7dcfa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dcfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dcfa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7dcfa-110">Permission type</span></span>|<span data-ttu-id="7dcfa-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7dcfa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dcfa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7dcfa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7dcfa-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7dcfa-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7dcfa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7dcfa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dcfa-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7dcfa-115">Not supported.</span></span>|
|<span data-ttu-id="7dcfa-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7dcfa-116">Application</span></span>|<span data-ttu-id="7dcfa-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7dcfa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7dcfa-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7dcfa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7dcfa-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7dcfa-119">Optional query parameters</span></span>
<span data-ttu-id="7dcfa-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7dcfa-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7dcfa-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7dcfa-121">Request headers</span></span>
|<span data-ttu-id="7dcfa-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7dcfa-122">Header</span></span>|<span data-ttu-id="7dcfa-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7dcfa-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7dcfa-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7dcfa-124">Authorization</span></span>|<span data-ttu-id="7dcfa-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7dcfa-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7dcfa-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7dcfa-126">Accept</span></span>|<span data-ttu-id="7dcfa-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7dcfa-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dcfa-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7dcfa-128">Request body</span></span>
<span data-ttu-id="7dcfa-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7dcfa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7dcfa-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dcfa-130">Response</span></span>
<span data-ttu-id="7dcfa-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7dcfa-131">If successful, this method returns a `200 OK` response code and [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dcfa-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7dcfa-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7dcfa-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7dcfa-133">Request</span></span>
<span data-ttu-id="7dcfa-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7dcfa-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
```

### <a name="response"></a><span data-ttu-id="7dcfa-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dcfa-135">Response</span></span>
<span data-ttu-id="7dcfa-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7dcfa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppContent",
    "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
  }
}
```





