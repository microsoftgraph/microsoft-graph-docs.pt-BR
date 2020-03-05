---
title: Listar membros
description: Recupera uma lista dos usuários atribuídos à função de diretório.  Somente usuários podem ser atribuídos a uma função de diretório.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7f68b3ace4e04d97d91dd2bd02ed66a44cc7fa6f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42434438"
---
# <a name="list-members"></a><span data-ttu-id="d9d99-104">Listar membros</span><span class="sxs-lookup"><span data-stu-id="d9d99-104">List members</span></span>

<span data-ttu-id="d9d99-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d9d99-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9d99-106">Recupera uma lista dos usuários atribuídos à função de diretório.</span><span class="sxs-lookup"><span data-stu-id="d9d99-106">Retrieve a list of the users that are assigned to the directory role.</span></span>  <span data-ttu-id="d9d99-107">Somente usuários podem ser atribuídos a uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="d9d99-107">Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="d9d99-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9d99-108">Permissions</span></span>
<span data-ttu-id="d9d99-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9d99-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d9d99-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9d99-111">Permission type</span></span>      | <span data-ttu-id="d9d99-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9d99-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9d99-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9d99-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d9d99-114">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="d9d99-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d9d99-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9d99-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9d99-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9d99-116">Not supported.</span></span>    |
|<span data-ttu-id="d9d99-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9d99-117">Application</span></span> | <span data-ttu-id="d9d99-118">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d9d99-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="d9d99-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9d99-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d9d99-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d9d99-120">Optional query parameters</span></span>
<span data-ttu-id="d9d99-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d9d99-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d9d99-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9d99-122">Request headers</span></span>
| <span data-ttu-id="d9d99-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d9d99-123">Name</span></span>       | <span data-ttu-id="d9d99-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9d99-124">Type</span></span> | <span data-ttu-id="d9d99-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9d99-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d9d99-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9d99-126">Authorization</span></span>  | <span data-ttu-id="d9d99-127">string</span><span class="sxs-lookup"><span data-stu-id="d9d99-127">string</span></span>  | <span data-ttu-id="d9d99-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9d99-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9d99-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9d99-130">Request body</span></span>
<span data-ttu-id="d9d99-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9d99-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9d99-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9d99-132">Response</span></span>

<span data-ttu-id="d9d99-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9d99-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d9d99-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9d99-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9d99-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9d99-135">Request</span></span>
<span data-ttu-id="d9d99-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9d99-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d9d99-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9d99-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="d9d99-138">C#</span><span class="sxs-lookup"><span data-stu-id="d9d99-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9d99-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9d99-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9d99-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9d99-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d9d99-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9d99-141">Response</span></span>
<span data-ttu-id="d9d99-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9d99-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
