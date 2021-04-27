---
title: Listar membros
description: Recupera uma lista dos usuários atribuídos à função de diretório.  Somente usuários podem ser atribuídos a uma função de diretório.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9425849444a31454e3a98fcd2fbabd8a04184938
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046822"
---
# <a name="list-members"></a><span data-ttu-id="33e12-104">Listar membros</span><span class="sxs-lookup"><span data-stu-id="33e12-104">List members</span></span>

<span data-ttu-id="33e12-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33e12-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33e12-p102">Recupera uma lista dos usuários atribuídos à função de diretório.  Somente usuários podem ser atribuídos a uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="33e12-p102">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="33e12-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="33e12-108">Permissions</span></span>
<span data-ttu-id="33e12-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33e12-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="33e12-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33e12-111">Permission type</span></span>      | <span data-ttu-id="33e12-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33e12-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33e12-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33e12-113">Delegated (work or school account)</span></span> | <span data-ttu-id="33e12-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="33e12-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="33e12-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33e12-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33e12-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33e12-116">Not supported.</span></span>    |
|<span data-ttu-id="33e12-117">Application</span><span class="sxs-lookup"><span data-stu-id="33e12-117">Application</span></span> | <span data-ttu-id="33e12-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33e12-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="33e12-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33e12-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="33e12-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="33e12-120">Optional query parameters</span></span>
<span data-ttu-id="33e12-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="33e12-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="33e12-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33e12-122">Request headers</span></span>
| <span data-ttu-id="33e12-123">Nome</span><span class="sxs-lookup"><span data-stu-id="33e12-123">Name</span></span>       | <span data-ttu-id="33e12-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="33e12-124">Type</span></span> | <span data-ttu-id="33e12-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="33e12-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="33e12-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="33e12-126">Authorization</span></span>  | <span data-ttu-id="33e12-127">string</span><span class="sxs-lookup"><span data-stu-id="33e12-127">string</span></span>  | <span data-ttu-id="33e12-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33e12-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33e12-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33e12-130">Request body</span></span>
<span data-ttu-id="33e12-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="33e12-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33e12-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="33e12-132">Response</span></span>

<span data-ttu-id="33e12-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33e12-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="33e12-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33e12-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33e12-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33e12-135">Request</span></span>
<span data-ttu-id="33e12-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33e12-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="33e12-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="33e12-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="33e12-138">C#</span><span class="sxs-lookup"><span data-stu-id="33e12-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33e12-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33e12-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33e12-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33e12-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33e12-141">Java</span><span class="sxs-lookup"><span data-stu-id="33e12-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="33e12-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="33e12-142">Response</span></span>
<span data-ttu-id="33e12-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33e12-143">Here is an example of the response.</span></span> <span data-ttu-id="33e12-144">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="33e12-144">Note: The response object shown here might be shortened for readability.</span></span>
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
