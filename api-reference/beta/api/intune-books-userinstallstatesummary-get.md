---
title: Get userInstallStateSummary
description: Ler propriedades e relações do objeto userInstallStateSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 76b2cff4e5ae21a055159e829fb38690bbbcd176
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760330"
---
# <a name="get-userinstallstatesummary"></a><span data-ttu-id="d1210-103">Get userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="d1210-103">Get userInstallStateSummary</span></span>

> <span data-ttu-id="d1210-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d1210-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1210-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d1210-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1210-106">Ler propriedades e relações do objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d1210-106">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1210-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d1210-107">Prerequisites</span></span>
<span data-ttu-id="d1210-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1210-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1210-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1210-110">Permission type</span></span>|<span data-ttu-id="d1210-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d1210-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1210-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1210-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d1210-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1210-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d1210-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1210-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1210-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1210-115">Not supported.</span></span>|
|<span data-ttu-id="d1210-116">Application</span><span class="sxs-lookup"><span data-stu-id="d1210-116">Application</span></span>|<span data-ttu-id="d1210-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1210-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1210-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1210-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1210-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d1210-119">Optional query parameters</span></span>
<span data-ttu-id="d1210-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d1210-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1210-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1210-121">Request headers</span></span>
|<span data-ttu-id="d1210-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d1210-122">Header</span></span>|<span data-ttu-id="d1210-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d1210-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1210-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1210-124">Authorization</span></span>|<span data-ttu-id="d1210-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1210-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1210-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d1210-126">Accept</span></span>|<span data-ttu-id="d1210-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d1210-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1210-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1210-128">Request body</span></span>
<span data-ttu-id="d1210-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1210-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1210-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1210-130">Response</span></span>
<span data-ttu-id="d1210-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1210-131">If successful, this method returns a `200 OK` response code and [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1210-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1210-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1210-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1210-133">Request</span></span>
<span data-ttu-id="d1210-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1210-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="d1210-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1210-135">Response</span></span>
<span data-ttu-id="d1210-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1210-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




