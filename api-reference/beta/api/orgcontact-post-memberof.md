---
title: Criar memberOf
description: Use essa API para criar um novo memberOf.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b8919fb0a9513d2278d07a73cf1dc95327fdc983
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055509"
---
# <a name="create-memberof"></a><span data-ttu-id="27936-103">Criar memberOf</span><span class="sxs-lookup"><span data-stu-id="27936-103">Create memberOf</span></span>

<span data-ttu-id="27936-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27936-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27936-105">Use essa API para criar um novo memberOf.</span><span class="sxs-lookup"><span data-stu-id="27936-105">Use this API to create a new memberOf.</span></span>
## <a name="permissions"></a><span data-ttu-id="27936-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="27936-106">Permissions</span></span>
<span data-ttu-id="27936-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27936-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27936-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27936-109">Permission type</span></span>      | <span data-ttu-id="27936-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27936-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27936-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27936-111">Delegated (work or school account)</span></span> | <span data-ttu-id="27936-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27936-112">Not supported.</span></span>    |
|<span data-ttu-id="27936-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27936-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27936-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27936-114">Not supported.</span></span>    |
|<span data-ttu-id="27936-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27936-115">Application</span></span> | <span data-ttu-id="27936-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27936-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27936-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27936-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="27936-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27936-118">Request headers</span></span>
| <span data-ttu-id="27936-119">Nome</span><span class="sxs-lookup"><span data-stu-id="27936-119">Name</span></span>       | <span data-ttu-id="27936-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="27936-120">Type</span></span> | <span data-ttu-id="27936-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="27936-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="27936-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="27936-122">Authorization</span></span>  | <span data-ttu-id="27936-123">string</span><span class="sxs-lookup"><span data-stu-id="27936-123">string</span></span>  | <span data-ttu-id="27936-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27936-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27936-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27936-126">Request body</span></span>
<span data-ttu-id="27936-127">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="27936-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="27936-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="27936-128">Response</span></span>

<span data-ttu-id="27936-129">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27936-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27936-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27936-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27936-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27936-131">Request</span></span>
<span data-ttu-id="27936-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27936-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="27936-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="27936-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact_2"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/memberOf
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="27936-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27936-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-orgcontact-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="27936-135">C#</span><span class="sxs-lookup"><span data-stu-id="27936-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-orgcontact-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="27936-136">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="27936-136">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="27936-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="27936-137">Response</span></span>
<span data-ttu-id="27936-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27936-138">Here is an example of the response.</span></span> <span data-ttu-id="27936-139">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="27936-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


