---
title: Obter domínio
description: Recupere as propriedades e os relacionamentos do objeto domain.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d280782f41f305672023c432364871de162b6647
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130813"
---
# <a name="get-domain"></a><span data-ttu-id="37ddc-103">Obter domínio</span><span class="sxs-lookup"><span data-stu-id="37ddc-103">Get domain</span></span>

<span data-ttu-id="37ddc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37ddc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37ddc-105">Recupere as propriedades e os relacionamentos do objeto domain.</span><span class="sxs-lookup"><span data-stu-id="37ddc-105">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="37ddc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37ddc-106">Permissions</span></span>

<span data-ttu-id="37ddc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37ddc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="37ddc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37ddc-109">Permission type</span></span>      | <span data-ttu-id="37ddc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37ddc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37ddc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37ddc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="37ddc-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="37ddc-112">Directory.Read.All</span></span>    |
|<span data-ttu-id="37ddc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37ddc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37ddc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37ddc-114">Not supported.</span></span>    |
|<span data-ttu-id="37ddc-115">Application</span><span class="sxs-lookup"><span data-stu-id="37ddc-115">Application</span></span> | <span data-ttu-id="37ddc-116">Domain.Read.All, Domain.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="37ddc-116">Domain.Read.All, Domain.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37ddc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37ddc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="37ddc-118">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="37ddc-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="37ddc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="37ddc-119">Optional query parameters</span></span>

<span data-ttu-id="37ddc-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="37ddc-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37ddc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37ddc-121">Request headers</span></span>

| <span data-ttu-id="37ddc-122">Nome</span><span class="sxs-lookup"><span data-stu-id="37ddc-122">Name</span></span>      |<span data-ttu-id="37ddc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="37ddc-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="37ddc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="37ddc-124">Authorization</span></span>  | <span data-ttu-id="37ddc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37ddc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="37ddc-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37ddc-127">Content-Type</span></span>  | <span data-ttu-id="37ddc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="37ddc-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="37ddc-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37ddc-129">Request body</span></span>
<span data-ttu-id="37ddc-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37ddc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37ddc-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="37ddc-131">Response</span></span>

<span data-ttu-id="37ddc-132">Se bem-sucedido, este método retorna um código de resposta e `200 OK` [um](../resources/domain.md) objeto de domínio no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37ddc-132">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="37ddc-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37ddc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37ddc-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37ddc-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="37ddc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="37ddc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/domains/contoso.com
```
# <a name="c"></a>[<span data-ttu-id="37ddc-136">C#</span><span class="sxs-lookup"><span data-stu-id="37ddc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37ddc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37ddc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37ddc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37ddc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37ddc-139">Java</span><span class="sxs-lookup"><span data-stu-id="37ddc-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="37ddc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="37ddc-140">Response</span></span>
<span data-ttu-id="37ddc-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37ddc-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
