---
title: Get privilegedRoleSummary
description: Recupere as propriedades e as relações do objeto privilegedRoleSummary.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: c03bc052a3a07e2ecf9237d3829f32667a4e2dd3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052877"
---
# <a name="get-privilegedrolesummary"></a><span data-ttu-id="6b132-103">Get privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="6b132-103">Get privilegedRoleSummary</span></span>

<span data-ttu-id="6b132-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b132-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b132-105">Recupere as propriedades e as relações do [objeto privilegedRoleSummary.](../resources/privilegedrolesummary.md)</span><span class="sxs-lookup"><span data-stu-id="6b132-105">Retrieve the properties and relationships of [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b132-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b132-106">Permissions</span></span>
<span data-ttu-id="6b132-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b132-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6b132-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b132-109">Permission type</span></span>      | <span data-ttu-id="6b132-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b132-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b132-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b132-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b132-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6b132-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6b132-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b132-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b132-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b132-114">Not supported.</span></span>    |
|<span data-ttu-id="6b132-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b132-115">Application</span></span> | <span data-ttu-id="6b132-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b132-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b132-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b132-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}?$expand=summary
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6b132-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6b132-118">Optional query parameters</span></span>
<span data-ttu-id="6b132-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6b132-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b132-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b132-120">Request headers</span></span>
| <span data-ttu-id="6b132-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6b132-121">Name</span></span>      |<span data-ttu-id="6b132-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b132-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6b132-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b132-123">Authorization</span></span>  | <span data-ttu-id="6b132-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b132-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b132-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b132-126">Request body</span></span>
<span data-ttu-id="6b132-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6b132-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b132-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b132-128">Response</span></span>

<span data-ttu-id="6b132-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [privilegedRoleSummary](../resources/privilegedrolesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b132-129">If successful, this method returns a `200 OK` response code and [privilegedRoleSummary](../resources/privilegedrolesummary.md) object in the response body.</span></span>

<span data-ttu-id="6b132-130">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="6b132-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="6b132-131">Caso contrário, o código de status HTTP 403 Forbidden será retornado.</span><span class="sxs-lookup"><span data-stu-id="6b132-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="6b132-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b132-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b132-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b132-133">Request</span></span>
<span data-ttu-id="6b132-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b132-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b132-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b132-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesummary"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/summary
```
# <a name="c"></a>[<span data-ttu-id="6b132-136">C#</span><span class="sxs-lookup"><span data-stu-id="6b132-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrolesummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b132-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b132-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrolesummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b132-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b132-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrolesummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b132-139">Java</span><span class="sxs-lookup"><span data-stu-id="6b132-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedrolesummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6b132-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b132-140">Response</span></span>
<span data-ttu-id="6b132-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b132-141">Here is an example of the response.</span></span> <span data-ttu-id="6b132-142">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6b132-142">Note: The response object shown here might be shortened for readability.</span></span>
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
