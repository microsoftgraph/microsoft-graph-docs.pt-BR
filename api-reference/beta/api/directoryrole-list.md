---
title: Listar directoryRoles
description: Lista as funções de diretório ativadas no locatário.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 406c0646a3d9dbac3f31dd2bd075a40e1678a415
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046808"
---
# <a name="list-directoryroles"></a><span data-ttu-id="8102c-103">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="8102c-103">List directoryRoles</span></span>

<span data-ttu-id="8102c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8102c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8102c-105">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="8102c-105">List the directory roles that are activated in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="8102c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8102c-106">Permissions</span></span>
<span data-ttu-id="8102c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8102c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8102c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8102c-109">Permission type</span></span>      | <span data-ttu-id="8102c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8102c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8102c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8102c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8102c-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8102c-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8102c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8102c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8102c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8102c-114">Not supported.</span></span>    |
|<span data-ttu-id="8102c-115">Application</span><span class="sxs-lookup"><span data-stu-id="8102c-115">Application</span></span> | <span data-ttu-id="8102c-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8102c-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8102c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8102c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8102c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8102c-118">Optional query parameters</span></span>
<span data-ttu-id="8102c-119">Esse método **não** tem suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="8102c-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8102c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8102c-120">Request headers</span></span>
| <span data-ttu-id="8102c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8102c-121">Name</span></span>       | <span data-ttu-id="8102c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="8102c-122">Type</span></span> | <span data-ttu-id="8102c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8102c-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8102c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8102c-124">Authorization</span></span>  | <span data-ttu-id="8102c-125">string</span><span class="sxs-lookup"><span data-stu-id="8102c-125">string</span></span>  | <span data-ttu-id="8102c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8102c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8102c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8102c-128">Request body</span></span>
<span data-ttu-id="8102c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8102c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8102c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8102c-130">Response</span></span>

<span data-ttu-id="8102c-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8102c-131">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8102c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8102c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8102c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8102c-133">Request</span></span>
<span data-ttu-id="8102c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8102c-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8102c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8102c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles
```
# <a name="c"></a>[<span data-ttu-id="8102c-136">C#</span><span class="sxs-lookup"><span data-stu-id="8102c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8102c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8102c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8102c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8102c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8102c-139">Java</span><span class="sxs-lookup"><span data-stu-id="8102c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8102c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8102c-140">Response</span></span>
<span data-ttu-id="8102c-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8102c-141">Here is an example of the response.</span></span> <span data-ttu-id="8102c-142">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8102c-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 187

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
