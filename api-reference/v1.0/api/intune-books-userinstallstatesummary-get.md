---
title: Get userInstallStateSummary
description: Ler propriedades e relações do objeto userInstallStateSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c5c64f92f18d1993eb8b6f542a515b60501a3279
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515522"
---
# <a name="get-userinstallstatesummary"></a><span data-ttu-id="6aab6-103">Get userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="6aab6-103">Get userInstallStateSummary</span></span>

<span data-ttu-id="6aab6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6aab6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6aab6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6aab6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6aab6-106">Ler propriedades e relações do objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6aab6-106">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6aab6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6aab6-107">Prerequisites</span></span>
<span data-ttu-id="6aab6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6aab6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6aab6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6aab6-110">Permission type</span></span>|<span data-ttu-id="6aab6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6aab6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6aab6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6aab6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6aab6-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6aab6-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6aab6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6aab6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6aab6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6aab6-115">Not supported.</span></span>|
|<span data-ttu-id="6aab6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6aab6-116">Application</span></span>|<span data-ttu-id="6aab6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6aab6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6aab6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6aab6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6aab6-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6aab6-119">Optional query parameters</span></span>
<span data-ttu-id="6aab6-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6aab6-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6aab6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6aab6-121">Request headers</span></span>
|<span data-ttu-id="6aab6-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6aab6-122">Header</span></span>|<span data-ttu-id="6aab6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="6aab6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6aab6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6aab6-124">Authorization</span></span>|<span data-ttu-id="6aab6-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6aab6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6aab6-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6aab6-126">Accept</span></span>|<span data-ttu-id="6aab6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6aab6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6aab6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6aab6-128">Request body</span></span>
<span data-ttu-id="6aab6-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6aab6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6aab6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6aab6-130">Response</span></span>
<span data-ttu-id="6aab6-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6aab6-131">If successful, this method returns a `200 OK` response code and [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aab6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6aab6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6aab6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6aab6-133">Request</span></span>
<span data-ttu-id="6aab6-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6aab6-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="6aab6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6aab6-135">Response</span></span>
<span data-ttu-id="6aab6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6aab6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "value": {
    "@odata.type": "#microsoft.graph.userInstallStateSummary",
    "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
    "userName": "User Name value",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notInstalledDeviceCount": 7
  }
}
```




