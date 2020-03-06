---
title: Listar memberOf
description: 'Obtenha todos os grupos e funções de diretório dos quais o usuário é um membro direto. '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 477bfbd87081ae28aa45cd7498a731b4efaa6939
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509063"
---
# <a name="list-memberof"></a><span data-ttu-id="f0823-103">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="f0823-103">List memberOf</span></span>

<span data-ttu-id="f0823-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0823-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f0823-105">Obtenha [grupos](../resources/group.md) e [funções de diretório](../resources/directoryrole.md) dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="f0823-105">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f0823-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0823-106">Permissions</span></span>
<span data-ttu-id="f0823-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0823-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0823-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0823-109">Permission type</span></span>      | <span data-ttu-id="f0823-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0823-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0823-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0823-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f0823-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f0823-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f0823-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0823-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0823-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0823-114">Not supported.</span></span>    |
|<span data-ttu-id="f0823-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0823-115">Application</span></span> | <span data-ttu-id="f0823-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0823-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="f0823-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0823-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f0823-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f0823-118">Optional query parameters</span></span>
<span data-ttu-id="f0823-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f0823-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="f0823-120">$filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="f0823-120">$filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="f0823-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0823-121">Request headers</span></span>
| <span data-ttu-id="f0823-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f0823-122">Header</span></span>       | <span data-ttu-id="f0823-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f0823-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f0823-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0823-124">Authorization</span></span>  | <span data-ttu-id="f0823-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0823-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f0823-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f0823-127">Accept</span></span>  | <span data-ttu-id="f0823-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f0823-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0823-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0823-129">Request body</span></span>
<span data-ttu-id="f0823-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f0823-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0823-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0823-131">Response</span></span>

<span data-ttu-id="f0823-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0823-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0823-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0823-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0823-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0823-134">Request</span></span>
<span data-ttu-id="f0823-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0823-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f0823-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0823-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/memberOf
```
# <a name="c"></a>[<span data-ttu-id="f0823-137">C#</span><span class="sxs-lookup"><span data-stu-id="f0823-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0823-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0823-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0823-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0823-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0823-140">Java</span><span class="sxs-lookup"><span data-stu-id="f0823-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f0823-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0823-141">Response</span></span>
<span data-ttu-id="f0823-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0823-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
