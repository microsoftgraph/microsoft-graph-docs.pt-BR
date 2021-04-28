---
title: Listar openShifts
description: Listar objetos openshift em uma equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: afde5a9badc018657254dbedab476ecfb5a759bc
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035285"
---
# <a name="list-openshifts"></a><span data-ttu-id="7f666-103">Listar openShifts</span><span class="sxs-lookup"><span data-stu-id="7f666-103">List openShifts</span></span>

<span data-ttu-id="7f666-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f666-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7f666-105">Listar [objetos openShift](../resources/openshift.md) em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="7f666-105">List [openShift](../resources/openshift.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f666-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f666-106">Permissions</span></span>

<span data-ttu-id="7f666-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f666-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f666-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f666-109">Permission type</span></span>                        | <span data-ttu-id="7f666-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f666-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7f666-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f666-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f666-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f666-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="7f666-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f666-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f666-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f666-114">Not supported.</span></span> |
| <span data-ttu-id="7f666-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f666-115">Application</span></span>                            | <span data-ttu-id="7f666-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f666-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="7f666-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="7f666-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="7f666-118">Os administradores globais podem acessar grupos dos que não são membros.</span><span class="sxs-lookup"><span data-stu-id="7f666-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="7f666-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f666-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShifts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f666-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7f666-120">Optional query parameters</span></span>

<span data-ttu-id="7f666-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7f666-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7f666-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7f666-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>
  
## <a name="request-headers"></a><span data-ttu-id="7f666-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f666-123">Request headers</span></span>

| <span data-ttu-id="7f666-124">Nome</span><span class="sxs-lookup"><span data-stu-id="7f666-124">Name</span></span>      |<span data-ttu-id="7f666-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f666-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7f666-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f666-126">Authorization</span></span> | <span data-ttu-id="7f666-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f666-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f666-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f666-129">Request body</span></span>

<span data-ttu-id="7f666-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7f666-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f666-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f666-131">Response</span></span>

<span data-ttu-id="7f666-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e todos os objetos [openShift](../resources/openshift.md) na equipe no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f666-132">If successful, this method returns a `200 OK` response code and all [openShift](../resources/openshift.md) objects in the team in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7f666-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7f666-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7f666-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f666-134">Request</span></span>

<span data-ttu-id="7f666-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f666-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7f666-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f666-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_openshift_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShifts
```
# <a name="c"></a>[<span data-ttu-id="7f666-137">C#</span><span class="sxs-lookup"><span data-stu-id="7f666-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-openshift-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f666-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f666-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-openshift-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f666-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f666-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-openshift-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f666-140">Java</span><span class="sxs-lookup"><span data-stu-id="7f666-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-openshift-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="7f666-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f666-141">Response</span></span>

<span data-ttu-id="7f666-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7f666-142">The following is an example of the response.</span></span>

> <span data-ttu-id="7f666-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7f666-143">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
  {
  "id": "OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "sharedOpenShift": {
  "notes": "Inventory Management",
  "openSlotCount":2,
  "displayName": "Day shift",
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T09:50:45.332Z",
  "theme": "white",
  "activities": [
  {
  "isPaid": true,
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T01:58:45.340Z",
  "code": "",
  "displayName": "Lunch"
  }
  ]
  },
  "draftOpenShift": {
  "notes": "Inventory Management",
  "openSlotCount":3,
  "displayName": "Day shift",
  "startDateTime": "2018-10-04T00:58:45.332Z",
  "endDateTime": "2018-10-04T08:58:45.340Z",
  "theme": "white",
  "activities": [
  {
  "isPaid": true,
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T07:58:45.332Z",
  "code": "Break",
  "displayName": "Lunch"
  }
  ]
  },
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "lastModifiedBy": {
  "application": null,
  "device": null,
  "conversation": null,
  "user": {
  "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
  "displayName": "John Doe"
  }
  }
  }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

