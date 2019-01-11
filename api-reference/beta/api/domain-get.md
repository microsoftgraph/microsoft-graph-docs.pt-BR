---
title: Obter domínio
description: Recupere as propriedades e os relacionamentos do objeto domain.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 49458b87f86bc5a7dbf4d7d3c196736050b2d6aa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813570"
---
# <a name="get-domain"></a><span data-ttu-id="10695-103">Obter domínio</span><span class="sxs-lookup"><span data-stu-id="10695-103">Get domain</span></span>

> <span data-ttu-id="10695-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="10695-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10695-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="10695-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="10695-106">Recupere as propriedades e os relacionamentos do objeto domain.</span><span class="sxs-lookup"><span data-stu-id="10695-106">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="10695-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="10695-107">Permissions</span></span>

<span data-ttu-id="10695-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10695-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="10695-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10695-110">Permission type</span></span>      | <span data-ttu-id="10695-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10695-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10695-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10695-112">Delegated (work or school account)</span></span> | <span data-ttu-id="10695-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="10695-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="10695-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10695-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10695-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10695-115">Not supported.</span></span>    |
|<span data-ttu-id="10695-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10695-116">Application</span></span> | <span data-ttu-id="10695-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10695-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="10695-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10695-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="10695-119">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="10695-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="10695-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="10695-120">Optional query parameters</span></span>

<span data-ttu-id="10695-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="10695-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10695-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10695-122">Request headers</span></span>

| <span data-ttu-id="10695-123">Nome</span><span class="sxs-lookup"><span data-stu-id="10695-123">Name</span></span>      |<span data-ttu-id="10695-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="10695-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="10695-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="10695-125">Authorization</span></span>  | <span data-ttu-id="10695-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10695-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="10695-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10695-128">Content-Type</span></span>  | <span data-ttu-id="10695-129">application/json</span><span class="sxs-lookup"><span data-stu-id="10695-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="10695-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10695-130">Request body</span></span>
<span data-ttu-id="10695-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="10695-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10695-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="10695-132">Response</span></span>

<span data-ttu-id="10695-133">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10695-133">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="10695-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10695-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10695-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10695-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="10695-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="10695-136">Response</span></span>
<span data-ttu-id="10695-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10695-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
