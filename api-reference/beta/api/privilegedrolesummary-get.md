---
title: Get privilegedRoleSummary
description: Recupere as propriedades e os relacionamentos do objeto privilegedRoleSummary.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 6ce046aa9be1a57bfb99e40392be71a2aab7d784
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034907"
---
# <a name="get-privilegedrolesummary"></a><span data-ttu-id="12a6a-103">Get privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="12a6a-103">Get privilegedRoleSummary</span></span>

<span data-ttu-id="12a6a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12a6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12a6a-105">Recupere as propriedades e os relacionamentos do objeto [privilegedRoleSummary](../resources/privilegedrolesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="12a6a-105">Retrieve the properties and relationships of [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="12a6a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="12a6a-106">Permissions</span></span>
<span data-ttu-id="12a6a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12a6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="12a6a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12a6a-109">Permission type</span></span>      | <span data-ttu-id="12a6a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12a6a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12a6a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12a6a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="12a6a-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="12a6a-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="12a6a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12a6a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12a6a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12a6a-114">Not supported.</span></span>    |
|<span data-ttu-id="12a6a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12a6a-115">Application</span></span> | <span data-ttu-id="12a6a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12a6a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12a6a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12a6a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}?$expand=summary
```
## <a name="optional-query-parameters"></a><span data-ttu-id="12a6a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="12a6a-118">Optional query parameters</span></span>
<span data-ttu-id="12a6a-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="12a6a-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12a6a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12a6a-120">Request headers</span></span>
| <span data-ttu-id="12a6a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="12a6a-121">Name</span></span>      |<span data-ttu-id="12a6a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="12a6a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="12a6a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="12a6a-123">Authorization</span></span>  | <span data-ttu-id="12a6a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12a6a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12a6a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12a6a-126">Request body</span></span>
<span data-ttu-id="12a6a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12a6a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12a6a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="12a6a-128">Response</span></span>

<span data-ttu-id="12a6a-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [privilegedRoleSummary](../resources/privilegedrolesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12a6a-129">If successful, this method returns a `200 OK` response code and [privilegedRoleSummary](../resources/privilegedrolesummary.md) object in the response body.</span></span>

<span data-ttu-id="12a6a-130">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="12a6a-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="12a6a-131">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="12a6a-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="12a6a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12a6a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12a6a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12a6a-133">Request</span></span>
<span data-ttu-id="12a6a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12a6a-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="12a6a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="12a6a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesummary"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/summary
```
# <a name="c"></a>[<span data-ttu-id="12a6a-136">C#</span><span class="sxs-lookup"><span data-stu-id="12a6a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrolesummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12a6a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12a6a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrolesummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12a6a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12a6a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrolesummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="12a6a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="12a6a-139">Response</span></span>
<span data-ttu-id="12a6a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12a6a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 137

{
  "id": "id-value",
  "status": "status-value",
  "usersCount": 99,
  "managedCount": 99,
  "elevatedCount": 99,
  "mfaEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


