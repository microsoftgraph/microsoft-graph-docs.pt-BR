---
title: Listar macOsVppAppAssignedLicenses
description: Listar Propriedades e relações dos objetos macOsVppAppAssignedLicense.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 51e8594021587ea53dfd77c407bfaa8997bc1d94
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982872"
---
# <a name="list-macosvppappassignedlicenses"></a><span data-ttu-id="46615-103">Listar macOsVppAppAssignedLicenses</span><span class="sxs-lookup"><span data-stu-id="46615-103">List macOsVppAppAssignedLicenses</span></span>

> <span data-ttu-id="46615-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="46615-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46615-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="46615-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46615-106">Listar Propriedades e relações dos objetos [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="46615-106">List properties and relationships of the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46615-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="46615-107">Prerequisites</span></span>
<span data-ttu-id="46615-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46615-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46615-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46615-110">Permission type</span></span>|<span data-ttu-id="46615-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="46615-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46615-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46615-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46615-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="46615-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="46615-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46615-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46615-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46615-115">Not supported.</span></span>|
|<span data-ttu-id="46615-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46615-116">Application</span></span>|<span data-ttu-id="46615-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46615-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46615-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46615-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="46615-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46615-119">Request headers</span></span>
|<span data-ttu-id="46615-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="46615-120">Header</span></span>|<span data-ttu-id="46615-121">Valor</span><span class="sxs-lookup"><span data-stu-id="46615-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46615-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="46615-122">Authorization</span></span>|<span data-ttu-id="46615-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46615-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46615-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="46615-124">Accept</span></span>|<span data-ttu-id="46615-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46615-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46615-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46615-126">Request body</span></span>
<span data-ttu-id="46615-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46615-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46615-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="46615-128">Response</span></span>
<span data-ttu-id="46615-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46615-129">If successful, this method returns a `200 OK` response code and a collection of [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46615-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46615-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="46615-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46615-131">Request</span></span>
<span data-ttu-id="46615-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46615-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="46615-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="46615-133">Response</span></span>
<span data-ttu-id="46615-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46615-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 342

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
      "id": "a1204d8e-4d8e-a120-8e4d-20a18e4d20a1",
      "userEmailAddress": "User Email Address value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




