---
title: Obter linkedResource
description: Leia as propriedades e os relacionamentos de um objeto linkedResource.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2806eb145db6be03a4d217c6d77bc0ceb9894322
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849864"
---
# <a name="get-linkedresource"></a><span data-ttu-id="f7fe3-103">Obter linkedResource</span><span class="sxs-lookup"><span data-stu-id="f7fe3-103">Get linkedResource</span></span>
<span data-ttu-id="f7fe3-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="f7fe3-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="f7fe3-105">Leia as propriedades e os relacionamentos de um objeto [linkedResource](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="f7fe3-105">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7fe3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7fe3-106">Permissions</span></span>
<span data-ttu-id="f7fe3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7fe3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7fe3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7fe3-109">Permission type</span></span>|<span data-ttu-id="f7fe3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f7fe3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7fe3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7fe3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f7fe3-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7fe3-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f7fe3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7fe3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7fe3-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7fe3-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f7fe3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7fe3-115">Application</span></span>|<span data-ttu-id="f7fe3-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f7fe3-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7fe3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7fe3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="f7fe3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7fe3-118">Request headers</span></span>
|<span data-ttu-id="f7fe3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f7fe3-119">Name</span></span>|<span data-ttu-id="f7fe3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7fe3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f7fe3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7fe3-121">Authorization</span></span>|<span data-ttu-id="f7fe3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7fe3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7fe3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7fe3-124">Request body</span></span>
<span data-ttu-id="f7fe3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7fe3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7fe3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7fe3-126">Response</span></span>

<span data-ttu-id="f7fe3-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [linkedResource](../resources/linkedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7fe3-127">If successful, this method returns a `200 OK` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7fe3-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f7fe3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7fe3-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7fe3-129">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "get_linkedresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
```


### <a name="response"></a><span data-ttu-id="f7fe3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7fe3-130">Response</span></span>
<span data-ttu-id="f7fe3-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f7fe3-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.linkedResource"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
     "@odata.type": "#microsoft.graph.linkedResource",
      "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
      "webUrl": "http://microsoft.com",
      "applicationName": "Microsoft",
      "displayName": "Microsoft",
      "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
  }
}
```