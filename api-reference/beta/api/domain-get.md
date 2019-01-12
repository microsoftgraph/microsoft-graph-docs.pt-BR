---
title: Obter domínio
description: Recupere as propriedades e os relacionamentos do objeto domain.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8086887652412c88372871a5a8d6914372e3f83f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955384"
---
# <a name="get-domain"></a><span data-ttu-id="c852c-103">Obter domínio</span><span class="sxs-lookup"><span data-stu-id="c852c-103">Get domain</span></span>

> <span data-ttu-id="c852c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c852c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c852c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c852c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c852c-106">Recupere as propriedades e os relacionamentos do objeto domain.</span><span class="sxs-lookup"><span data-stu-id="c852c-106">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c852c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c852c-107">Permissions</span></span>

<span data-ttu-id="c852c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c852c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c852c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c852c-110">Permission type</span></span>      | <span data-ttu-id="c852c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c852c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c852c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c852c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c852c-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c852c-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="c852c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c852c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c852c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c852c-115">Not supported.</span></span>    |
|<span data-ttu-id="c852c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c852c-116">Application</span></span> | <span data-ttu-id="c852c-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c852c-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c852c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c852c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="c852c-119">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="c852c-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="c852c-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c852c-120">Optional query parameters</span></span>

<span data-ttu-id="c852c-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c852c-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c852c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c852c-122">Request headers</span></span>

| <span data-ttu-id="c852c-123">Nome</span><span class="sxs-lookup"><span data-stu-id="c852c-123">Name</span></span>      |<span data-ttu-id="c852c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c852c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c852c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c852c-125">Authorization</span></span>  | <span data-ttu-id="c852c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c852c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c852c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c852c-128">Content-Type</span></span>  | <span data-ttu-id="c852c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="c852c-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c852c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c852c-130">Request body</span></span>
<span data-ttu-id="c852c-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c852c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c852c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c852c-132">Response</span></span>

<span data-ttu-id="c852c-133">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c852c-133">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c852c-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c852c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c852c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c852c-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="c852c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c852c-136">Response</span></span>
<span data-ttu-id="c852c-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c852c-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
