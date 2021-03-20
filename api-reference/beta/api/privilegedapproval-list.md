---
title: List privilegedApproval
description: Recupere uma lista de objetos privilegedapproval.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: a806dc46ea34853a7c0182b0c37675541740f6c0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961425"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="28e0e-103">List privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="28e0e-103">List privilegedApproval</span></span>

<span data-ttu-id="28e0e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28e0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28e0e-105">Recupere uma lista de objetos privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="28e0e-105">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="28e0e-106">Para filtrar os resultados da consulta, use as expressões ``$filter`` padrão do OData nos URIs.</span><span class="sxs-lookup"><span data-stu-id="28e0e-106">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="28e0e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="28e0e-107">Permissions</span></span>
<span data-ttu-id="28e0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28e0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="28e0e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28e0e-110">Permission type</span></span>      | <span data-ttu-id="28e0e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28e0e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28e0e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28e0e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="28e0e-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="28e0e-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="28e0e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28e0e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28e0e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28e0e-115">Not supported.</span></span>    |
|<span data-ttu-id="28e0e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28e0e-116">Application</span></span> | <span data-ttu-id="28e0e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28e0e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="28e0e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28e0e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="28e0e-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="28e0e-119">Optional query parameters</span></span>
<span data-ttu-id="28e0e-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="28e0e-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28e0e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28e0e-121">Request headers</span></span>
| <span data-ttu-id="28e0e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="28e0e-122">Name</span></span>      |<span data-ttu-id="28e0e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="28e0e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="28e0e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="28e0e-124">Authorization</span></span>  | <span data-ttu-id="28e0e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28e0e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28e0e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28e0e-127">Request body</span></span>
<span data-ttu-id="28e0e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28e0e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28e0e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="28e0e-129">Response</span></span>

<span data-ttu-id="28e0e-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28e0e-130">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="28e0e-131">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="28e0e-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="28e0e-132">Caso contrário, o código de status HTTP 403 Forbidden será retornado.</span><span class="sxs-lookup"><span data-stu-id="28e0e-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="28e0e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28e0e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28e0e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28e0e-134">Request</span></span>
<span data-ttu-id="28e0e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28e0e-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28e0e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="28e0e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedApproval
```
# <a name="c"></a>[<span data-ttu-id="28e0e-137">C#</span><span class="sxs-lookup"><span data-stu-id="28e0e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedapproval-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28e0e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28e0e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedapproval-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28e0e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28e0e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedapproval-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28e0e-140">Java</span><span class="sxs-lookup"><span data-stu-id="28e0e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedapproval-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="28e0e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="28e0e-141">Response</span></span>
<span data-ttu-id="28e0e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28e0e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
