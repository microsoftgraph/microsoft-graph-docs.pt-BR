---
title: Listar contactFolders
description: Obter a coleção de pastas de contatos na pasta Contatos padrão do usuário conectado.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 558c688737992d3fc9117e505399da7610331a3b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276451"
---
# <a name="list-contactfolders"></a><span data-ttu-id="4ab0d-103">Listar contactFolders</span><span class="sxs-lookup"><span data-stu-id="4ab0d-103">List contactFolders</span></span>

<span data-ttu-id="4ab0d-104">Obter a coleção de pastas de contatos na pasta Contatos padrão do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="4ab0d-104">Get the contact folder collection in the default Contacts folder of the signed-in user.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ab0d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ab0d-105">Permissions</span></span>
<span data-ttu-id="4ab0d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ab0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ab0d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ab0d-108">Permission type</span></span>      | <span data-ttu-id="4ab0d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ab0d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ab0d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ab0d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4ab0d-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ab0d-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4ab0d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ab0d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ab0d-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ab0d-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4ab0d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ab0d-114">Application</span></span> | <span data-ttu-id="4ab0d-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ab0d-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ab0d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ab0d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4ab0d-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4ab0d-117">Optional query parameters</span></span>
<span data-ttu-id="4ab0d-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4ab0d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4ab0d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ab0d-119">Request headers</span></span>
| <span data-ttu-id="4ab0d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ab0d-120">Header</span></span>       | <span data-ttu-id="4ab0d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4ab0d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4ab0d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ab0d-122">Authorization</span></span>  | <span data-ttu-id="4ab0d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ab0d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4ab0d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4ab0d-125">Content-Type</span></span>   | <span data-ttu-id="4ab0d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ab0d-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4ab0d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ab0d-127">Request body</span></span>
<span data-ttu-id="4ab0d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ab0d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ab0d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ab0d-129">Response</span></span>

<span data-ttu-id="4ab0d-130">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ab0d-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4ab0d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ab0d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ab0d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ab0d-132">Request</span></span>
<span data-ttu-id="4ab0d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ab0d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders
```
##### <a name="response"></a><span data-ttu-id="4ab0d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ab0d-134">Response</span></span>
<span data-ttu-id="4ab0d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ab0d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4ab0d-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="4ab0d-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4ab0d-139">C#</span><span class="sxs-lookup"><span data-stu-id="4ab0d-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_contactfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4ab0d-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="4ab0d-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_contactfolders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4ab0d-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4ab0d-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_contactfolders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list-contactfolders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-list-contactfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list-contactfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
