---
title: Listar userInstallStateSummaries
description: Listar propriedades e relações dos objetos userInstallStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3cf891b84eb1adf46d955c6b68e8b61d4679e224
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322272"
---
# <a name="list-userinstallstatesummaries"></a><span data-ttu-id="2ca33-103">Listar userInstallStateSummaries</span><span class="sxs-lookup"><span data-stu-id="2ca33-103">List userInstallStateSummaries</span></span>

> <span data-ttu-id="2ca33-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2ca33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ca33-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ca33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ca33-106">Listar propriedades e relações dos objetos [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="2ca33-106">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ca33-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2ca33-107">Prerequisites</span></span>
<span data-ttu-id="2ca33-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ca33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ca33-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ca33-110">Permission type</span></span>|<span data-ttu-id="2ca33-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2ca33-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ca33-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ca33-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ca33-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ca33-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2ca33-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ca33-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ca33-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ca33-115">Not supported.</span></span>|
|<span data-ttu-id="2ca33-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ca33-116">Application</span></span>|<span data-ttu-id="2ca33-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ca33-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ca33-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ca33-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="2ca33-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ca33-119">Request headers</span></span>
|<span data-ttu-id="2ca33-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ca33-120">Header</span></span>|<span data-ttu-id="2ca33-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2ca33-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ca33-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ca33-122">Authorization</span></span>|<span data-ttu-id="2ca33-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ca33-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ca33-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ca33-124">Accept</span></span>|<span data-ttu-id="2ca33-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ca33-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ca33-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ca33-126">Request body</span></span>
<span data-ttu-id="2ca33-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ca33-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ca33-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ca33-128">Response</span></span>
<span data-ttu-id="2ca33-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ca33-129">If successful, this method returns a `200 OK` response code and a collection of [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ca33-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ca33-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ca33-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ca33-131">Request</span></span>
<span data-ttu-id="2ca33-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ca33-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="2ca33-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ca33-133">Response</span></span>
<span data-ttu-id="2ca33-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ca33-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userInstallStateSummary",
      "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
      "userName": "User Name value",
      "installedDeviceCount": 4,
      "failedDeviceCount": 1,
      "notInstalledDeviceCount": 7
    }
  ]
}
```






