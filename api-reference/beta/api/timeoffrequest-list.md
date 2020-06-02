---
title: Listar timeOffRequests
description: Recupere uma lista de objetos timeOffRequest na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d30670bc1183c27a405e5dcae6addda1554cd1c3
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44217054"
---
# <a name="list-timeoffrequest"></a><span data-ttu-id="c7cfc-103">Listar timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="c7cfc-103">List timeOffRequest</span></span>

<span data-ttu-id="c7cfc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7cfc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7cfc-105">Recupere uma lista de objetos [timeoffrequest](../resources/timeoffrequest.md) na equipe.</span><span class="sxs-lookup"><span data-stu-id="c7cfc-105">Retrieve a list of [timeoffrequest](../resources/timeoffrequest.md) objects in the team.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7cfc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7cfc-106">Permissions</span></span>

<span data-ttu-id="c7cfc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7cfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7cfc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7cfc-109">Permission type</span></span>                        | <span data-ttu-id="c7cfc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7cfc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="c7cfc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7cfc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c7cfc-112">Schedule. Read. All, Group. Read. All, Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c7cfc-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c7cfc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7cfc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7cfc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7cfc-114">Not supported.</span></span>    |
|<span data-ttu-id="c7cfc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7cfc-115">Application</span></span> | <span data-ttu-id="c7cfc-116">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="c7cfc-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="c7cfc-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="c7cfc-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="c7cfc-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="c7cfc-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c7cfc-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="c7cfc-119">Global admins can access groups that they are not a member of.</span></span> 

## <a name="http-request"></a><span data-ttu-id="c7cfc-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7cfc-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7cfc-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c7cfc-121">Optional query parameters</span></span>

<span data-ttu-id="c7cfc-122">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c7cfc-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c7cfc-123">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c7cfc-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7cfc-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7cfc-124">Request headers</span></span>

| <span data-ttu-id="c7cfc-125">Nome</span><span class="sxs-lookup"><span data-stu-id="c7cfc-125">Name</span></span>      |<span data-ttu-id="c7cfc-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7cfc-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c7cfc-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7cfc-127">Authorization</span></span> | <span data-ttu-id="c7cfc-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7cfc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7cfc-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7cfc-130">Request body</span></span>

<span data-ttu-id="c7cfc-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7cfc-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7cfc-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7cfc-132">Response</span></span>

<span data-ttu-id="c7cfc-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e os objetos [timeOffRequest](../resources/timeoffrequest.md) solicitados no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7cfc-133">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c7cfc-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c7cfc-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7cfc-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7cfc-135">Request</span></span>

<span data-ttu-id="c7cfc-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7cfc-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c7cfc-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7cfc-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests
```
# <a name="c"></a>[<span data-ttu-id="c7cfc-138">C#</span><span class="sxs-lookup"><span data-stu-id="c7cfc-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7cfc-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7cfc-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7cfc-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7cfc-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="c7cfc-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7cfc-141">Response</span></span>

<span data-ttu-id="c7cfc-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c7cfc-142">The following is an example of the response.</span></span>

> <span data-ttu-id="c7cfc-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7cfc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
