---
title: Obter directoryRoleTemplate
description: Recupera as propriedades e os relacionamentos do objeto directoryroletemplate.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 16a7c578c019554c9ebc87833fe8ea1982810937
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272223"
---
# <a name="get-directoryroletemplate"></a><span data-ttu-id="41c11-103">Obter directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="41c11-103">Get directoryRoleTemplate</span></span>

<span data-ttu-id="41c11-104">Recupera as propriedades e os relacionamentos do objeto directoryroletemplate.</span><span class="sxs-lookup"><span data-stu-id="41c11-104">Retrieve the properties and relationships of a directoryroletemplate object.</span></span>
## <a name="permissions"></a><span data-ttu-id="41c11-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="41c11-105">Permissions</span></span>
<span data-ttu-id="41c11-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41c11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41c11-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41c11-108">Permission type</span></span>      | <span data-ttu-id="41c11-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41c11-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41c11-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41c11-110">Delegated (work or school account)</span></span> | <span data-ttu-id="41c11-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="41c11-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="41c11-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41c11-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41c11-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41c11-113">Not supported.</span></span>    |
|<span data-ttu-id="41c11-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41c11-114">Application</span></span> | <span data-ttu-id="41c11-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41c11-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41c11-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41c11-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="41c11-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="41c11-117">Optional query parameters</span></span>
<span data-ttu-id="41c11-118">Esse método **não** tem suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="41c11-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="41c11-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41c11-119">Request headers</span></span>
| <span data-ttu-id="41c11-120">Nome</span><span class="sxs-lookup"><span data-stu-id="41c11-120">Name</span></span>       | <span data-ttu-id="41c11-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="41c11-121">Type</span></span> | <span data-ttu-id="41c11-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="41c11-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="41c11-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="41c11-123">Authorization</span></span>  | <span data-ttu-id="41c11-124">string</span><span class="sxs-lookup"><span data-stu-id="41c11-124">string</span></span>  | <span data-ttu-id="41c11-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41c11-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41c11-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41c11-127">Request body</span></span>
<span data-ttu-id="41c11-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41c11-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41c11-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="41c11-129">Response</span></span>

<span data-ttu-id="41c11-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryRoleTemplate](../resources/directoryroletemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41c11-130">If successful, this method returns a `200 OK` response code and [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="41c11-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41c11-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41c11-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41c11-132">Request</span></span>
<span data-ttu-id="41c11-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41c11-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplate"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="41c11-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="41c11-134">Response</span></span>
<span data-ttu-id="41c11-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41c11-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "description": "description-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="41c11-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="41c11-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="41c11-139">C#</span><span class="sxs-lookup"><span data-stu-id="41c11-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directoryroletemplate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41c11-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="41c11-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directoryroletemplate-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="41c11-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="41c11-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_directoryroletemplate-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryRoleTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryroletemplate-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directoryroletemplate-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryroletemplate-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
