---
title: Criar memberOf
description: Use esta API para criar um novo memberOf.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 187c8a866d4fe66721f7fde782cc976bab4d9a76
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44680666"
---
# <a name="create-memberof"></a><span data-ttu-id="e0a52-103">Criar memberOf</span><span class="sxs-lookup"><span data-stu-id="e0a52-103">Create memberOf</span></span>

<span data-ttu-id="e0a52-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0a52-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0a52-105">Use esta API para criar um novo memberOf.</span><span class="sxs-lookup"><span data-stu-id="e0a52-105">Use this API to create a new memberOf.</span></span>
## <a name="permissions"></a><span data-ttu-id="e0a52-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0a52-106">Permissions</span></span>
<span data-ttu-id="e0a52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0a52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0a52-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0a52-109">Permission type</span></span>      | <span data-ttu-id="e0a52-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0a52-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0a52-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0a52-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e0a52-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0a52-112">Not supported.</span></span>    |
|<span data-ttu-id="e0a52-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0a52-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0a52-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0a52-114">Not supported.</span></span>    |
|<span data-ttu-id="e0a52-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0a52-115">Application</span></span> | <span data-ttu-id="e0a52-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0a52-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0a52-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0a52-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="e0a52-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0a52-118">Request headers</span></span>
| <span data-ttu-id="e0a52-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e0a52-119">Name</span></span>       | <span data-ttu-id="e0a52-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0a52-120">Type</span></span> | <span data-ttu-id="e0a52-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0a52-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e0a52-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0a52-122">Authorization</span></span>  | <span data-ttu-id="e0a52-123">string</span><span class="sxs-lookup"><span data-stu-id="e0a52-123">string</span></span>  | <span data-ttu-id="e0a52-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0a52-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0a52-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0a52-126">Request body</span></span>
<span data-ttu-id="e0a52-127">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="e0a52-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e0a52-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0a52-128">Response</span></span>

<span data-ttu-id="e0a52-129">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0a52-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0a52-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0a52-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0a52-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0a52-131">Request</span></span>
<span data-ttu-id="e0a52-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0a52-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0a52-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0a52-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact"
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
# <a name="javascript"></a>[<span data-ttu-id="e0a52-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0a52-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="e0a52-135">C#</span><span class="sxs-lookup"><span data-stu-id="e0a52-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="e0a52-136">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="e0a52-136">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e0a52-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0a52-137">Response</span></span>
<span data-ttu-id="e0a52-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0a52-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
