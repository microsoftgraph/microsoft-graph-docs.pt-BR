---
title: Listar resourceOperations
description: Listar propriedades e relações dos objetos resourceOperation.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e610121c5639b0bc7ef2bcc982d41b3a8c386111
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512262"
---
# <a name="list-resourceoperations"></a><span data-ttu-id="59de2-103">Listar resourceOperations</span><span class="sxs-lookup"><span data-stu-id="59de2-103">List resourceOperations</span></span>

<span data-ttu-id="59de2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59de2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59de2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59de2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59de2-106">Listar propriedades e relações dos objetos [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="59de2-106">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59de2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59de2-107">Prerequisites</span></span>
<span data-ttu-id="59de2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59de2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59de2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59de2-110">Permission type</span></span>|<span data-ttu-id="59de2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="59de2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59de2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59de2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="59de2-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="59de2-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="59de2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59de2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59de2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59de2-115">Not supported.</span></span>|
|<span data-ttu-id="59de2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59de2-116">Application</span></span>|<span data-ttu-id="59de2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59de2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59de2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59de2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="59de2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59de2-119">Request headers</span></span>
|<span data-ttu-id="59de2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59de2-120">Header</span></span>|<span data-ttu-id="59de2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="59de2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59de2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="59de2-122">Authorization</span></span>|<span data-ttu-id="59de2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59de2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59de2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="59de2-124">Accept</span></span>|<span data-ttu-id="59de2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="59de2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59de2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59de2-126">Request body</span></span>
<span data-ttu-id="59de2-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="59de2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59de2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="59de2-128">Response</span></span>
<span data-ttu-id="59de2-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [resourceOperation](../resources/intune-rbac-resourceoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59de2-129">If successful, this method returns a `200 OK` response code and a collection of [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59de2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59de2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="59de2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59de2-131">Request</span></span>
<span data-ttu-id="59de2-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59de2-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations
```

### <a name="response"></a><span data-ttu-id="59de2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="59de2-133">Response</span></span>
<span data-ttu-id="59de2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59de2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




