---
title: Obter directoryObject
description: Recupere as propriedades e as relações do objeto directoryobject.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7303cefc9779f4080ddccd3fbe6b55ec6a4404c3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436908"
---
# <a name="get-directoryobject"></a><span data-ttu-id="f8186-103">Obter directoryObject</span><span class="sxs-lookup"><span data-stu-id="f8186-103">Get directoryObject</span></span>

<span data-ttu-id="f8186-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8186-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8186-105">Recupere as propriedades e as relações do objeto directoryobject.</span><span class="sxs-lookup"><span data-stu-id="f8186-105">Retrieve the properties and relationships of directoryobject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f8186-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f8186-106">Permissions</span></span>
<span data-ttu-id="f8186-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8186-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8186-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8186-109">Permission type</span></span>      | <span data-ttu-id="f8186-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8186-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8186-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8186-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f8186-112">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f8186-112">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f8186-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8186-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8186-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8186-114">Not supported.</span></span>    |
|<span data-ttu-id="f8186-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8186-115">Application</span></span> | <span data-ttu-id="f8186-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8186-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8186-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8186-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f8186-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f8186-118">Optional query parameters</span></span>
<span data-ttu-id="f8186-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f8186-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f8186-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8186-120">Request headers</span></span>
| <span data-ttu-id="f8186-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f8186-121">Name</span></span>       | <span data-ttu-id="f8186-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8186-122">Type</span></span> | <span data-ttu-id="f8186-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8186-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f8186-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8186-124">Authorization</span></span>  | <span data-ttu-id="f8186-125">string</span><span class="sxs-lookup"><span data-stu-id="f8186-125">string</span></span>  | <span data-ttu-id="f8186-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8186-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8186-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8186-128">Request body</span></span>
<span data-ttu-id="f8186-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8186-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8186-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8186-130">Response</span></span>

<span data-ttu-id="f8186-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8186-131">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f8186-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8186-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8186-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8186-133">Request</span></span>
<span data-ttu-id="f8186-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8186-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f8186-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8186-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/{id}
```
# <a name="c"></a>[<span data-ttu-id="f8186-136">C#</span><span class="sxs-lookup"><span data-stu-id="f8186-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8186-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8186-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8186-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8186-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f8186-139">Java</span><span class="sxs-lookup"><span data-stu-id="f8186-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryobject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f8186-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8186-140">Response</span></span>
<span data-ttu-id="f8186-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8186-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 22

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
