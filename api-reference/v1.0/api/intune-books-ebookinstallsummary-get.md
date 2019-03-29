---
title: Get eBookInstallSummary
description: Ler propriedades e relações do objeto eBookInstallSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b62a12a1b8a616bfd9ef9d8188d4ebe53cf23092
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974605"
---
# <a name="get-ebookinstallsummary"></a><span data-ttu-id="363e7-103">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="363e7-103">Get eBookInstallSummary</span></span>

> <span data-ttu-id="363e7-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="363e7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="363e7-105">Ler propriedades e relações do objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="363e7-105">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="363e7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="363e7-106">Prerequisites</span></span>
<span data-ttu-id="363e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="363e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="363e7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="363e7-109">Permission type</span></span>|<span data-ttu-id="363e7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="363e7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="363e7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="363e7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="363e7-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="363e7-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="363e7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="363e7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="363e7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="363e7-114">Not supported.</span></span>|
|<span data-ttu-id="363e7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="363e7-115">Application</span></span>|<span data-ttu-id="363e7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="363e7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="363e7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="363e7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="363e7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="363e7-118">Optional query parameters</span></span>
<span data-ttu-id="363e7-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="363e7-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="363e7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="363e7-120">Request headers</span></span>
|<span data-ttu-id="363e7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="363e7-121">Header</span></span>|<span data-ttu-id="363e7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="363e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="363e7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="363e7-123">Authorization</span></span>|<span data-ttu-id="363e7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="363e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="363e7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="363e7-125">Accept</span></span>|<span data-ttu-id="363e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="363e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="363e7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="363e7-127">Request body</span></span>
<span data-ttu-id="363e7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="363e7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="363e7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="363e7-129">Response</span></span>
<span data-ttu-id="363e7-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="363e7-130">If successful, this method returns a `200 OK` response code and [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="363e7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="363e7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="363e7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="363e7-132">Request</span></span>
<span data-ttu-id="363e7-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="363e7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

### <a name="response"></a><span data-ttu-id="363e7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="363e7-134">Response</span></span>
<span data-ttu-id="363e7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="363e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



