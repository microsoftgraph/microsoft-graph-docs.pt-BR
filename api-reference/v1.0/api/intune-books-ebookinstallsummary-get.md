---
title: Get eBookInstallSummary
description: Ler propriedades e relações do objeto eBookInstallSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d1d7774c445cb43d2b089f117442c8b0745508b1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515683"
---
# <a name="get-ebookinstallsummary"></a><span data-ttu-id="1b0c3-103">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="1b0c3-103">Get eBookInstallSummary</span></span>

<span data-ttu-id="1b0c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b0c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b0c3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1b0c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b0c3-106">Ler propriedades e relações do objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="1b0c3-106">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b0c3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1b0c3-107">Prerequisites</span></span>
<span data-ttu-id="1b0c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b0c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b0c3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b0c3-110">Permission type</span></span>|<span data-ttu-id="1b0c3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1b0c3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b0c3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b0c3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1b0c3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b0c3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1b0c3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b0c3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b0c3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b0c3-115">Not supported.</span></span>|
|<span data-ttu-id="1b0c3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b0c3-116">Application</span></span>|<span data-ttu-id="1b0c3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b0c3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b0c3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b0c3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1b0c3-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1b0c3-119">Optional query parameters</span></span>
<span data-ttu-id="1b0c3-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1b0c3-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b0c3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b0c3-121">Request headers</span></span>
|<span data-ttu-id="1b0c3-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1b0c3-122">Header</span></span>|<span data-ttu-id="1b0c3-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1b0c3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b0c3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b0c3-124">Authorization</span></span>|<span data-ttu-id="1b0c3-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b0c3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b0c3-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1b0c3-126">Accept</span></span>|<span data-ttu-id="1b0c3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1b0c3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b0c3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b0c3-128">Request body</span></span>
<span data-ttu-id="1b0c3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1b0c3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b0c3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b0c3-130">Response</span></span>
<span data-ttu-id="1b0c3-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b0c3-131">If successful, this method returns a `200 OK` response code and [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b0c3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b0c3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b0c3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b0c3-133">Request</span></span>
<span data-ttu-id="1b0c3-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b0c3-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

### <a name="response"></a><span data-ttu-id="1b0c3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b0c3-135">Response</span></span>
<span data-ttu-id="1b0c3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b0c3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 320

{
  "value": {
    "@odata.type": "#microsoft.graph.eBookInstallSummary",
    "id": "9708ad78-ad78-9708-78ad-089778ad0897",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notInstalledDeviceCount": 7,
    "installedUserCount": 2,
    "failedUserCount": 15,
    "notInstalledUserCount": 5
  }
}
```




