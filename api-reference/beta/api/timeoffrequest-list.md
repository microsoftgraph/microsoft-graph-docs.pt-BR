---
title: Listar timeOffRequests
description: Recupere uma lista de objetos timeOffRequest na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c874c1ff5074220f608484b3784b6f2b3630a269
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010469"
---
# <a name="list-timeoffrequest"></a><span data-ttu-id="ff50e-103">Listar timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="ff50e-103">List timeOffRequest</span></span>

<span data-ttu-id="ff50e-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ff50e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff50e-105">Recupere uma lista de objetos [timeoffrequest](../resources/timeoffrequest.md) na equipe.</span><span class="sxs-lookup"><span data-stu-id="ff50e-105">Retrieve a list of [timeoffrequest](../resources/timeoffrequest.md) objects in the team.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff50e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff50e-106">Permissions</span></span>

<span data-ttu-id="ff50e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff50e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff50e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff50e-109">Permission type</span></span>                        | <span data-ttu-id="ff50e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff50e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="ff50e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff50e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ff50e-112">Schedule. Read. All, Group. Read. All, Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ff50e-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ff50e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff50e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff50e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff50e-114">Not supported.</span></span>    |
|<span data-ttu-id="ff50e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff50e-115">Application</span></span> | <span data-ttu-id="ff50e-116">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="ff50e-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="ff50e-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="ff50e-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="ff50e-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="ff50e-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ff50e-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="ff50e-119">Global admins can access groups that they are not a member of.</span></span> 

## <a name="http-request"></a><span data-ttu-id="ff50e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff50e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff50e-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ff50e-121">Optional query parameters</span></span>

<span data-ttu-id="ff50e-122">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ff50e-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ff50e-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ff50e-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff50e-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff50e-124">Request headers</span></span>

| <span data-ttu-id="ff50e-125">Nome</span><span class="sxs-lookup"><span data-stu-id="ff50e-125">Name</span></span>      |<span data-ttu-id="ff50e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff50e-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ff50e-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff50e-127">Authorization</span></span> | <span data-ttu-id="ff50e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff50e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff50e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff50e-130">Request body</span></span>

<span data-ttu-id="ff50e-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff50e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff50e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff50e-132">Response</span></span>

<span data-ttu-id="ff50e-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e os objetos [timeOffRequest](../resources/timeoffrequest.md) solicitados no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff50e-133">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff50e-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ff50e-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ff50e-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff50e-135">Request</span></span>

<span data-ttu-id="ff50e-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff50e-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ff50e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff50e-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests
```
# <a name="c"></a>[<span data-ttu-id="ff50e-138">C#</span><span class="sxs-lookup"><span data-stu-id="ff50e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff50e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff50e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff50e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff50e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="ff50e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff50e-141">Response</span></span>

<span data-ttu-id="ff50e-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ff50e-142">The following is an example of the response.</span></span>

> <span data-ttu-id="ff50e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff50e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
        {
        "id": "0b87dd20-d5ed-4764-9c3e-cfc8516def09",
        "startDateTime": "datetime-value",
        "endDateTime": "datetime-value",
        "timeOffReasonId": "timeOffReasonId-value"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List timeOffRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


