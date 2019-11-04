---
title: Listar directoryRoles
description: Lista as funções de diretório ativadas no locatário.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 02a99d98c0f37654e6594b816e7d3d0596301ec7
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939120"
---
# <a name="list-directoryroles"></a><span data-ttu-id="5806b-103">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="5806b-103">List directoryRoles</span></span>

<span data-ttu-id="5806b-104">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="5806b-104">List the directory roles that are activated in the tenant.</span></span>

<span data-ttu-id="5806b-105">Essa operação retorna apenas as funções que foram ativadas.</span><span class="sxs-lookup"><span data-stu-id="5806b-105">This operation only returns roles that have been activated.</span></span> <span data-ttu-id="5806b-106">Uma função é ativada quando um administrador ativa a função usando a API [Activate directoryRole](directoryrole-post-directoryroles.md) .</span><span class="sxs-lookup"><span data-stu-id="5806b-106">A role becomes activated when an admin activates the role using the [Activate directoryRole](directoryrole-post-directoryroles.md) API.</span></span> <span data-ttu-id="5806b-107">Nem todas as funções internas são ativadas inicialmente.</span><span class="sxs-lookup"><span data-stu-id="5806b-107">Not all built-in roles are initially activated.</span></span> 

<span data-ttu-id="5806b-108">Ao atribuir uma função usando o portal do Azure, a etapa de ativação de função é feita implicitamente no nome do administrador.</span><span class="sxs-lookup"><span data-stu-id="5806b-108">When assigning a role using the Azure portal, the role activation step is implicitly done on the admin's behalf.</span></span> <span data-ttu-id="5806b-109">Para obter a lista completa de funções disponíveis no Azure AD, use [list directoryRoleTemplates](directoryroletemplate-list.md).</span><span class="sxs-lookup"><span data-stu-id="5806b-109">To get the full list of roles that are available in Azure AD, use [List directoryRoleTemplates](directoryroletemplate-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5806b-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="5806b-110">Permissions</span></span>
<span data-ttu-id="5806b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5806b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5806b-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5806b-113">Permission type</span></span>      | <span data-ttu-id="5806b-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5806b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5806b-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5806b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="5806b-116">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="5806b-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5806b-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5806b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5806b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5806b-118">Not supported.</span></span>    |
|<span data-ttu-id="5806b-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5806b-119">Application</span></span> | <span data-ttu-id="5806b-120">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5806b-120">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5806b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5806b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5806b-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5806b-122">Optional query parameters</span></span>
<span data-ttu-id="5806b-123">Esse método **não** tem suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="5806b-123">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5806b-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5806b-124">Request headers</span></span>
| <span data-ttu-id="5806b-125">Nome</span><span class="sxs-lookup"><span data-stu-id="5806b-125">Name</span></span>       | <span data-ttu-id="5806b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="5806b-126">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="5806b-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="5806b-127">Authorization</span></span>  | <span data-ttu-id="5806b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5806b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5806b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5806b-130">Request body</span></span>
<span data-ttu-id="5806b-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5806b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5806b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5806b-132">Response</span></span>

<span data-ttu-id="5806b-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5806b-133">If successful, this method returns a `200 OK` response code and a collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5806b-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5806b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5806b-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5806b-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5806b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="5806b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5806b-137">C#</span><span class="sxs-lookup"><span data-stu-id="5806b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5806b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5806b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5806b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5806b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5806b-140">Java</span><span class="sxs-lookup"><span data-stu-id="5806b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5806b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5806b-141">Response</span></span>
<span data-ttu-id="5806b-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5806b-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
