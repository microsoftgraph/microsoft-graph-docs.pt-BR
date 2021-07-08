---
title: Listar directoryRoles
description: Lista as funções de diretório ativadas no locatário.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b34011e1ed208405f40e4a5a5be6af20e1f217fe
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334420"
---
# <a name="list-directoryroles"></a><span data-ttu-id="eba61-103">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="eba61-103">List directoryRoles</span></span>

<span data-ttu-id="eba61-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eba61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eba61-105">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="eba61-105">List the directory roles that are activated in the tenant.</span></span>

<span data-ttu-id="eba61-106">Essa operação retorna apenas funções que foram ativadas.</span><span class="sxs-lookup"><span data-stu-id="eba61-106">This operation only returns roles that have been activated.</span></span> <span data-ttu-id="eba61-107">Uma função é ativada quando um administrador ativa a função usando a API [Activate directoryRole.](directoryrole-post-directoryroles.md)</span><span class="sxs-lookup"><span data-stu-id="eba61-107">A role becomes activated when an admin activates the role using the [Activate directoryRole](directoryrole-post-directoryroles.md) API.</span></span> <span data-ttu-id="eba61-108">Nem todas as funções in-iciais são ativadas inicialmente.</span><span class="sxs-lookup"><span data-stu-id="eba61-108">Not all built-in roles are initially activated.</span></span> 

<span data-ttu-id="eba61-109">Ao atribuir uma função usando o portal do Azure, a etapa de ativação de função é feita implicitamente em nome do administrador.</span><span class="sxs-lookup"><span data-stu-id="eba61-109">When assigning a role using the Azure portal, the role activation step is implicitly done on the admin's behalf.</span></span> <span data-ttu-id="eba61-110">Para obter a lista completa de funções disponíveis no Azure AD, use [List directoryRoleTemplates](directoryroletemplate-list.md).</span><span class="sxs-lookup"><span data-stu-id="eba61-110">To get the full list of roles that are available in Azure AD, use [List directoryRoleTemplates](directoryroletemplate-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eba61-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="eba61-111">Permissions</span></span>
<span data-ttu-id="eba61-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eba61-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eba61-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eba61-114">Permission type</span></span>      | <span data-ttu-id="eba61-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eba61-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eba61-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eba61-116">Delegated (work or school account)</span></span> | <span data-ttu-id="eba61-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eba61-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eba61-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eba61-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eba61-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eba61-119">Not supported.</span></span>    |
|<span data-ttu-id="eba61-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eba61-120">Application</span></span> | <span data-ttu-id="eba61-121">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eba61-121">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eba61-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eba61-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eba61-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eba61-123">Optional query parameters</span></span>
<span data-ttu-id="eba61-124">Esse método **não** tem suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="eba61-124">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="eba61-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eba61-125">Request headers</span></span>
| <span data-ttu-id="eba61-126">Nome</span><span class="sxs-lookup"><span data-stu-id="eba61-126">Name</span></span>       | <span data-ttu-id="eba61-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="eba61-127">Type</span></span> | <span data-ttu-id="eba61-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="eba61-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="eba61-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="eba61-129">Authorization</span></span>  | <span data-ttu-id="eba61-130">string</span><span class="sxs-lookup"><span data-stu-id="eba61-130">string</span></span>  | <span data-ttu-id="eba61-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eba61-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eba61-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eba61-133">Request body</span></span>
<span data-ttu-id="eba61-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eba61-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eba61-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="eba61-135">Response</span></span>

<span data-ttu-id="eba61-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eba61-136">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eba61-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eba61-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eba61-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eba61-138">Request</span></span>
<span data-ttu-id="eba61-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eba61-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eba61-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="eba61-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles
```
# <a name="c"></a>[<span data-ttu-id="eba61-141">C#</span><span class="sxs-lookup"><span data-stu-id="eba61-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eba61-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eba61-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eba61-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eba61-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eba61-144">Java</span><span class="sxs-lookup"><span data-stu-id="eba61-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="eba61-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="eba61-145">Response</span></span>
<span data-ttu-id="eba61-p105">Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="eba61-p105">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryRoles",
  "value": [
    {
      "id": "9ed3a0c4-53e1-498c-ab4d-2473476fde14",
      "deletedDateTime": null,
      "description": "Can manage all aspects of Azure AD and Microsoft services that use Azure AD identities.",
      "displayName": "Global Administrator",
      "roleTemplateId": "62e90394-69f5-4237-9190-012177145e10"
    },
    {
      "id": "f8e85ed8-f66f-4058-b170-3efae8b9c6e5",
      "deletedDateTime": null,
      "description": "Device Administrators",
      "displayName": "Azure AD Joined Device Local Administrator",
      "roleTemplateId": "9f06204d-73c1-4d4c-880a-6edb90606fd8"
    },
    {
      "id": "fe8f10bf-c9c2-47eb-95cb-c26cc85f1830",
      "deletedDateTime": null,
      "description": "Can read basic directory information. Commonly used to grant directory read access to applications and guests.",
      "displayName": "Directory Readers",
      "roleTemplateId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directoryRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
