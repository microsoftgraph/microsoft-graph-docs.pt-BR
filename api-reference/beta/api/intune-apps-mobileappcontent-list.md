---
title: Listar mobileAppContents
description: Listar propriedades e relações dos objetos mobileAppContent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d9bce10c6c418989b28d976cf166ee90fc8d719f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143280"
---
# <a name="list-mobileappcontents"></a><span data-ttu-id="0e0ba-103">Listar mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="0e0ba-103">List mobileAppContents</span></span>

<span data-ttu-id="0e0ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e0ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e0ba-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e0ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e0ba-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e0ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e0ba-107">Listar propriedades e relações dos objetos [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="0e0ba-107">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e0ba-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0e0ba-108">Prerequisites</span></span>
<span data-ttu-id="0e0ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e0ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e0ba-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e0ba-111">Permission type</span></span>|<span data-ttu-id="0e0ba-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e0ba-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e0ba-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e0ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e0ba-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e0ba-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0e0ba-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e0ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e0ba-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e0ba-116">Not supported.</span></span>|
|<span data-ttu-id="0e0ba-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e0ba-117">Application</span></span>|<span data-ttu-id="0e0ba-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e0ba-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e0ba-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e0ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="0e0ba-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e0ba-120">Request headers</span></span>
|<span data-ttu-id="0e0ba-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0e0ba-121">Header</span></span>|<span data-ttu-id="0e0ba-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0e0ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e0ba-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e0ba-123">Authorization</span></span>|<span data-ttu-id="0e0ba-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e0ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e0ba-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0e0ba-125">Accept</span></span>|<span data-ttu-id="0e0ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e0ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e0ba-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e0ba-127">Request body</span></span>
<span data-ttu-id="0e0ba-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0e0ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e0ba-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e0ba-129">Response</span></span>
<span data-ttu-id="0e0ba-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileAppContent](../resources/intune-apps-mobileappcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e0ba-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e0ba-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e0ba-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e0ba-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e0ba-132">Request</span></span>
<span data-ttu-id="0e0ba-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e0ba-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
```

### <a name="response"></a><span data-ttu-id="0e0ba-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e0ba-134">Response</span></span>
<span data-ttu-id="0e0ba-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e0ba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




