---
title: Obter openShiftChangeRequest
description: Recupere as propriedades e as relações de um objeto openShiftChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c1b0e8e298fe862d889884ac38f20afa0083782c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052226"
---
# <a name="get-openshiftchangerequest"></a><span data-ttu-id="29790-103">Obter openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="29790-103">Get openShiftChangeRequest</span></span>

<span data-ttu-id="29790-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29790-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="29790-105">Recupere as propriedades e as relações de um [objeto openShiftChangeRequest.](../resources/openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="29790-105">Retrieve the properties and relationships of an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="29790-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="29790-106">Permissions</span></span>

<span data-ttu-id="29790-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29790-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="29790-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29790-109">Permission type</span></span>                        | <span data-ttu-id="29790-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29790-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="29790-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29790-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="29790-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29790-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="29790-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29790-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29790-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29790-114">Not supported.</span></span> |
| <span data-ttu-id="29790-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29790-115">Application</span></span>                            | <span data-ttu-id="29790-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29790-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="29790-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="29790-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="29790-118">Os administradores globais podem acessar grupos dos que não são membros.</span><span class="sxs-lookup"><span data-stu-id="29790-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="29790-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29790-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShiftChangeRequests/{openShiftsChangeRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="29790-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="29790-120">Optional query parameters</span></span>

<span data-ttu-id="29790-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="29790-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="29790-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="29790-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="29790-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29790-123">Request headers</span></span>

| <span data-ttu-id="29790-124">Nome</span><span class="sxs-lookup"><span data-stu-id="29790-124">Name</span></span>      |<span data-ttu-id="29790-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="29790-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="29790-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="29790-126">Authorization</span></span> | <span data-ttu-id="29790-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29790-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29790-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29790-129">Request body</span></span>

<span data-ttu-id="29790-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="29790-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29790-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="29790-131">Response</span></span>

<span data-ttu-id="29790-132">Se tiver êxito, este método retornará um código de resposta e o objeto `200 OK` [openShiftChangeRequest](../resources/openshiftchangerequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29790-132">If successful, this method returns a `200 OK` response code and the requested [openShiftChangeRequest](../resources/openshiftchangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="29790-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="29790-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="29790-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29790-134">Request</span></span>

<span data-ttu-id="29790-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="29790-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="29790-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="29790-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_openshiftchangerequest_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShiftChangeRequests/SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09
```
# <a name="c"></a>[<span data-ttu-id="29790-137">C#</span><span class="sxs-lookup"><span data-stu-id="29790-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-openshiftchangerequest-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29790-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29790-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-openshiftchangerequest-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29790-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29790-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-openshiftchangerequest-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29790-140">Java</span><span class="sxs-lookup"><span data-stu-id="29790-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-openshiftchangerequest-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="29790-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="29790-141">Response</span></span>

<span data-ttu-id="29790-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="29790-142">The following is an example of the response.</span></span>

> <span data-ttu-id="29790-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="29790-143">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShiftChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09",
  "openShiftId": "577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "assignedTo": "manager",
  "state": "pending",
  "senderUserId": "3fe0bc21-1398-4fd9-9713-52511b434c1e",
  "senderDateTime": "2019-05-01T10:00:00Z",
  "senderMessage": "Can I take this shift?",
  "managerUserId": null,
  "managerActionDateTime": null,
  "managerActionMessage": null,
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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get openShiftChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

