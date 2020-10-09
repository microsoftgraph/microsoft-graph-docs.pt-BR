---
title: Listar createdObjects
description: Obtenha uma lista de objetos de diretório criados pelo usuário.
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 1ed481ac71f157533293aba29f9b85e66ab92586
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402370"
---
# <a name="list-createdobjects"></a><span data-ttu-id="8364b-103">Listar createdObjects</span><span class="sxs-lookup"><span data-stu-id="8364b-103">List createdObjects</span></span>

<span data-ttu-id="8364b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8364b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8364b-105">Obtenha uma lista de objetos de diretório criados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="8364b-105">Get a list of directory objects that were created by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="8364b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8364b-106">Permissions</span></span>
<span data-ttu-id="8364b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8364b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8364b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8364b-109">Permission type</span></span>      | <span data-ttu-id="8364b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8364b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8364b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8364b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8364b-112">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8364b-112">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8364b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8364b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8364b-114">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8364b-114">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="8364b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8364b-115">Application</span></span> | <span data-ttu-id="8364b-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8364b-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="8364b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8364b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8364b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8364b-118">Optional query parameters</span></span>
<span data-ttu-id="8364b-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8364b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8364b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8364b-120">Request headers</span></span>
| <span data-ttu-id="8364b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8364b-121">Header</span></span>       | <span data-ttu-id="8364b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8364b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8364b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8364b-123">Authorization</span></span>  | <span data-ttu-id="8364b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8364b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8364b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8364b-126">Content-Type</span></span>  | <span data-ttu-id="8364b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8364b-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8364b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8364b-128">Request body</span></span>
<span data-ttu-id="8364b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8364b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8364b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8364b-130">Response</span></span>

<span data-ttu-id="8364b-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8364b-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8364b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8364b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8364b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8364b-133">Request</span></span>
<span data-ttu-id="8364b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8364b-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8364b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8364b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/createdObjects
```
# <a name="c"></a>[<span data-ttu-id="8364b-136">C#</span><span class="sxs-lookup"><span data-stu-id="8364b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-createdobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8364b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8364b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-createdobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8364b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8364b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-createdobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8364b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8364b-139">Response</span></span>
<span data-ttu-id="8364b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8364b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->