---
title: Listar directoryRoles
description: Lista as funções de diretório ativadas no locatário.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: f327c47c36bf2b26fe50eeb4b2d511f157c8006d
ms.sourcegitcommit: 9eeb056f311044aaa40654cdb3ae5ae61f1c4d04
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/09/2021
ms.locfileid: "52854205"
---
# <a name="list-directoryroles"></a><span data-ttu-id="3d745-103">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="3d745-103">List directoryRoles</span></span>

<span data-ttu-id="3d745-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d745-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d745-105">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="3d745-105">List the directory roles that are activated in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="3d745-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d745-106">Permissions</span></span>
<span data-ttu-id="3d745-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d745-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d745-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d745-109">Permission type</span></span>      | <span data-ttu-id="3d745-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d745-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d745-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d745-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3d745-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3d745-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3d745-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d745-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d745-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d745-114">Not supported.</span></span>    |
|<span data-ttu-id="3d745-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d745-115">Application</span></span> | <span data-ttu-id="3d745-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d745-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d745-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d745-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3d745-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3d745-118">Optional query parameters</span></span>
<span data-ttu-id="3d745-119">Esse método **não** tem suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="3d745-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d745-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d745-120">Request headers</span></span>
| <span data-ttu-id="3d745-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3d745-121">Name</span></span>       | <span data-ttu-id="3d745-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d745-122">Type</span></span> | <span data-ttu-id="3d745-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d745-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3d745-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d745-124">Authorization</span></span>  | <span data-ttu-id="3d745-125">string</span><span class="sxs-lookup"><span data-stu-id="3d745-125">string</span></span>  | <span data-ttu-id="3d745-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d745-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d745-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d745-128">Request body</span></span>
<span data-ttu-id="3d745-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3d745-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d745-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d745-130">Response</span></span>

<span data-ttu-id="3d745-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d745-131">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3d745-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d745-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d745-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d745-133">Request</span></span>
<span data-ttu-id="3d745-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d745-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3d745-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d745-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles
```
# <a name="c"></a>[<span data-ttu-id="3d745-136">C#</span><span class="sxs-lookup"><span data-stu-id="3d745-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d745-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d745-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d745-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d745-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3d745-139">Java</span><span class="sxs-lookup"><span data-stu-id="3d745-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3d745-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d745-140">Response</span></span>
<span data-ttu-id="3d745-p103">Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="3d745-p103">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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
