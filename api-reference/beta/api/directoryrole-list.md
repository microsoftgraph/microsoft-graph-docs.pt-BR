---
title: Listar directoryRoles
description: Lista as funções de diretório ativadas no locatário.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bc9819e749ae9e251a6a4643483130440291407f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42434389"
---
# <a name="list-directoryroles"></a><span data-ttu-id="7dab6-103">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="7dab6-103">List directoryRoles</span></span>

<span data-ttu-id="7dab6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7dab6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dab6-105">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="7dab6-105">List the directory roles that are activated in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="7dab6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7dab6-106">Permissions</span></span>
<span data-ttu-id="7dab6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dab6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dab6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7dab6-109">Permission type</span></span>      | <span data-ttu-id="7dab6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7dab6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7dab6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7dab6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7dab6-112">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="7dab6-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7dab6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7dab6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dab6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7dab6-114">Not supported.</span></span>    |
|<span data-ttu-id="7dab6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7dab6-115">Application</span></span> | <span data-ttu-id="7dab6-116">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7dab6-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dab6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7dab6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7dab6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7dab6-118">Optional query parameters</span></span>
<span data-ttu-id="7dab6-119">Esse método **não** tem suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="7dab6-119">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7dab6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7dab6-120">Request headers</span></span>
| <span data-ttu-id="7dab6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7dab6-121">Name</span></span>       | <span data-ttu-id="7dab6-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="7dab6-122">Type</span></span> | <span data-ttu-id="7dab6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dab6-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7dab6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7dab6-124">Authorization</span></span>  | <span data-ttu-id="7dab6-125">string</span><span class="sxs-lookup"><span data-stu-id="7dab6-125">string</span></span>  | <span data-ttu-id="7dab6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7dab6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7dab6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7dab6-128">Request body</span></span>
<span data-ttu-id="7dab6-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7dab6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7dab6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dab6-130">Response</span></span>

<span data-ttu-id="7dab6-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7dab6-131">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7dab6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7dab6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7dab6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7dab6-133">Request</span></span>
<span data-ttu-id="7dab6-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7dab6-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7dab6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dab6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles
```
# <a name="c"></a>[<span data-ttu-id="7dab6-136">C#</span><span class="sxs-lookup"><span data-stu-id="7dab6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7dab6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dab6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7dab6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dab6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7dab6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dab6-139">Response</span></span>
<span data-ttu-id="7dab6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7dab6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
