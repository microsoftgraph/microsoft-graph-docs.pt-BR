---
title: Obter domínio
description: Recupere as propriedades e os relacionamentos do objeto Domain.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ad4fe48857324098bd27ba79c751b407ed59de84
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656633"
---
# <a name="get-domain"></a><span data-ttu-id="f05ea-103">Obter domínio</span><span class="sxs-lookup"><span data-stu-id="f05ea-103">Get domain</span></span>

<span data-ttu-id="f05ea-104">Recupere as propriedades e os relacionamentos do objeto Domain.</span><span class="sxs-lookup"><span data-stu-id="f05ea-104">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f05ea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f05ea-105">Permissions</span></span>

<span data-ttu-id="f05ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f05ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f05ea-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f05ea-108">Permission type</span></span>      | <span data-ttu-id="f05ea-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f05ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f05ea-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f05ea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f05ea-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f05ea-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="f05ea-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f05ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f05ea-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f05ea-113">Not supported.</span></span>    |
|<span data-ttu-id="f05ea-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f05ea-114">Application</span></span> | <span data-ttu-id="f05ea-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f05ea-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f05ea-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f05ea-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="f05ea-117">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="f05ea-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="f05ea-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f05ea-118">Optional query parameters</span></span>

<span data-ttu-id="f05ea-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f05ea-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f05ea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f05ea-120">Request headers</span></span>

| <span data-ttu-id="f05ea-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f05ea-121">Name</span></span>      |<span data-ttu-id="f05ea-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f05ea-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f05ea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f05ea-123">Authorization</span></span>  | <span data-ttu-id="f05ea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f05ea-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f05ea-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f05ea-126">Content-Type</span></span>  | <span data-ttu-id="f05ea-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f05ea-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f05ea-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f05ea-128">Request body</span></span>
<span data-ttu-id="f05ea-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f05ea-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f05ea-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f05ea-130">Response</span></span>

<span data-ttu-id="f05ea-131">Se bem-sucedido, este método retorna o `200 OK` código de resposta e o objeto [Domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f05ea-131">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f05ea-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f05ea-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f05ea-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f05ea-133">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="f05ea-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f05ea-134">Response</span></span>
<span data-ttu-id="f05ea-p103">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f05ea-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f05ea-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f05ea-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f05ea-138">C#</span><span class="sxs-lookup"><span data-stu-id="f05ea-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_domain-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f05ea-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="f05ea-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_domain-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
