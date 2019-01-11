---
title: Obter domínio
description: Recupere as propriedades e os relacionamentos do objeto domain.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 4d49fe39f9e953b6e0bcdb4504a4f2296d5d4ff9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817217"
---
# <a name="get-domain"></a><span data-ttu-id="0e770-103">Obter domínio</span><span class="sxs-lookup"><span data-stu-id="0e770-103">Get domain</span></span>

<span data-ttu-id="0e770-104">Recupere as propriedades e os relacionamentos do objeto domain.</span><span class="sxs-lookup"><span data-stu-id="0e770-104">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e770-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e770-105">Permissions</span></span>

<span data-ttu-id="0e770-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e770-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0e770-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e770-108">Permission type</span></span>      | <span data-ttu-id="0e770-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e770-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e770-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e770-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0e770-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e770-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="0e770-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e770-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e770-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e770-113">Not supported.</span></span>    |
|<span data-ttu-id="0e770-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e770-114">Application</span></span> | <span data-ttu-id="0e770-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e770-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e770-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e770-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="0e770-117">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="0e770-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="0e770-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0e770-118">Optional query parameters</span></span>

<span data-ttu-id="0e770-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0e770-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e770-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e770-120">Request headers</span></span>

| <span data-ttu-id="0e770-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0e770-121">Name</span></span>      |<span data-ttu-id="0e770-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e770-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0e770-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e770-123">Authorization</span></span>  | <span data-ttu-id="0e770-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e770-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e770-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0e770-126">Content-Type</span></span>  | <span data-ttu-id="0e770-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0e770-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e770-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e770-128">Request body</span></span>
<span data-ttu-id="0e770-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0e770-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e770-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e770-130">Response</span></span>

<span data-ttu-id="0e770-131">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e770-131">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0e770-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e770-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e770-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e770-133">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="0e770-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e770-134">Response</span></span>
<span data-ttu-id="0e770-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e770-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
