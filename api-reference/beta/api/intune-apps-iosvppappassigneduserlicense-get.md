---
title: Obter iosVppAppAssignedUserLicense
description: Leia as propriedades e as relações do objeto iosVppAppAssignedUserLicense.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1235dbb30186ba741506d70dc48cebf83e0b96d3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761815"
---
# <a name="get-iosvppappassigneduserlicense"></a><span data-ttu-id="07451-103">Obter iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="07451-103">Get iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="07451-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="07451-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07451-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07451-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07451-106">Leia as propriedades e as relações do objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="07451-106">Read properties and relationships of the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07451-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07451-107">Prerequisites</span></span>
<span data-ttu-id="07451-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07451-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07451-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07451-110">Permission type</span></span>|<span data-ttu-id="07451-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="07451-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07451-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07451-112">Delegated (work or school account)</span></span>|<span data-ttu-id="07451-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="07451-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="07451-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07451-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07451-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07451-115">Not supported.</span></span>|
|<span data-ttu-id="07451-116">Application</span><span class="sxs-lookup"><span data-stu-id="07451-116">Application</span></span>|<span data-ttu-id="07451-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="07451-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07451-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07451-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="07451-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="07451-119">Optional query parameters</span></span>
<span data-ttu-id="07451-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="07451-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07451-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07451-121">Request headers</span></span>
|<span data-ttu-id="07451-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07451-122">Header</span></span>|<span data-ttu-id="07451-123">Valor</span><span class="sxs-lookup"><span data-stu-id="07451-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07451-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="07451-124">Authorization</span></span>|<span data-ttu-id="07451-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07451-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07451-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07451-126">Accept</span></span>|<span data-ttu-id="07451-127">application/json</span><span class="sxs-lookup"><span data-stu-id="07451-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07451-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07451-128">Request body</span></span>
<span data-ttu-id="07451-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="07451-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07451-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="07451-130">Response</span></span>
<span data-ttu-id="07451-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07451-131">If successful, this method returns a `200 OK` response code and [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07451-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07451-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="07451-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07451-133">Request</span></span>
<span data-ttu-id="07451-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07451-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

### <a name="response"></a><span data-ttu-id="07451-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="07451-135">Response</span></span>
<span data-ttu-id="07451-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07451-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 318

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
    "id": "fedc747d-747d-fedc-7d74-dcfe7d74dcfe",
    "userEmailAddress": "User Email Address value",
    "userId": "User Id value",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value"
  }
}
```




