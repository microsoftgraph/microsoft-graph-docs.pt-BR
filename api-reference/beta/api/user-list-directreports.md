---
title: Listar directReports
description: Obtenha relatórios diretos do usuário. Retorna os usuários e contatos para quem este usuário está atribuído como gerente.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 143c92f1b30eef96569b8fa3b9d669d90b3ebd2d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270179"
---
# <a name="list-directreports"></a><span data-ttu-id="0b34b-104">Listar directReports</span><span class="sxs-lookup"><span data-stu-id="0b34b-104">List directReports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b34b-105">Obtenha relatórios diretos do usuário.</span><span class="sxs-lookup"><span data-stu-id="0b34b-105">Get user's direct reports.</span></span> <span data-ttu-id="0b34b-106">Retorna os usuários e contatos para quem este usuário está atribuído como gerente.</span><span class="sxs-lookup"><span data-stu-id="0b34b-106">Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="0b34b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b34b-107">Permissions</span></span>
<span data-ttu-id="0b34b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b34b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b34b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b34b-110">Permission type</span></span>      | <span data-ttu-id="0b34b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b34b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b34b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b34b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0b34b-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0b34b-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0b34b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b34b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b34b-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b34b-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="0b34b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b34b-116">Application</span></span> | <span data-ttu-id="0b34b-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b34b-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b34b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b34b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/directReports
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0b34b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0b34b-119">Optional query parameters</span></span>
<span data-ttu-id="0b34b-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0b34b-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0b34b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b34b-121">Request headers</span></span>
| <span data-ttu-id="0b34b-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b34b-122">Header</span></span>       | <span data-ttu-id="0b34b-123">Valor</span><span class="sxs-lookup"><span data-stu-id="0b34b-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="0b34b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b34b-124">Authorization</span></span>  | <span data-ttu-id="0b34b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b34b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0b34b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b34b-127">Content-Type</span></span>   | <span data-ttu-id="0b34b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0b34b-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0b34b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b34b-129">Request body</span></span>
<span data-ttu-id="0b34b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0b34b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b34b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b34b-131">Response</span></span>

<span data-ttu-id="0b34b-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b34b-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0b34b-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b34b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b34b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b34b-134">Request</span></span>
<span data-ttu-id="0b34b-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b34b-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/beta/me/directReports
```
##### <a name="response"></a><span data-ttu-id="0b34b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b34b-136">Response</span></span>
<span data-ttu-id="0b34b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b34b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0b34b-140">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="0b34b-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0b34b-141">C#</span><span class="sxs-lookup"><span data-stu-id="0b34b-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directreports-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b34b-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="0b34b-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directreports-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0b34b-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0b34b-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_directreports-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-directreports.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-list-directreports.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-directreports.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
