---
title: Obter iosVppAppAssignedLicense
description: Leia as propriedades e as relações do objeto iosVppAppAssignedLicense.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: be067377be8c8665bdc778f8f6e2aa07b74ac908
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36330395"
---
# <a name="get-iosvppappassignedlicense"></a><span data-ttu-id="fee94-103">Obter iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="fee94-103">Get iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="fee94-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fee94-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fee94-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fee94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fee94-106">Leia as propriedades e as relações do objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="fee94-106">Read properties and relationships of the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fee94-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fee94-107">Prerequisites</span></span>
<span data-ttu-id="fee94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fee94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fee94-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fee94-110">Permission type</span></span>|<span data-ttu-id="fee94-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fee94-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fee94-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fee94-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fee94-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fee94-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fee94-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fee94-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fee94-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fee94-115">Not supported.</span></span>|
|<span data-ttu-id="fee94-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fee94-116">Application</span></span>|<span data-ttu-id="fee94-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fee94-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fee94-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fee94-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fee94-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fee94-119">Optional query parameters</span></span>
<span data-ttu-id="fee94-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fee94-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fee94-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fee94-121">Request headers</span></span>
|<span data-ttu-id="fee94-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fee94-122">Header</span></span>|<span data-ttu-id="fee94-123">Valor</span><span class="sxs-lookup"><span data-stu-id="fee94-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fee94-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fee94-124">Authorization</span></span>|<span data-ttu-id="fee94-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fee94-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fee94-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fee94-126">Accept</span></span>|<span data-ttu-id="fee94-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fee94-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fee94-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fee94-128">Request body</span></span>
<span data-ttu-id="fee94-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fee94-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fee94-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fee94-130">Response</span></span>
<span data-ttu-id="fee94-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fee94-131">If successful, this method returns a `200 OK` response code and [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fee94-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fee94-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fee94-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fee94-133">Request</span></span>
<span data-ttu-id="fee94-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fee94-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

### <a name="response"></a><span data-ttu-id="fee94-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fee94-135">Response</span></span>
<span data-ttu-id="fee94-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fee94-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 314

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
    "id": "090a8d2e-8d2e-090a-2e8d-0a092e8d0a09",
    "userEmailAddress": "User Email Address value",
    "userId": "User Id value",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value"
  }
}
```






