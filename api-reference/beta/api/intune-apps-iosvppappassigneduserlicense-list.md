---
title: Listar iosVppAppAssignedUserLicenses
description: Listar Propriedades e relações dos objetos iosVppAppAssignedUserLicense.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 76060286b1c22db9375f44a54c5769003a260f02
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35962187"
---
# <a name="list-iosvppappassigneduserlicenses"></a><span data-ttu-id="9f62d-103">Listar iosVppAppAssignedUserLicenses</span><span class="sxs-lookup"><span data-stu-id="9f62d-103">List iosVppAppAssignedUserLicenses</span></span>

> <span data-ttu-id="9f62d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9f62d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f62d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9f62d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f62d-106">Listar Propriedades e relações dos objetos [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="9f62d-106">List properties and relationships of the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f62d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9f62d-107">Prerequisites</span></span>
<span data-ttu-id="9f62d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f62d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f62d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f62d-110">Permission type</span></span>|<span data-ttu-id="9f62d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9f62d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f62d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f62d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f62d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f62d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9f62d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f62d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f62d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f62d-115">Not supported.</span></span>|
|<span data-ttu-id="9f62d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f62d-116">Application</span></span>|<span data-ttu-id="9f62d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f62d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f62d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f62d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="9f62d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f62d-119">Request headers</span></span>
|<span data-ttu-id="9f62d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9f62d-120">Header</span></span>|<span data-ttu-id="9f62d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9f62d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f62d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f62d-122">Authorization</span></span>|<span data-ttu-id="9f62d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f62d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f62d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9f62d-124">Accept</span></span>|<span data-ttu-id="9f62d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f62d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f62d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f62d-126">Request body</span></span>
<span data-ttu-id="9f62d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9f62d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f62d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f62d-128">Response</span></span>
<span data-ttu-id="9f62d-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f62d-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f62d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f62d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f62d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f62d-131">Request</span></span>
<span data-ttu-id="9f62d-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f62d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="9f62d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f62d-133">Response</span></span>
<span data-ttu-id="9f62d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f62d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
      "id": "fedc747d-747d-fedc-7d74-dcfe7d74dcfe",
      "userEmailAddress": "User Email Address value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





