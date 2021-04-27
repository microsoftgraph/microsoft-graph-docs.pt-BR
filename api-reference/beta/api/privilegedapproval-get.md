---
title: Get privilegedApproval
description: Recupere as propriedades e as relações do objeto privilegedapproval.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: c51cf8c0629e5244c4cd9a06eaf9c85afe443d53
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049853"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="4d550-103">Get privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="4d550-103">Get privilegedApproval</span></span>

<span data-ttu-id="4d550-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d550-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d550-105">Recupere as propriedades e as relações do objeto privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="4d550-105">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4d550-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d550-106">Permissions</span></span>
<span data-ttu-id="4d550-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d550-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4d550-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d550-109">Permission type</span></span>      | <span data-ttu-id="4d550-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d550-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d550-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d550-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4d550-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4d550-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="4d550-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d550-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d550-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d550-114">Not supported.</span></span>    |
|<span data-ttu-id="4d550-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d550-115">Application</span></span> | <span data-ttu-id="4d550-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d550-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d550-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d550-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4d550-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4d550-118">Optional query parameters</span></span>
<span data-ttu-id="4d550-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4d550-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d550-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d550-120">Request headers</span></span>
| <span data-ttu-id="4d550-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4d550-121">Name</span></span>      |<span data-ttu-id="4d550-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d550-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4d550-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d550-123">Authorization</span></span>  | <span data-ttu-id="4d550-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d550-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d550-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d550-126">Request body</span></span>
<span data-ttu-id="4d550-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4d550-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d550-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d550-128">Response</span></span>

<span data-ttu-id="4d550-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d550-129">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="4d550-130">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="4d550-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="4d550-131">Caso contrário, o código de status HTTP 403 Forbidden será retornado.</span><span class="sxs-lookup"><span data-stu-id="4d550-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="4d550-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d550-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d550-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d550-133">Request</span></span>
<span data-ttu-id="4d550-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d550-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4d550-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d550-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedApproval/{id}
```
# <a name="c"></a>[<span data-ttu-id="4d550-136">C#</span><span class="sxs-lookup"><span data-stu-id="4d550-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedapproval-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d550-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d550-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedapproval-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d550-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d550-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedapproval-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4d550-139">Java</span><span class="sxs-lookup"><span data-stu-id="4d550-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedapproval-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4d550-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d550-140">Response</span></span>
<span data-ttu-id="4d550-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d550-141">Here is an example of the response.</span></span> <span data-ttu-id="4d550-142">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4d550-142">Note: The response object shown here might be shortened for readability.</span></span>
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
