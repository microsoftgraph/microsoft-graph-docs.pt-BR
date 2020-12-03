---
title: Listar gerente
description: Obtenha o gerente do usuário. Retorna o usuário ou contato atribuído como gerente do usuário.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 1f04dc23b777906a3ee36bbcefea035e1e8d2422
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49524421"
---
# <a name="list-manager"></a><span data-ttu-id="36c40-104">Listar gerente</span><span class="sxs-lookup"><span data-stu-id="36c40-104">List manager</span></span>

<span data-ttu-id="36c40-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36c40-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36c40-106">Retorna o usuário ou o contato organizacional atribuído como gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="36c40-106">Returns the user or organizational contact assigned as the user's manager.</span></span> <span data-ttu-id="36c40-107">Opcionalmente, você pode expandir a cadeia do gerente para o nó raiz.</span><span class="sxs-lookup"><span data-stu-id="36c40-107">Optionally, you can expand the manager's chain up to the root node.</span></span>

## <a name="permissions"></a><span data-ttu-id="36c40-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="36c40-108">Permissions</span></span>

<span data-ttu-id="36c40-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36c40-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36c40-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36c40-111">Permission type</span></span>      | <span data-ttu-id="36c40-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36c40-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36c40-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36c40-113">Delegated (work or school account)</span></span> | <span data-ttu-id="36c40-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="36c40-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="36c40-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36c40-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36c40-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36c40-116">Not supported.</span></span>    |
|<span data-ttu-id="36c40-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36c40-117">Application</span></span> | <span data-ttu-id="36c40-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36c40-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="36c40-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36c40-119">HTTP request</span></span>

<span data-ttu-id="36c40-120">Obtenha o gerente:</span><span class="sxs-lookup"><span data-stu-id="36c40-120">Get the manager:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
<span data-ttu-id="36c40-121">Obtenha a cadeia de gerenciamento:</span><span class="sxs-lookup"><span data-stu-id="36c40-121">Get the management chain:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me?$expand=manager
GET /users?$expand=manager($levels=n)
GET /users/{id | userPrincipalName}/?$expand=manager($levels=n)
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36c40-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="36c40-122">Optional query parameters</span></span>

<span data-ttu-id="36c40-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="36c40-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>  

<span data-ttu-id="36c40-124">Se sua solicitação incluir o `$expand=manager($levels=n)` parâmetro para obter a cadeia do gerente, você também deverá incluir o seguinte:</span><span class="sxs-lookup"><span data-stu-id="36c40-124">If your request includes the `$expand=manager($levels=n)` parameter to get the manager's chain, you must also include the following:</span></span>

- <span data-ttu-id="36c40-125">`$count=true` parâmetro de cadeia de caracteres de consulta</span><span class="sxs-lookup"><span data-stu-id="36c40-125">`$count=true` query string parameter</span></span>
- <span data-ttu-id="36c40-126">`ConsistencyLevel=eventual` cabeçalho da solicitação</span><span class="sxs-lookup"><span data-stu-id="36c40-126">`ConsistencyLevel=eventual` request header</span></span>

><span data-ttu-id="36c40-127">**Observação:** o `n` valor de `$levels` pode ser `max` (para retornar todos os gerentes) ou um número entre 1 e 1000.</span><span class="sxs-lookup"><span data-stu-id="36c40-127">**Note:** the `n` value of `$levels` can be `max` (to return all managers) or a number between 1 and 1000.</span></span>  
> <span data-ttu-id="36c40-128">Quando o `$level` parâmetro não é especificado, somente o gerente imediato é retornado.</span><span class="sxs-lookup"><span data-stu-id="36c40-128">When the `$level` parameter is not specified, only the immediate manager is returned.</span></span>  
> <span data-ttu-id="36c40-129">Você pode especificar `$select` dentro `$expand` para selecionar as propriedades do gerente individual: `$expand=manager($levels=max;$select=id,displayName)`</span><span class="sxs-lookup"><span data-stu-id="36c40-129">You can specify `$select` inside `$expand` to select the individual manager's properties: `$expand=manager($levels=max;$select=id,displayName)`</span></span>

## <a name="request-headers"></a><span data-ttu-id="36c40-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36c40-130">Request headers</span></span>

| <span data-ttu-id="36c40-131">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="36c40-131">Header</span></span>       | <span data-ttu-id="36c40-132">Valor</span><span class="sxs-lookup"><span data-stu-id="36c40-132">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="36c40-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="36c40-133">Authorization</span></span>  | <span data-ttu-id="36c40-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36c40-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="36c40-136">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="36c40-136">ConsistencyLevel</span></span> | <span data-ttu-id="36c40-137">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="36c40-137">eventual.</span></span> <span data-ttu-id="36c40-138">Obrigatório quando a solicitação inclui o `$expand=manager($levels=max)` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="36c40-138">Required when the request includes the `$expand=manager($levels=max)` parameter.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36c40-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36c40-139">Request body</span></span>

<span data-ttu-id="36c40-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36c40-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36c40-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="36c40-141">Response</span></span>

<span data-ttu-id="36c40-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36c40-142">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36c40-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="36c40-143">Examples</span></span>

### <a name="example-1-get-manager"></a><span data-ttu-id="36c40-144">Exemplo 1: obter gerente</span><span class="sxs-lookup"><span data-stu-id="36c40-144">Example 1: Get manager</span></span>

<span data-ttu-id="36c40-145">O exemplo a seguir mostra uma solicitação para obter o gerente.</span><span class="sxs-lookup"><span data-stu-id="36c40-145">The following example shows a request to get the manager.</span></span>

#### <a name="request"></a><span data-ttu-id="36c40-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36c40-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="36c40-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="36c40-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```
# <a name="c"></a>[<span data-ttu-id="36c40-148">C#</span><span class="sxs-lookup"><span data-stu-id="36c40-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36c40-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36c40-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36c40-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36c40-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36c40-151">Java</span><span class="sxs-lookup"><span data-stu-id="36c40-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36c40-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="36c40-152">Response</span></span>

<span data-ttu-id="36c40-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="36c40-153">The following is an example of the response.</span></span>
><span data-ttu-id="36c40-154">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="36c40-154">**Note**: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-manager-chain-up-to-the-root-level"></a><span data-ttu-id="36c40-155">Exemplo 2: obter cadeia de gerentes até o nível raiz</span><span class="sxs-lookup"><span data-stu-id="36c40-155">Example 2: Get manager chain up to the root level</span></span>

<span data-ttu-id="36c40-156">O exemplo a seguir mostra uma solicitação para obter a cadeia de gerentes até o nível raiz.</span><span class="sxs-lookup"><span data-stu-id="36c40-156">The following example shows a request to get the manager chain up to the root level.</span></span>

#### <a name="request"></a><span data-ttu-id="36c40-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36c40-157">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_transitive_managers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me?$expand=manager($levels=max;$select=id,displayName)&$select=id,displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="36c40-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="36c40-158">Response</span></span>

<span data-ttu-id="36c40-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="36c40-159">The following is an example of the response.</span></span> <span data-ttu-id="36c40-160">Os gerenciadores transitivos são exibidos hierarquicamente.</span><span class="sxs-lookup"><span data-stu-id="36c40-160">Transitive managers are displayed hierarchically.</span></span>

><span data-ttu-id="36c40-161">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="36c40-161">**Note**: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
