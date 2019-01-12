---
title: Get eBookInstallSummary
description: Ler propriedades e relações do objeto eBookInstallSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d60ea9c491d931f022ae83dda6285d36c6855f89
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933635"
---
# <a name="get-ebookinstallsummary"></a><span data-ttu-id="84119-103">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="84119-103">Get eBookInstallSummary</span></span>

> <span data-ttu-id="84119-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="84119-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84119-105">Ler propriedades e relações do objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="84119-105">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84119-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="84119-106">Prerequisites</span></span>
<span data-ttu-id="84119-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84119-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84119-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84119-109">Permission type</span></span>|<span data-ttu-id="84119-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="84119-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84119-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84119-111">Delegated (work or school account)</span></span>|<span data-ttu-id="84119-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="84119-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="84119-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84119-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84119-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84119-114">Not supported.</span></span>|
|<span data-ttu-id="84119-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84119-115">Application</span></span>|<span data-ttu-id="84119-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84119-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84119-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84119-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84119-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="84119-118">Optional query parameters</span></span>
<span data-ttu-id="84119-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="84119-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="84119-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84119-120">Request headers</span></span>
|<span data-ttu-id="84119-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84119-121">Header</span></span>|<span data-ttu-id="84119-122">Valor</span><span class="sxs-lookup"><span data-stu-id="84119-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84119-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="84119-123">Authorization</span></span>|<span data-ttu-id="84119-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84119-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84119-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="84119-125">Accept</span></span>|<span data-ttu-id="84119-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84119-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84119-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84119-127">Request body</span></span>
<span data-ttu-id="84119-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="84119-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84119-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="84119-129">Response</span></span>
<span data-ttu-id="84119-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84119-130">If successful, this method returns a `200 OK` response code and [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84119-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84119-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="84119-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84119-132">Request</span></span>
<span data-ttu-id="84119-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84119-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

### <a name="response"></a><span data-ttu-id="84119-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="84119-134">Response</span></span>
<span data-ttu-id="84119-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84119-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



