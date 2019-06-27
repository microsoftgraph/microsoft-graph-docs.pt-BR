---
title: Obter domínio
description: Recupere as propriedades e os relacionamentos do objeto Domain.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fa145397ccec8da6444cf0be6c88215e96afe3da
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260470"
---
# <a name="get-domain"></a><span data-ttu-id="c2b00-103">Obter domínio</span><span class="sxs-lookup"><span data-stu-id="c2b00-103">Get domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2b00-104">Recupere as propriedades e os relacionamentos do objeto Domain.</span><span class="sxs-lookup"><span data-stu-id="c2b00-104">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2b00-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2b00-105">Permissions</span></span>

<span data-ttu-id="c2b00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2b00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c2b00-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2b00-108">Permission type</span></span>      | <span data-ttu-id="c2b00-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2b00-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2b00-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2b00-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c2b00-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2b00-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="c2b00-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2b00-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2b00-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2b00-113">Not supported.</span></span>    |
|<span data-ttu-id="c2b00-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2b00-114">Application</span></span> | <span data-ttu-id="c2b00-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2b00-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2b00-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2b00-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="c2b00-117">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="c2b00-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="c2b00-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c2b00-118">Optional query parameters</span></span>

<span data-ttu-id="c2b00-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c2b00-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2b00-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2b00-120">Request headers</span></span>

| <span data-ttu-id="c2b00-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c2b00-121">Name</span></span>      |<span data-ttu-id="c2b00-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2b00-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c2b00-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2b00-123">Authorization</span></span>  | <span data-ttu-id="c2b00-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2b00-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c2b00-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2b00-126">Content-Type</span></span>  | <span data-ttu-id="c2b00-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c2b00-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2b00-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2b00-128">Request body</span></span>
<span data-ttu-id="c2b00-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2b00-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2b00-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2b00-130">Response</span></span>

<span data-ttu-id="c2b00-131">Se bem-sucedido, este método retorna o `200 OK` código de resposta e o objeto [Domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2b00-131">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2b00-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2b00-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2b00-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2b00-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="c2b00-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2b00-134">Response</span></span>
<span data-ttu-id="c2b00-p103">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2b00-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c2b00-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c2b00-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c2b00-138">C#</span><span class="sxs-lookup"><span data-stu-id="c2b00-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_domain-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2b00-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2b00-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_domain-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c2b00-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c2b00-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_domain-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/domain-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
