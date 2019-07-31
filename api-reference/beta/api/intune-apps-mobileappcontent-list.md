---
title: Listar mobileAppContents
description: Listar propriedades e relações dos objetos mobileAppContent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ed80d89c73683fe9ba1d117d2eafe88dab8ade29
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960822"
---
# <a name="list-mobileappcontents"></a><span data-ttu-id="e672f-103">Listar mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="e672f-103">List mobileAppContents</span></span>

> <span data-ttu-id="e672f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e672f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e672f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e672f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e672f-106">Listar propriedades e relações dos objetos [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="e672f-106">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e672f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e672f-107">Prerequisites</span></span>
<span data-ttu-id="e672f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e672f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e672f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e672f-110">Permission type</span></span>|<span data-ttu-id="e672f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e672f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e672f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e672f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e672f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e672f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e672f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e672f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e672f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e672f-115">Not supported.</span></span>|
|<span data-ttu-id="e672f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e672f-116">Application</span></span>|<span data-ttu-id="e672f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e672f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e672f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e672f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="e672f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e672f-119">Request headers</span></span>
|<span data-ttu-id="e672f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e672f-120">Header</span></span>|<span data-ttu-id="e672f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e672f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e672f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e672f-122">Authorization</span></span>|<span data-ttu-id="e672f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e672f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e672f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e672f-124">Accept</span></span>|<span data-ttu-id="e672f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e672f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e672f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e672f-126">Request body</span></span>
<span data-ttu-id="e672f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e672f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e672f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e672f-128">Response</span></span>
<span data-ttu-id="e672f-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileAppContent](../resources/intune-apps-mobileappcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e672f-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e672f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e672f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e672f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e672f-131">Request</span></span>
<span data-ttu-id="e672f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e672f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
```

### <a name="response"></a><span data-ttu-id="e672f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e672f-133">Response</span></span>
<span data-ttu-id="e672f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e672f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 148

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppContent",
      "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
    }
  ]
}
```





