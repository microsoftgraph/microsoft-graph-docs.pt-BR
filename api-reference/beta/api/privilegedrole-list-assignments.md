---
title: Listar tarefas
description: Recupere uma lista de objetos privilegedRoleAssignment associados à função. Cada privilegedRoleAssignment representa uma atribuição de função a um usuário.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 298742424152f7e483d709b33a6668e61cd866c3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441316"
---
# <a name="list-assignments"></a><span data-ttu-id="d5f26-104">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="d5f26-104">List assignments</span></span>

<span data-ttu-id="d5f26-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5f26-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5f26-106">Recupere uma lista de [objetos privilegedRoleAssignment](../resources/privilegedroleassignment.md) associados à função.</span><span class="sxs-lookup"><span data-stu-id="d5f26-106">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="d5f26-107">Cada [privilegedRoleAssignment](../resources/privilegedroleassignment.md) representa uma atribuição de função a um usuário.</span><span class="sxs-lookup"><span data-stu-id="d5f26-107">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="d5f26-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5f26-108">Permissions</span></span>
<span data-ttu-id="d5f26-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5f26-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d5f26-111">O solicitante precisa ter uma das seguintes funções: Administrador de Função _Privilegiada,_ _Administrador Global,_ Administrador de Segurança _ou_ Leitor de _Segurança._</span><span class="sxs-lookup"><span data-stu-id="d5f26-111">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="d5f26-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5f26-112">Permission type</span></span>      | <span data-ttu-id="d5f26-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5f26-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5f26-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5f26-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d5f26-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d5f26-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d5f26-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5f26-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5f26-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5f26-117">Not supported.</span></span>    |
|<span data-ttu-id="d5f26-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5f26-118">Application</span></span> | <span data-ttu-id="d5f26-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5f26-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5f26-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5f26-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="d5f26-121">Observe que ``{id}`` é a ID da função de destino.</span><span class="sxs-lookup"><span data-stu-id="d5f26-121">Note that ``{id}`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="d5f26-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d5f26-122">Optional query parameters</span></span>
<span data-ttu-id="d5f26-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d5f26-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5f26-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5f26-124">Request headers</span></span>
| <span data-ttu-id="d5f26-125">Nome</span><span class="sxs-lookup"><span data-stu-id="d5f26-125">Name</span></span>      |<span data-ttu-id="d5f26-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5f26-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d5f26-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5f26-127">Authorization</span></span>  | <span data-ttu-id="d5f26-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5f26-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5f26-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5f26-130">Request body</span></span>
<span data-ttu-id="d5f26-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d5f26-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5f26-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5f26-132">Response</span></span>

<span data-ttu-id="d5f26-133">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5f26-133">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="d5f26-134">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="d5f26-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="d5f26-135">Caso contrário, o código de status HTTP 403 Forbidden será retornado.</span><span class="sxs-lookup"><span data-stu-id="d5f26-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="d5f26-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5f26-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5f26-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5f26-137">Request</span></span>
<span data-ttu-id="d5f26-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5f26-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d5f26-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5f26-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
# <a name="c"></a>[<span data-ttu-id="d5f26-140">C#</span><span class="sxs-lookup"><span data-stu-id="d5f26-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-assignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5f26-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5f26-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-assignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5f26-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5f26-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-assignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d5f26-143">Java</span><span class="sxs-lookup"><span data-stu-id="d5f26-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-assignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d5f26-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5f26-144">Response</span></span>
<span data-ttu-id="d5f26-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5f26-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
