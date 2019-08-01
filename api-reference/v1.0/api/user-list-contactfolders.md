---
title: Listar contactFolders
description: Obter a coleção de pastas de contatos na pasta Contatos padrão do usuário conectado.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7975f15a0568778de4748b0c218135738e135e95
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026968"
---
# <a name="list-contactfolders"></a><span data-ttu-id="f52ac-103">Listar contactFolders</span><span class="sxs-lookup"><span data-stu-id="f52ac-103">List contactFolders</span></span>

<span data-ttu-id="f52ac-104">Obter a coleção de pastas de contatos na pasta Contatos padrão do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="f52ac-104">Get the contact folder collection in the default Contacts folder of the signed-in user.</span></span>
## <a name="permissions"></a><span data-ttu-id="f52ac-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f52ac-105">Permissions</span></span>
<span data-ttu-id="f52ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f52ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f52ac-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f52ac-108">Permission type</span></span>      | <span data-ttu-id="f52ac-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f52ac-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f52ac-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f52ac-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f52ac-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f52ac-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="f52ac-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f52ac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f52ac-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f52ac-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="f52ac-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f52ac-114">Application</span></span> | <span data-ttu-id="f52ac-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f52ac-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f52ac-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f52ac-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f52ac-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f52ac-117">Optional query parameters</span></span>
<span data-ttu-id="f52ac-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f52ac-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f52ac-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f52ac-119">Request headers</span></span>
| <span data-ttu-id="f52ac-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f52ac-120">Header</span></span>       | <span data-ttu-id="f52ac-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f52ac-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f52ac-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f52ac-122">Authorization</span></span>  | <span data-ttu-id="f52ac-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f52ac-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f52ac-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f52ac-125">Content-Type</span></span>   | <span data-ttu-id="f52ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f52ac-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f52ac-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f52ac-127">Request body</span></span>
<span data-ttu-id="f52ac-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f52ac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f52ac-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f52ac-129">Response</span></span>

<span data-ttu-id="f52ac-130">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f52ac-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f52ac-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f52ac-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f52ac-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f52ac-132">Request</span></span>
<span data-ttu-id="f52ac-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f52ac-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f52ac-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f52ac-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f52ac-135">C#</span><span class="sxs-lookup"><span data-stu-id="f52ac-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f52ac-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="f52ac-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f52ac-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f52ac-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f52ac-138">Java</span><span class="sxs-lookup"><span data-stu-id="f52ac-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contactfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f52ac-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f52ac-139">Response</span></span>
<span data-ttu-id="f52ac-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f52ac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
