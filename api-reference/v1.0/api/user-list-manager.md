---
title: Listar gerente
description: Obtenha o gerente do usuário. Retorna o usuário ou contato atribuído como gerente do usuário.
localization_priority: Priority
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 1b51b94b03f18647e8d3cf88036ecee22ab4de3a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943353"
---
# <a name="list-manager"></a><span data-ttu-id="18aa6-104">Listar gerente</span><span class="sxs-lookup"><span data-stu-id="18aa6-104">List manager</span></span>

<span data-ttu-id="18aa6-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18aa6-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18aa6-106">Retorna o usuário ou o contato organizacional atribuído como gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="18aa6-106">Returns the user or organizational contact assigned as the user's manager.</span></span> <span data-ttu-id="18aa6-107">Opcionalmente, você pode expandir a cadeia do gerente ao nó raiz.</span><span class="sxs-lookup"><span data-stu-id="18aa6-107">Optionally, you can expand the manager's chain up to the root node.</span></span>

## <a name="permissions"></a><span data-ttu-id="18aa6-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="18aa6-108">Permissions</span></span>

<span data-ttu-id="18aa6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18aa6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18aa6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18aa6-111">Permission type</span></span>      | <span data-ttu-id="18aa6-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18aa6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18aa6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18aa6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="18aa6-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="18aa6-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="18aa6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18aa6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18aa6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18aa6-116">Not supported.</span></span>    |
|<span data-ttu-id="18aa6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18aa6-117">Application</span></span> | <span data-ttu-id="18aa6-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18aa6-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="18aa6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18aa6-119">HTTP request</span></span>

<span data-ttu-id="18aa6-120">Obtenha o gerente:</span><span class="sxs-lookup"><span data-stu-id="18aa6-120">Get the manager:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
<span data-ttu-id="18aa6-121">Obtenha a cadeia de gerenciamento:</span><span class="sxs-lookup"><span data-stu-id="18aa6-121">Get the management chain:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me?$expand=manager
GET /users?$expand=manager($levels=n)
GET /users/{id | userPrincipalName}/?$expand=manager($levels=n)
```

## <a name="optional-query-parameters"></a><span data-ttu-id="18aa6-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="18aa6-122">Optional query parameters</span></span>

<span data-ttu-id="18aa6-123">Este método oferece suporte aos parâmetros de consulta `$select` e `$expand`[OData](/graph/query-parameters)para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="18aa6-123">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>  

><span data-ttu-id="18aa6-124">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="18aa6-124">**Note:**</span></span> 
> + <span data-ttu-id="18aa6-125">O valor `n` de `$levels` pode ser `max` (para retornar todos os gerentes) ou um número entre 1 e 1000.</span><span class="sxs-lookup"><span data-stu-id="18aa6-125">The `n` value of `$levels` can be `max` (to return all managers) or a number between 1 and 1000.</span></span>  
> + <span data-ttu-id="18aa6-126">Quando o `$levels` parâmetro não for especificado, apenas o gerente imediato será retornado.</span><span class="sxs-lookup"><span data-stu-id="18aa6-126">When the `$levels` parameter is not specified, only the immediate manager is returned.</span></span>  
> + <span data-ttu-id="18aa6-127">Você pode especificar `$select` dentro de `$expand` para selecionar as propriedades do gerente individual.</span><span class="sxs-lookup"><span data-stu-id="18aa6-127">You can specify `$select` inside `$expand` to select the individual manager's properties.</span></span> <span data-ttu-id="18aa6-128">O parâmetro `$levels` é obrigatório: `$expand=manager($levels=max;$select=id,displayName)`</span><span class="sxs-lookup"><span data-stu-id="18aa6-128">The `$levels` parameter is required: `$expand=manager($levels=max;$select=id,displayName)`</span></span>

## <a name="request-headers"></a><span data-ttu-id="18aa6-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18aa6-129">Request headers</span></span>

| <span data-ttu-id="18aa6-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18aa6-130">Header</span></span>       | <span data-ttu-id="18aa6-131">Valor</span><span class="sxs-lookup"><span data-stu-id="18aa6-131">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="18aa6-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="18aa6-132">Authorization</span></span>  | <span data-ttu-id="18aa6-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18aa6-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="18aa6-135">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="18aa6-135">ConsistencyLevel</span></span> | <span data-ttu-id="18aa6-136">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="18aa6-136">eventual.</span></span> <span data-ttu-id="18aa6-137">Obrigatório quando a solicitação inclui o parâmetro `$expand=manager($levels=max)`.</span><span class="sxs-lookup"><span data-stu-id="18aa6-137">Required when the request includes the `$expand=manager($levels=max)` parameter.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18aa6-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18aa6-138">Request body</span></span>

<span data-ttu-id="18aa6-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="18aa6-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18aa6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="18aa6-140">Response</span></span>

<span data-ttu-id="18aa6-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18aa6-141">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="18aa6-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="18aa6-142">Examples</span></span>

### <a name="example-1-get-manager"></a><span data-ttu-id="18aa6-143">Exemplo 1: obtenha o gerente</span><span class="sxs-lookup"><span data-stu-id="18aa6-143">Example 1: Get manager</span></span>

<span data-ttu-id="18aa6-144">O exemplo a seguir mostra uma solicitação para obter o gerente.</span><span class="sxs-lookup"><span data-stu-id="18aa6-144">The following example shows a request to get the manager.</span></span>

#### <a name="request"></a><span data-ttu-id="18aa6-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18aa6-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="18aa6-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="18aa6-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
# <a name="c"></a>[<span data-ttu-id="18aa6-147">C#</span><span class="sxs-lookup"><span data-stu-id="18aa6-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18aa6-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18aa6-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18aa6-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18aa6-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18aa6-150">Java</span><span class="sxs-lookup"><span data-stu-id="18aa6-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="18aa6-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="18aa6-151">Response</span></span>

<span data-ttu-id="18aa6-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="18aa6-152">The following is an example of the response.</span></span>
><span data-ttu-id="18aa6-153">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="18aa6-153">**Note**: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "<user-id>",
  "displayName": "Sara Davis",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```

### <a name="example-2-get-manager-chain-up-to-the-root-level"></a><span data-ttu-id="18aa6-154">Exemplo 2: obtenha a cadeia de gerentes ao nível raiz</span><span class="sxs-lookup"><span data-stu-id="18aa6-154">Example 2: Get manager chain up to the root level</span></span>

<span data-ttu-id="18aa6-155">O exemplo a seguir mostra uma solicitação para obter a cadeia de gerentes ao nível raiz.</span><span class="sxs-lookup"><span data-stu-id="18aa6-155">The following example shows a request to get the manager chain up to the root level.</span></span>

#### <a name="request"></a><span data-ttu-id="18aa6-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18aa6-156">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_transitive_managers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me?$expand=manager($levels=max;$select=id,displayName)&$select=id,displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="18aa6-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="18aa6-157">Response</span></span>

<span data-ttu-id="18aa6-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="18aa6-158">The following is an example of the response.</span></span> <span data-ttu-id="18aa6-159">Os gerentes transitivos são exibidos hierarquicamente.</span><span class="sxs-lookup"><span data-stu-id="18aa6-159">Transitive managers are displayed hierarchically.</span></span>

><span data-ttu-id="18aa6-160">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="18aa6-160">**Note**: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "<user1-id>",
    "displayName": "Individual Contributor",
    "manager": {
        "id": "<manager1-id>",
        "displayName": "Manager 1",
        "manager": {
            "id": "<manager2-id>",
            "displayName": "Manager 2",
            "manager": {
                "id": "<manager3-id>",
                "displayName": "Manager 3"
            }
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
