---
title: Get userInstallStateSummary
description: Ler propriedades e relações do objeto userInstallStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 87ac0b8d8e04a17d227adb20cf65f7e91baaabc1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019923"
---
# <a name="get-userinstallstatesummary"></a><span data-ttu-id="de995-103">Get userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="de995-103">Get userInstallStateSummary</span></span>

> <span data-ttu-id="de995-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="de995-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de995-105">Ler propriedades e relações do objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="de995-105">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de995-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="de995-106">Prerequisites</span></span>
<span data-ttu-id="de995-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de995-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de995-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de995-109">Permission type</span></span>|<span data-ttu-id="de995-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="de995-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de995-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de995-111">Delegated (work or school account)</span></span>|<span data-ttu-id="de995-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="de995-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="de995-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de995-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de995-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de995-114">Not supported.</span></span>|
|<span data-ttu-id="de995-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de995-115">Application</span></span>|<span data-ttu-id="de995-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de995-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de995-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de995-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="de995-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="de995-118">Optional query parameters</span></span>
<span data-ttu-id="de995-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="de995-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="de995-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de995-120">Request headers</span></span>
|<span data-ttu-id="de995-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de995-121">Header</span></span>|<span data-ttu-id="de995-122">Valor</span><span class="sxs-lookup"><span data-stu-id="de995-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de995-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="de995-123">Authorization</span></span>|<span data-ttu-id="de995-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de995-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de995-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="de995-125">Accept</span></span>|<span data-ttu-id="de995-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de995-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de995-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de995-127">Request body</span></span>
<span data-ttu-id="de995-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="de995-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de995-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="de995-129">Response</span></span>
<span data-ttu-id="de995-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de995-130">If successful, this method returns a `200 OK` response code and [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de995-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de995-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="de995-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de995-132">Request</span></span>
<span data-ttu-id="de995-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de995-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="de995-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="de995-134">Response</span></span>
<span data-ttu-id="de995-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de995-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



