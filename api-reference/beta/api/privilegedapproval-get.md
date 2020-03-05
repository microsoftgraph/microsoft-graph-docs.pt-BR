---
title: Get privilegedApproval
description: Recupere as propriedades e os relacionamentos do objeto privilegedapproval.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: c9451389fd863fef8af32d46288200a62e8b9f67
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455432"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="95abd-103">Get privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="95abd-103">Get privilegedApproval</span></span>

<span data-ttu-id="95abd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="95abd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95abd-105">Recupere as propriedades e os relacionamentos do objeto privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="95abd-105">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="95abd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="95abd-106">Permissions</span></span>
<span data-ttu-id="95abd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95abd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="95abd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95abd-109">Permission type</span></span>      | <span data-ttu-id="95abd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95abd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95abd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95abd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="95abd-112">PrivilegedAccess. ReadWrite. AzureAD, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="95abd-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="95abd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95abd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95abd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95abd-114">Not supported.</span></span>    |
|<span data-ttu-id="95abd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95abd-115">Application</span></span> | <span data-ttu-id="95abd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95abd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="95abd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95abd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="95abd-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="95abd-118">Optional query parameters</span></span>
<span data-ttu-id="95abd-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="95abd-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="95abd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95abd-120">Request headers</span></span>
| <span data-ttu-id="95abd-121">Nome</span><span class="sxs-lookup"><span data-stu-id="95abd-121">Name</span></span>      |<span data-ttu-id="95abd-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="95abd-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="95abd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="95abd-123">Authorization</span></span>  | <span data-ttu-id="95abd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95abd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95abd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95abd-126">Request body</span></span>
<span data-ttu-id="95abd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="95abd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95abd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="95abd-128">Response</span></span>

<span data-ttu-id="95abd-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95abd-129">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="95abd-130">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="95abd-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="95abd-131">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="95abd-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="95abd-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95abd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="95abd-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95abd-133">Request</span></span>
<span data-ttu-id="95abd-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95abd-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="95abd-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="95abd-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedApproval/{id}
```
# <a name="c"></a>[<span data-ttu-id="95abd-136">C#</span><span class="sxs-lookup"><span data-stu-id="95abd-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95abd-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95abd-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95abd-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95abd-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="95abd-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="95abd-139">Response</span></span>
<span data-ttu-id="95abd-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95abd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
