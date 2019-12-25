---
title: Listar memberOf
description: 'Obtenha todos os grupos e funções de diretório dos quais o usuário é um membro direto. '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 692f53b619d47a268cc987dbaffe9e4b45d3224d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864030"
---
# <a name="list-memberof"></a><span data-ttu-id="7e9d2-103">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="7e9d2-103">List memberOf</span></span>

<span data-ttu-id="7e9d2-104">Obtenha [grupos](../resources/group.md) e [funções de diretório](../resources/directoryrole.md) dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="7e9d2-104">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7e9d2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e9d2-105">Permissions</span></span>
<span data-ttu-id="7e9d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e9d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e9d2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e9d2-108">Permission type</span></span>      | <span data-ttu-id="7e9d2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e9d2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e9d2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e9d2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7e9d2-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7e9d2-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7e9d2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e9d2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e9d2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e9d2-113">Not supported.</span></span>    |
|<span data-ttu-id="7e9d2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e9d2-114">Application</span></span> | <span data-ttu-id="7e9d2-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e9d2-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="7e9d2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e9d2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7e9d2-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7e9d2-117">Optional query parameters</span></span>
<span data-ttu-id="7e9d2-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7e9d2-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="7e9d2-119">$filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="7e9d2-119">$filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="7e9d2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e9d2-120">Request headers</span></span>
| <span data-ttu-id="7e9d2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7e9d2-121">Header</span></span>       | <span data-ttu-id="7e9d2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7e9d2-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7e9d2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e9d2-123">Authorization</span></span>  | <span data-ttu-id="7e9d2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e9d2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7e9d2-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7e9d2-126">Accept</span></span>  | <span data-ttu-id="7e9d2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7e9d2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e9d2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e9d2-128">Request body</span></span>
<span data-ttu-id="7e9d2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e9d2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e9d2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e9d2-130">Response</span></span>

<span data-ttu-id="7e9d2-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e9d2-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7e9d2-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e9d2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e9d2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e9d2-133">Request</span></span>
<span data-ttu-id="7e9d2-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e9d2-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7e9d2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e9d2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e9d2-136">C#</span><span class="sxs-lookup"><span data-stu-id="7e9d2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e9d2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e9d2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e9d2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e9d2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7e9d2-139">Java</span><span class="sxs-lookup"><span data-stu-id="7e9d2-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7e9d2-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e9d2-140">Response</span></span>
<span data-ttu-id="7e9d2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e9d2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
