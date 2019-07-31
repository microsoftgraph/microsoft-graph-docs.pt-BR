---
title: Listar tarefas
description: Recupere uma lista de objetos privilegedRoleAssignment que estão associados à função. Cada privilegedRoleAssignment representa uma atribuição de função a um usuário.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5deac12d589f97fd64958cf791067142446546ca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983359"
---
# <a name="list-assignments"></a><span data-ttu-id="f330f-104">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="f330f-104">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f330f-105">Recupere uma lista de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) que estão associados à função.</span><span class="sxs-lookup"><span data-stu-id="f330f-105">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="f330f-106">Cada [privilegedRoleAssignment](../resources/privilegedroleassignment.md) representa uma atribuição de função a um usuário.</span><span class="sxs-lookup"><span data-stu-id="f330f-106">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="f330f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f330f-107">Permissions</span></span>
<span data-ttu-id="f330f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f330f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f330f-110">O solicitante precisa ter uma das seguintes funções: administrador de _função privilegiada_, _administrador global_, _administrador de segurança_ou _leitor de segurança_.</span><span class="sxs-lookup"><span data-stu-id="f330f-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="f330f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f330f-111">Permission type</span></span>      | <span data-ttu-id="f330f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f330f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f330f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f330f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f330f-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f330f-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f330f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f330f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f330f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f330f-116">Not supported.</span></span>    |
|<span data-ttu-id="f330f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f330f-117">Application</span></span> | <span data-ttu-id="f330f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f330f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f330f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f330f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="f330f-120">Observe que ``<id>`` é a ID da função de destino.</span><span class="sxs-lookup"><span data-stu-id="f330f-120">Note that ``<id>`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="f330f-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f330f-121">Optional query parameters</span></span>
<span data-ttu-id="f330f-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f330f-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f330f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f330f-123">Request headers</span></span>
| <span data-ttu-id="f330f-124">Nome</span><span class="sxs-lookup"><span data-stu-id="f330f-124">Name</span></span>      |<span data-ttu-id="f330f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f330f-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f330f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="f330f-126">Authorization</span></span>  | <span data-ttu-id="f330f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f330f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f330f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f330f-129">Request body</span></span>
<span data-ttu-id="f330f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f330f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f330f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f330f-131">Response</span></span>

<span data-ttu-id="f330f-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f330f-132">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="f330f-133">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="f330f-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="f330f-134">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="f330f-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="f330f-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f330f-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f330f-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f330f-136">Request</span></span>
<span data-ttu-id="f330f-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f330f-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f330f-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="f330f-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f330f-139">C#</span><span class="sxs-lookup"><span data-stu-id="f330f-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-assignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f330f-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="f330f-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-assignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f330f-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f330f-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-assignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f330f-142">Java</span><span class="sxs-lookup"><span data-stu-id="f330f-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-assignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f330f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f330f-143">Response</span></span>
<span data-ttu-id="f330f-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f330f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
