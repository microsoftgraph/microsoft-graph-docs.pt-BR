---
title: Listar resourceOperations
description: Listar propriedades e relações dos objetos resourceOperation.
author: tfitzmac
ms.openlocfilehash: af691d9f0563fa3b9805a512f234b35d1bad4d74
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319191"
---
# <a name="list-resourceoperations"></a><span data-ttu-id="a3b07-103">Listar resourceOperations</span><span class="sxs-lookup"><span data-stu-id="a3b07-103">List resourceOperations</span></span>

> <span data-ttu-id="a3b07-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a3b07-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3b07-105">Listar propriedades e relações dos objetos [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="a3b07-105">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a3b07-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a3b07-106">Prerequisites</span></span>
<span data-ttu-id="a3b07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3b07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3b07-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3b07-109">Permission type</span></span>|<span data-ttu-id="a3b07-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a3b07-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3b07-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3b07-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a3b07-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3b07-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="a3b07-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3b07-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3b07-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3b07-114">Not supported.</span></span>|
|<span data-ttu-id="a3b07-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3b07-115">Application</span></span>|<span data-ttu-id="a3b07-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3b07-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3b07-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3b07-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="a3b07-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3b07-118">Request headers</span></span>
|<span data-ttu-id="a3b07-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a3b07-119">Header</span></span>|<span data-ttu-id="a3b07-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a3b07-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3b07-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3b07-121">Authorization</span></span>|<span data-ttu-id="a3b07-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3b07-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3b07-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a3b07-123">Accept</span></span>|<span data-ttu-id="a3b07-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a3b07-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3b07-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3b07-125">Request body</span></span>
<span data-ttu-id="a3b07-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a3b07-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3b07-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3b07-127">Response</span></span>
<span data-ttu-id="a3b07-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [resourceOperation](../resources/intune-rbac-resourceoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3b07-128">If successful, this method returns a `200 OK` response code and a collection of [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3b07-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3b07-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="a3b07-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3b07-130">Request</span></span>
<span data-ttu-id="a3b07-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3b07-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations
```

### <a name="response"></a><span data-ttu-id="a3b07-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3b07-132">Response</span></span>
<span data-ttu-id="a3b07-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3b07-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 280

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.resourceOperation",
      "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
      "resourceName": "Resource Name value",
      "actionName": "Action Name value",
      "description": "Description value"
    }
  ]
}
```



