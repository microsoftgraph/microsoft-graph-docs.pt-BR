---
title: Listar userInstallStateSummaries
description: Listar propriedades e relações dos objetos userInstallStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5c0259bc827d3b8afa8d104353d511a837e8609b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971616"
---
# <a name="list-userinstallstatesummaries"></a><span data-ttu-id="f1848-103">Listar userInstallStateSummaries</span><span class="sxs-lookup"><span data-stu-id="f1848-103">List userInstallStateSummaries</span></span>

> <span data-ttu-id="f1848-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f1848-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1848-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1848-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1848-106">Listar propriedades e relações dos objetos [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f1848-106">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1848-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1848-107">Prerequisites</span></span>
<span data-ttu-id="f1848-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1848-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1848-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1848-110">Permission type</span></span>|<span data-ttu-id="f1848-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1848-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1848-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1848-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1848-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1848-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f1848-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1848-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1848-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1848-115">Not supported.</span></span>|
|<span data-ttu-id="f1848-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1848-116">Application</span></span>|<span data-ttu-id="f1848-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1848-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1848-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1848-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="f1848-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1848-119">Request headers</span></span>
|<span data-ttu-id="f1848-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1848-120">Header</span></span>|<span data-ttu-id="f1848-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f1848-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1848-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1848-122">Authorization</span></span>|<span data-ttu-id="f1848-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1848-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1848-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f1848-124">Accept</span></span>|<span data-ttu-id="f1848-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1848-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1848-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1848-126">Request body</span></span>
<span data-ttu-id="f1848-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1848-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1848-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1848-128">Response</span></span>
<span data-ttu-id="f1848-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1848-129">If successful, this method returns a `200 OK` response code and a collection of [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1848-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1848-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1848-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1848-131">Request</span></span>
<span data-ttu-id="f1848-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1848-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="f1848-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1848-133">Response</span></span>
<span data-ttu-id="f1848-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1848-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




