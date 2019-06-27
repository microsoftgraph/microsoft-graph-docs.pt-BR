---
title: Listar childFolders
description: Obtenha uma coleção de pastas filho sob a pasta de contatos especificada.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 10130f215228c762289e485b29d7022a029780a0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261310"
---
# <a name="list-childfolders"></a><span data-ttu-id="56d83-103">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="56d83-103">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56d83-104">Obtenha uma coleção de pastas filho sob a pasta de contatos especificada.</span><span class="sxs-lookup"><span data-stu-id="56d83-104">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="56d83-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="56d83-105">Permissions</span></span>
<span data-ttu-id="56d83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56d83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56d83-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56d83-108">Permission type</span></span>      | <span data-ttu-id="56d83-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56d83-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56d83-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56d83-110">Delegated (work or school account)</span></span> | <span data-ttu-id="56d83-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56d83-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="56d83-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56d83-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56d83-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56d83-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="56d83-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56d83-114">Application</span></span> | <span data-ttu-id="56d83-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56d83-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="56d83-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56d83-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="56d83-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="56d83-117">Optional query parameters</span></span>
<span data-ttu-id="56d83-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="56d83-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="56d83-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56d83-119">Request headers</span></span>
| <span data-ttu-id="56d83-120">Nome</span><span class="sxs-lookup"><span data-stu-id="56d83-120">Name</span></span>       | <span data-ttu-id="56d83-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="56d83-121">Type</span></span> | <span data-ttu-id="56d83-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="56d83-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="56d83-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="56d83-123">Authorization</span></span>  | <span data-ttu-id="56d83-124">string</span><span class="sxs-lookup"><span data-stu-id="56d83-124">string</span></span>  | <span data-ttu-id="56d83-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56d83-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56d83-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56d83-127">Request body</span></span>
<span data-ttu-id="56d83-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="56d83-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56d83-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="56d83-129">Response</span></span>

<span data-ttu-id="56d83-130">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56d83-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="56d83-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56d83-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56d83-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56d83-132">Request</span></span>
<span data-ttu-id="56d83-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56d83-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="56d83-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="56d83-134">Response</span></span>
<span data-ttu-id="56d83-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56d83-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="56d83-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="56d83-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="56d83-139">C#</span><span class="sxs-lookup"><span data-stu-id="56d83-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_childfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56d83-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="56d83-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_childfolders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="56d83-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="56d83-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_childfolders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/contactfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/contactfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
