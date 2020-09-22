---
title: Listar iosVppAppAssignedUserLicenses
description: Listar Propriedades e relações dos objetos iosVppAppAssignedUserLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e2eaa501439282e55d60a6fba1ccfab99ee2e30a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006010"
---
# <a name="list-iosvppappassigneduserlicenses"></a><span data-ttu-id="bbf26-103">Listar iosVppAppAssignedUserLicenses</span><span class="sxs-lookup"><span data-stu-id="bbf26-103">List iosVppAppAssignedUserLicenses</span></span>

<span data-ttu-id="bbf26-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbf26-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbf26-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bbf26-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbf26-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bbf26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbf26-107">Listar Propriedades e relações dos objetos [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="bbf26-107">List properties and relationships of the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bbf26-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bbf26-108">Prerequisites</span></span>
<span data-ttu-id="bbf26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbf26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbf26-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbf26-111">Permission type</span></span>|<span data-ttu-id="bbf26-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bbf26-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbf26-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbf26-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bbf26-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbf26-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bbf26-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbf26-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbf26-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbf26-116">Not supported.</span></span>|
|<span data-ttu-id="bbf26-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbf26-117">Application</span></span>|<span data-ttu-id="bbf26-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbf26-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbf26-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbf26-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="bbf26-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf26-120">Request headers</span></span>
|<span data-ttu-id="bbf26-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bbf26-121">Header</span></span>|<span data-ttu-id="bbf26-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bbf26-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbf26-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbf26-123">Authorization</span></span>|<span data-ttu-id="bbf26-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbf26-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbf26-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bbf26-125">Accept</span></span>|<span data-ttu-id="bbf26-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bbf26-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbf26-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf26-127">Request body</span></span>
<span data-ttu-id="bbf26-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bbf26-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbf26-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbf26-129">Response</span></span>
<span data-ttu-id="bbf26-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbf26-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbf26-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbf26-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bbf26-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf26-132">Request</span></span>
<span data-ttu-id="bbf26-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbf26-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="bbf26-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbf26-134">Response</span></span>
<span data-ttu-id="bbf26-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bbf26-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






