---
title: Listar mobileAppContents
description: Listar propriedades e relações dos objetos mobileAppContent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cbaf9b6e6ed656079019904e7037d3e9ca8ea701
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754074"
---
# <a name="list-mobileappcontents"></a><span data-ttu-id="32ab3-103">Listar mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="32ab3-103">List mobileAppContents</span></span>

<span data-ttu-id="32ab3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32ab3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32ab3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="32ab3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32ab3-106">Listar propriedades e relações dos objetos [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="32ab3-106">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32ab3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="32ab3-107">Prerequisites</span></span>
<span data-ttu-id="32ab3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32ab3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32ab3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32ab3-110">Permission type</span></span>|<span data-ttu-id="32ab3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32ab3-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32ab3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32ab3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32ab3-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32ab3-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="32ab3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32ab3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32ab3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32ab3-115">Not supported.</span></span>|
|<span data-ttu-id="32ab3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32ab3-116">Application</span></span>|<span data-ttu-id="32ab3-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32ab3-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32ab3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32ab3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="32ab3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32ab3-119">Request headers</span></span>
|<span data-ttu-id="32ab3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32ab3-120">Header</span></span>|<span data-ttu-id="32ab3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="32ab3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32ab3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="32ab3-122">Authorization</span></span>|<span data-ttu-id="32ab3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32ab3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32ab3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="32ab3-124">Accept</span></span>|<span data-ttu-id="32ab3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="32ab3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32ab3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32ab3-126">Request body</span></span>
<span data-ttu-id="32ab3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="32ab3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32ab3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="32ab3-128">Response</span></span>
<span data-ttu-id="32ab3-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileAppContent](../resources/intune-apps-mobileappcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32ab3-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32ab3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32ab3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="32ab3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32ab3-131">Request</span></span>
<span data-ttu-id="32ab3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32ab3-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
```

### <a name="response"></a><span data-ttu-id="32ab3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="32ab3-133">Response</span></span>
<span data-ttu-id="32ab3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32ab3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




