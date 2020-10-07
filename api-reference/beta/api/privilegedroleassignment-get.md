---
title: Get privilegedRoleAssignment
description: Recupere as propriedades e os relacionamentos do objeto privilegedRoleAssignment.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 95e03214de4bd926ba6ebf5f889aceff4be5b99f
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373794"
---
# <a name="get-privilegedroleassignment"></a><span data-ttu-id="8bdbf-103">Get privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="8bdbf-103">Get privilegedRoleAssignment</span></span>

<span data-ttu-id="8bdbf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bdbf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bdbf-105">Recupere as propriedades e os relacionamentos do objeto privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="8bdbf-105">Retrieve the properties and relationships of privilegedRoleAssignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8bdbf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8bdbf-106">Permissions</span></span>
<span data-ttu-id="8bdbf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bdbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8bdbf-109">O solicitante precisa ter uma das seguintes funções: administrador de _função privilegiada_, _administrador global_, _administrador de segurança_ou _leitor de segurança_.</span><span class="sxs-lookup"><span data-stu-id="8bdbf-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="8bdbf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bdbf-110">Permission type</span></span>      | <span data-ttu-id="8bdbf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8bdbf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bdbf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bdbf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8bdbf-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8bdbf-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8bdbf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bdbf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bdbf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bdbf-115">Not supported.</span></span>    |
|<span data-ttu-id="8bdbf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8bdbf-116">Application</span></span> | <span data-ttu-id="8bdbf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bdbf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bdbf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bdbf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8bdbf-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8bdbf-119">Optional query parameters</span></span>
<span data-ttu-id="8bdbf-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8bdbf-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8bdbf-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8bdbf-121">Request headers</span></span>
| <span data-ttu-id="8bdbf-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8bdbf-122">Name</span></span>      |<span data-ttu-id="8bdbf-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bdbf-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8bdbf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8bdbf-124">Authorization</span></span>  | <span data-ttu-id="8bdbf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bdbf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bdbf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8bdbf-127">Request body</span></span>
<span data-ttu-id="8bdbf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8bdbf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bdbf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bdbf-129">Response</span></span>

<span data-ttu-id="8bdbf-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bdbf-130">If successful, this method returns a `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="8bdbf-131">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="8bdbf-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="8bdbf-132">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="8bdbf-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="8bdbf-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8bdbf-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8bdbf-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bdbf-134">Request</span></span>
<span data-ttu-id="8bdbf-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8bdbf-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8bdbf-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bdbf-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="8bdbf-137">C#</span><span class="sxs-lookup"><span data-stu-id="8bdbf-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8bdbf-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bdbf-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8bdbf-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bdbf-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8bdbf-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bdbf-140">Response</span></span>
<span data-ttu-id="8bdbf-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8bdbf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
