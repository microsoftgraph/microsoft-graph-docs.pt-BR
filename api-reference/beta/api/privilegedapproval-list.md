---
title: List privilegedApproval
description: Recupere uma lista de objetos privilegedapproval.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: ec53c87df049e0eab2a48256d6cfbc7d67a2b0f7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053549"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="28e97-103">List privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="28e97-103">List privilegedApproval</span></span>

<span data-ttu-id="28e97-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28e97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28e97-105">Recupere uma lista de objetos privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="28e97-105">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="28e97-106">Para filtrar os resultados da consulta, use as expressões ``$filter`` padrão do OData nos URIs.</span><span class="sxs-lookup"><span data-stu-id="28e97-106">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="28e97-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="28e97-107">Permissions</span></span>
<span data-ttu-id="28e97-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28e97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="28e97-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28e97-110">Permission type</span></span>      | <span data-ttu-id="28e97-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28e97-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28e97-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28e97-112">Delegated (work or school account)</span></span> | <span data-ttu-id="28e97-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="28e97-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="28e97-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28e97-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28e97-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28e97-115">Not supported.</span></span>    |
|<span data-ttu-id="28e97-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28e97-116">Application</span></span> | <span data-ttu-id="28e97-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28e97-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="28e97-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28e97-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="28e97-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="28e97-119">Optional query parameters</span></span>
<span data-ttu-id="28e97-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="28e97-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28e97-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28e97-121">Request headers</span></span>
| <span data-ttu-id="28e97-122">Nome</span><span class="sxs-lookup"><span data-stu-id="28e97-122">Name</span></span>      |<span data-ttu-id="28e97-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="28e97-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="28e97-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="28e97-124">Authorization</span></span>  | <span data-ttu-id="28e97-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28e97-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28e97-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28e97-127">Request body</span></span>
<span data-ttu-id="28e97-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28e97-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28e97-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="28e97-129">Response</span></span>

<span data-ttu-id="28e97-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28e97-130">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="28e97-131">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="28e97-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="28e97-132">Caso contrário, o código de status HTTP 403 Forbidden será retornado.</span><span class="sxs-lookup"><span data-stu-id="28e97-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="28e97-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28e97-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28e97-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28e97-134">Request</span></span>
<span data-ttu-id="28e97-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28e97-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28e97-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="28e97-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedApproval
```
# <a name="c"></a>[<span data-ttu-id="28e97-137">C#</span><span class="sxs-lookup"><span data-stu-id="28e97-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedapproval-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28e97-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28e97-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedapproval-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28e97-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28e97-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedapproval-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28e97-140">Java</span><span class="sxs-lookup"><span data-stu-id="28e97-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedapproval-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="28e97-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="28e97-141">Response</span></span>
<span data-ttu-id="28e97-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28e97-142">Here is an example of the response.</span></span> <span data-ttu-id="28e97-143">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="28e97-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 246

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "approvalType": "approvalType-value",
      "approvalState": "approvalState-value",
      "approvalDuration": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
