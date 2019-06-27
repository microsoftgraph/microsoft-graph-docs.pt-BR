---
title: Obter directoryObject
description: Recupere as propriedades e os relacionamentos do objeto directoryObject.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0ecec08b7c27008596ddc973326e98658f519b73
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273651"
---
# <a name="get-directoryobject"></a><span data-ttu-id="995d2-103">Obter directoryObject</span><span class="sxs-lookup"><span data-stu-id="995d2-103">Get directoryObject</span></span>

<span data-ttu-id="995d2-104">Recupere as propriedades e os relacionamentos do objeto directoryObject.</span><span class="sxs-lookup"><span data-stu-id="995d2-104">Retrieve the properties and relationships of directoryObject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="995d2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="995d2-105">Permissions</span></span>
<span data-ttu-id="995d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="995d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="995d2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="995d2-108">Permission type</span></span>      | <span data-ttu-id="995d2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="995d2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="995d2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="995d2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="995d2-111">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="995d2-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="995d2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="995d2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="995d2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="995d2-113">Not supported.</span></span>    |
|<span data-ttu-id="995d2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="995d2-114">Application</span></span> | <span data-ttu-id="995d2-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="995d2-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="995d2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="995d2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="995d2-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="995d2-117">Optional query parameters</span></span>
<span data-ttu-id="995d2-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="995d2-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="995d2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="995d2-119">Request headers</span></span>
| <span data-ttu-id="995d2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="995d2-120">Name</span></span>       | <span data-ttu-id="995d2-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="995d2-121">Type</span></span> | <span data-ttu-id="995d2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="995d2-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="995d2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="995d2-123">Authorization</span></span>  | <span data-ttu-id="995d2-124">string</span><span class="sxs-lookup"><span data-stu-id="995d2-124">string</span></span>  | <span data-ttu-id="995d2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="995d2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="995d2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="995d2-127">Request body</span></span>
<span data-ttu-id="995d2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="995d2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="995d2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="995d2-129">Response</span></span>

<span data-ttu-id="995d2-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="995d2-130">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="995d2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="995d2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="995d2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="995d2-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="995d2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="995d2-133">Response</span></span>
<span data-ttu-id="995d2-p103">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="995d2-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="995d2-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="995d2-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="995d2-137">C#</span><span class="sxs-lookup"><span data-stu-id="995d2-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directoryobject-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="995d2-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="995d2-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directoryobject-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="995d2-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="995d2-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_directoryobject-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryobject-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directoryobject-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryobject-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
