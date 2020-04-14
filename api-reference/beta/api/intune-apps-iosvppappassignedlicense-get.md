---
title: Obter iosVppAppAssignedLicense
description: Leia as propriedades e as relações do objeto iosVppAppAssignedLicense.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d494f9d80508416744ddfd3b6aeb3f20378cfb35
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43416660"
---
# <a name="get-iosvppappassignedlicense"></a><span data-ttu-id="72482-103">Obter iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="72482-103">Get iosVppAppAssignedLicense</span></span>

<span data-ttu-id="72482-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72482-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72482-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="72482-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72482-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="72482-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72482-107">Leia as propriedades e as relações do objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="72482-107">Read properties and relationships of the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72482-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="72482-108">Prerequisites</span></span>
<span data-ttu-id="72482-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72482-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72482-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72482-111">Permission type</span></span>|<span data-ttu-id="72482-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="72482-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72482-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72482-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72482-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="72482-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="72482-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72482-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72482-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72482-116">Not supported.</span></span>|
|<span data-ttu-id="72482-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72482-117">Application</span></span>|<span data-ttu-id="72482-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="72482-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72482-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72482-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72482-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="72482-120">Optional query parameters</span></span>
<span data-ttu-id="72482-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="72482-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72482-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72482-122">Request headers</span></span>
|<span data-ttu-id="72482-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72482-123">Header</span></span>|<span data-ttu-id="72482-124">Valor</span><span class="sxs-lookup"><span data-stu-id="72482-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72482-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="72482-125">Authorization</span></span>|<span data-ttu-id="72482-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72482-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72482-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="72482-127">Accept</span></span>|<span data-ttu-id="72482-128">application/json</span><span class="sxs-lookup"><span data-stu-id="72482-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72482-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72482-129">Request body</span></span>
<span data-ttu-id="72482-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72482-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72482-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="72482-131">Response</span></span>
<span data-ttu-id="72482-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72482-132">If successful, this method returns a `200 OK` response code and [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72482-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72482-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="72482-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72482-134">Request</span></span>
<span data-ttu-id="72482-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72482-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

### <a name="response"></a><span data-ttu-id="72482-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="72482-136">Response</span></span>
<span data-ttu-id="72482-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72482-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



