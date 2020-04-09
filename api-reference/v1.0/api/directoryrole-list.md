---
title: Listar directoryRoles
description: Lista as funções de diretório ativadas no locatário.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7f4a8f8838d77c9a947c304ee18898832c1d5428
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181396"
---
# <a name="list-directoryroles"></a><span data-ttu-id="fb46e-103">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="fb46e-103">List directoryRoles</span></span>

<span data-ttu-id="fb46e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb46e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fb46e-105">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="fb46e-105">List the directory roles that are activated in the tenant.</span></span>

<span data-ttu-id="fb46e-106">Essa operação retorna apenas as funções que foram ativadas.</span><span class="sxs-lookup"><span data-stu-id="fb46e-106">This operation only returns roles that have been activated.</span></span> <span data-ttu-id="fb46e-107">Uma função é ativada quando um administrador ativa a função usando a API [Activate directoryRole](directoryrole-post-directoryroles.md) .</span><span class="sxs-lookup"><span data-stu-id="fb46e-107">A role becomes activated when an admin activates the role using the [Activate directoryRole](directoryrole-post-directoryroles.md) API.</span></span> <span data-ttu-id="fb46e-108">Nem todas as funções internas são ativadas inicialmente.</span><span class="sxs-lookup"><span data-stu-id="fb46e-108">Not all built-in roles are initially activated.</span></span> 

<span data-ttu-id="fb46e-109">Ao atribuir uma função usando o portal do Azure, a etapa de ativação de função é feita implicitamente no nome do administrador.</span><span class="sxs-lookup"><span data-stu-id="fb46e-109">When assigning a role using the Azure portal, the role activation step is implicitly done on the admin's behalf.</span></span> <span data-ttu-id="fb46e-110">Para obter a lista completa de funções disponíveis no Azure AD, use [list directoryRoleTemplates](directoryroletemplate-list.md).</span><span class="sxs-lookup"><span data-stu-id="fb46e-110">To get the full list of roles that are available in Azure AD, use [List directoryRoleTemplates](directoryroletemplate-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fb46e-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb46e-111">Permissions</span></span>
<span data-ttu-id="fb46e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb46e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb46e-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb46e-114">Permission type</span></span>      | <span data-ttu-id="fb46e-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb46e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb46e-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb46e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="fb46e-117">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="fb46e-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fb46e-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb46e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb46e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb46e-119">Not supported.</span></span>    |
|<span data-ttu-id="fb46e-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb46e-120">Application</span></span> | <span data-ttu-id="fb46e-121">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fb46e-121">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb46e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb46e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fb46e-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fb46e-123">Optional query parameters</span></span>
<span data-ttu-id="fb46e-124">Esse método **não** tem suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="fb46e-124">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb46e-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb46e-125">Request headers</span></span>
| <span data-ttu-id="fb46e-126">Nome</span><span class="sxs-lookup"><span data-stu-id="fb46e-126">Name</span></span>       | <span data-ttu-id="fb46e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb46e-127">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="fb46e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb46e-128">Authorization</span></span>  | <span data-ttu-id="fb46e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb46e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb46e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb46e-131">Request body</span></span>
<span data-ttu-id="fb46e-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fb46e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb46e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb46e-133">Response</span></span>

<span data-ttu-id="fb46e-134">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb46e-134">If successful, this method returns a `200 OK` response code and a collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fb46e-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb46e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb46e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb46e-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fb46e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb46e-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles
```
# <a name="c"></a>[<span data-ttu-id="fb46e-138">C#</span><span class="sxs-lookup"><span data-stu-id="fb46e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb46e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb46e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb46e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb46e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb46e-141">Java</span><span class="sxs-lookup"><span data-stu-id="fb46e-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fb46e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb46e-142">Response</span></span>
<span data-ttu-id="fb46e-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb46e-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
