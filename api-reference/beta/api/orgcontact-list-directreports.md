---
title: 'orgContact: list directReports'
description: Obter os subordinados diretos do contato.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6de88e05f415169a6ef0f3cc270cfc712e70efec
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596694"
---
# <a name="orgcontact-list-directreports"></a><span data-ttu-id="797a1-103">orgContact: list directReports</span><span class="sxs-lookup"><span data-stu-id="797a1-103">orgContact: List directReports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="797a1-104">Obter os subordinados diretos do contato.</span><span class="sxs-lookup"><span data-stu-id="797a1-104">Get the contact's direct reports.</span></span>

## <a name="permissions"></a><span data-ttu-id="797a1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="797a1-105">Permissions</span></span>
<span data-ttu-id="797a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="797a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="797a1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="797a1-108">Permission type</span></span>      | <span data-ttu-id="797a1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="797a1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="797a1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="797a1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="797a1-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="797a1-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="797a1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="797a1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="797a1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="797a1-113">Not supported.</span></span>    |
|<span data-ttu-id="797a1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="797a1-114">Application</span></span> | <span data-ttu-id="797a1-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="797a1-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="797a1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="797a1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="797a1-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="797a1-117">Optional query parameters</span></span>
<span data-ttu-id="797a1-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="797a1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="797a1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="797a1-119">Request headers</span></span>
| <span data-ttu-id="797a1-120">Nome</span><span class="sxs-lookup"><span data-stu-id="797a1-120">Name</span></span>       | <span data-ttu-id="797a1-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="797a1-121">Type</span></span> | <span data-ttu-id="797a1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="797a1-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="797a1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="797a1-123">Authorization</span></span>  | <span data-ttu-id="797a1-124">string</span><span class="sxs-lookup"><span data-stu-id="797a1-124">string</span></span>  | <span data-ttu-id="797a1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="797a1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="797a1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="797a1-127">Request body</span></span>
<span data-ttu-id="797a1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="797a1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="797a1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="797a1-129">Response</span></span>

<span data-ttu-id="797a1-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="797a1-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="797a1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="797a1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="797a1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="797a1-132">Request</span></span>
<span data-ttu-id="797a1-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="797a1-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/beta/contacts/{id}/directReports
```
##### <a name="response"></a><span data-ttu-id="797a1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="797a1-134">Response</span></span>
<span data-ttu-id="797a1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="797a1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="797a1-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="797a1-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="797a1-139">Basic</span><span class="sxs-lookup"><span data-stu-id="797a1-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directreports-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="797a1-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="797a1-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directreports-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/orgcontact-list-directreports.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/orgcontact-list-directreports.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
