---
title: Get privilegedRoleAssignment
description: Recupere as propriedades e os relacionamentos do objeto privilegedRoleAssignment.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9144f5eefdf21efaef28e0897221444336db7858
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412723"
---
# <a name="get-privilegedroleassignment"></a><span data-ttu-id="11d12-103">Get privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="11d12-103">Get privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11d12-104">Recupere as propriedades e os relacionamentos do objeto privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="11d12-104">Retrieve the properties and relationships of privilegedRoleAssignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="11d12-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="11d12-105">Permissions</span></span>
<span data-ttu-id="11d12-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11d12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="11d12-108">O solicitante precisa ter uma das seguintes funções: administrador de _função privilegiada_, _administrador global_, _administrador de segurança_ou _leitor de segurança_.</span><span class="sxs-lookup"><span data-stu-id="11d12-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="11d12-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11d12-109">Permission type</span></span>      | <span data-ttu-id="11d12-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11d12-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11d12-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11d12-111">Delegated (work or school account)</span></span> | <span data-ttu-id="11d12-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="11d12-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="11d12-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11d12-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11d12-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11d12-114">Not supported.</span></span>    |
|<span data-ttu-id="11d12-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11d12-115">Application</span></span> | <span data-ttu-id="11d12-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11d12-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11d12-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11d12-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="11d12-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="11d12-118">Optional query parameters</span></span>
<span data-ttu-id="11d12-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="11d12-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11d12-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11d12-120">Request headers</span></span>
| <span data-ttu-id="11d12-121">Nome</span><span class="sxs-lookup"><span data-stu-id="11d12-121">Name</span></span>      |<span data-ttu-id="11d12-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="11d12-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="11d12-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="11d12-123">Authorization</span></span>  | <span data-ttu-id="11d12-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11d12-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11d12-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11d12-126">Request body</span></span>
<span data-ttu-id="11d12-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="11d12-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11d12-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="11d12-128">Response</span></span>

<span data-ttu-id="11d12-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11d12-129">If successful, this method returns a `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="11d12-130">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="11d12-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="11d12-131">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="11d12-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="11d12-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11d12-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11d12-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11d12-133">Request</span></span>
<span data-ttu-id="11d12-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11d12-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="11d12-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="11d12-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="11d12-136">C#</span><span class="sxs-lookup"><span data-stu-id="11d12-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="11d12-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11d12-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="11d12-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="11d12-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="11d12-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="11d12-139">Response</span></span>
<span data-ttu-id="11d12-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11d12-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
