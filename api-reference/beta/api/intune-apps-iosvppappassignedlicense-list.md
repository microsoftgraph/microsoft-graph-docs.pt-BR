---
title: Listar iosVppAppAssignedLicenses
description: Listar Propriedades e relações dos objetos iosVppAppAssignedLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff3948a8882da0c2b1b6e29a56989169c5a4eb5e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990435"
---
# <a name="list-iosvppappassignedlicenses"></a><span data-ttu-id="be9ea-103">Listar iosVppAppAssignedLicenses</span><span class="sxs-lookup"><span data-stu-id="be9ea-103">List iosVppAppAssignedLicenses</span></span>

<span data-ttu-id="be9ea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be9ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be9ea-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="be9ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be9ea-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="be9ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be9ea-107">Listar Propriedades e relações dos objetos [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="be9ea-107">List properties and relationships of the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be9ea-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="be9ea-108">Prerequisites</span></span>
<span data-ttu-id="be9ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be9ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be9ea-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be9ea-111">Permission type</span></span>|<span data-ttu-id="be9ea-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="be9ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be9ea-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be9ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="be9ea-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="be9ea-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="be9ea-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be9ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be9ea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be9ea-116">Not supported.</span></span>|
|<span data-ttu-id="be9ea-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be9ea-117">Application</span></span>|<span data-ttu-id="be9ea-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="be9ea-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be9ea-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be9ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="be9ea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be9ea-120">Request headers</span></span>
|<span data-ttu-id="be9ea-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="be9ea-121">Header</span></span>|<span data-ttu-id="be9ea-122">Valor</span><span class="sxs-lookup"><span data-stu-id="be9ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be9ea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="be9ea-123">Authorization</span></span>|<span data-ttu-id="be9ea-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be9ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be9ea-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="be9ea-125">Accept</span></span>|<span data-ttu-id="be9ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="be9ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be9ea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be9ea-127">Request body</span></span>
<span data-ttu-id="be9ea-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="be9ea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be9ea-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="be9ea-129">Response</span></span>
<span data-ttu-id="be9ea-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be9ea-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be9ea-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be9ea-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="be9ea-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be9ea-132">Request</span></span>
<span data-ttu-id="be9ea-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be9ea-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="be9ea-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="be9ea-134">Response</span></span>
<span data-ttu-id="be9ea-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be9ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 340

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
      "id": "090a8d2e-8d2e-090a-2e8d-0a092e8d0a09",
      "userEmailAddress": "User Email Address value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```






