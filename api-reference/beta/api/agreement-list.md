---
title: Contratos de lista
description: Recupere uma lista de objetos do contrato.
localization_priority: Normal
ms.openlocfilehash: 3ae255a386986b5627aed99f29dca5bfb9934e30
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859917"
---
# <a name="list-agreements"></a><span data-ttu-id="2b545-103">Contratos de lista</span><span class="sxs-lookup"><span data-stu-id="2b545-103">List agreements</span></span>

> <span data-ttu-id="2b545-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2b545-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b545-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2b545-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b545-106">Recupere uma lista de objetos do [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="2b545-106">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b545-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="2b545-107">Permissions</span></span>
<span data-ttu-id="2b545-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b545-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b545-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b545-110">Permission type</span></span>                        | <span data-ttu-id="2b545-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b545-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b545-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b545-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2b545-113">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b545-113">Agreement.Read.All</span></span> |
|<span data-ttu-id="2b545-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b545-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b545-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b545-115">Not supported.</span></span> |
|<span data-ttu-id="2b545-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b545-116">Application</span></span>                            | <span data-ttu-id="2b545-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b545-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b545-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b545-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="2b545-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b545-119">Request headers</span></span>
| <span data-ttu-id="2b545-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2b545-120">Name</span></span>         | <span data-ttu-id="2b545-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b545-121">Type</span></span>        | <span data-ttu-id="2b545-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b545-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2b545-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b545-123">Authorization</span></span> | <span data-ttu-id="2b545-124">string</span><span class="sxs-lookup"><span data-stu-id="2b545-124">string</span></span> | <span data-ttu-id="2b545-125">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="2b545-125">Bearer \{token\}.</span></span> <span data-ttu-id="2b545-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b545-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b545-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b545-127">Request body</span></span>
<span data-ttu-id="2b545-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2b545-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2b545-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b545-129">Response</span></span>
<span data-ttu-id="2b545-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de [contrato](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b545-130">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b545-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b545-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b545-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b545-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```http
GET https://graph.microsoft.com/beta/agreements
```
##### <a name="response"></a><span data-ttu-id="2b545-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b545-133">Response</span></span>
><span data-ttu-id="2b545-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b545-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "value": [
    {
      "displayName": "displayName-value",
      "isViewingBeforeAcceptanceRequired": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
