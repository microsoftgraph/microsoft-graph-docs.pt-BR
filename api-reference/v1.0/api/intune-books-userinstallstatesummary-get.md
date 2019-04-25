---
title: Get userInstallStateSummary
description: Ler propriedades e relações do objeto userInstallStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d8e33f71e5a4b7008e7dc2b46fab5c04023ce579
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524579"
---
# <a name="get-userinstallstatesummary"></a><span data-ttu-id="ecba9-103">Get userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="ecba9-103">Get userInstallStateSummary</span></span>

> <span data-ttu-id="ecba9-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ecba9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecba9-105">Ler propriedades e relações do objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="ecba9-105">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecba9-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ecba9-106">Prerequisites</span></span>
<span data-ttu-id="ecba9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecba9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecba9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ecba9-109">Permission type</span></span>|<span data-ttu-id="ecba9-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ecba9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecba9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ecba9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ecba9-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ecba9-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ecba9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ecba9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecba9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecba9-114">Not supported.</span></span>|
|<span data-ttu-id="ecba9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ecba9-115">Application</span></span>|<span data-ttu-id="ecba9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecba9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecba9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecba9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ecba9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ecba9-118">Optional query parameters</span></span>
<span data-ttu-id="ecba9-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ecba9-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ecba9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ecba9-120">Request headers</span></span>
|<span data-ttu-id="ecba9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ecba9-121">Header</span></span>|<span data-ttu-id="ecba9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ecba9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecba9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ecba9-123">Authorization</span></span>|<span data-ttu-id="ecba9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecba9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecba9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ecba9-125">Accept</span></span>|<span data-ttu-id="ecba9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ecba9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecba9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ecba9-127">Request body</span></span>
<span data-ttu-id="ecba9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ecba9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecba9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecba9-129">Response</span></span>
<span data-ttu-id="ecba9-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ecba9-130">If successful, this method returns a `200 OK` response code and [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecba9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ecba9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecba9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ecba9-132">Request</span></span>
<span data-ttu-id="ecba9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecba9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="ecba9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecba9-134">Response</span></span>
<span data-ttu-id="ecba9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ecba9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



