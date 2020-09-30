---
title: Listar tarefas
description: Recupere uma lista de objetos privilegedRoleAssignment que estão associados à função. Cada privilegedRoleAssignment representa uma atribuição de função a um usuário.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 02a282546778e2de558f7f770426969a96441071
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315025"
---
# <a name="list-assignments"></a><span data-ttu-id="61471-104">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="61471-104">List assignments</span></span>

<span data-ttu-id="61471-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61471-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61471-106">Recupere uma lista de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) que estão associados à função.</span><span class="sxs-lookup"><span data-stu-id="61471-106">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="61471-107">Cada [privilegedRoleAssignment](../resources/privilegedroleassignment.md) representa uma atribuição de função a um usuário.</span><span class="sxs-lookup"><span data-stu-id="61471-107">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="61471-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="61471-108">Permissions</span></span>
<span data-ttu-id="61471-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61471-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="61471-111">O solicitante precisa ter uma das seguintes funções: administrador de _função privilegiada_, _administrador global_, _administrador de segurança_ou _leitor de segurança_.</span><span class="sxs-lookup"><span data-stu-id="61471-111">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="61471-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61471-112">Permission type</span></span>      | <span data-ttu-id="61471-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61471-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61471-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61471-114">Delegated (work or school account)</span></span> | <span data-ttu-id="61471-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="61471-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="61471-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61471-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61471-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61471-117">Not supported.</span></span>    |
|<span data-ttu-id="61471-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61471-118">Application</span></span> | <span data-ttu-id="61471-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61471-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="61471-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61471-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="61471-121">Observe que ``{id}`` é a ID da função de destino.</span><span class="sxs-lookup"><span data-stu-id="61471-121">Note that ``{id}`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="61471-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="61471-122">Optional query parameters</span></span>
<span data-ttu-id="61471-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="61471-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61471-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61471-124">Request headers</span></span>
| <span data-ttu-id="61471-125">Nome</span><span class="sxs-lookup"><span data-stu-id="61471-125">Name</span></span>      |<span data-ttu-id="61471-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="61471-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="61471-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="61471-127">Authorization</span></span>  | <span data-ttu-id="61471-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61471-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61471-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61471-130">Request body</span></span>
<span data-ttu-id="61471-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="61471-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61471-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="61471-132">Response</span></span>

<span data-ttu-id="61471-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61471-133">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="61471-134">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="61471-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="61471-135">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="61471-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="61471-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61471-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="61471-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61471-137">Request</span></span>
<span data-ttu-id="61471-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61471-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="61471-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="61471-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
# <a name="c"></a>[<span data-ttu-id="61471-140">C#</span><span class="sxs-lookup"><span data-stu-id="61471-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-assignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61471-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61471-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-assignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61471-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61471-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-assignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="61471-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="61471-143">Response</span></span>
<span data-ttu-id="61471-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61471-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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