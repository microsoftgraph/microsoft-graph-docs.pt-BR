---
title: Obter directoryObject
description: Recupere as propriedades e os relacionamentos do objeto directoryobject.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 29fee99420ea038e5d0e7b096a2f3adbf7e5eea5
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43180948"
---
# <a name="get-directoryobject"></a><span data-ttu-id="2bdbf-103">Obter directoryObject</span><span class="sxs-lookup"><span data-stu-id="2bdbf-103">Get directoryObject</span></span>

<span data-ttu-id="2bdbf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bdbf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bdbf-105">Recupere as propriedades e os relacionamentos do objeto directoryobject.</span><span class="sxs-lookup"><span data-stu-id="2bdbf-105">Retrieve the properties and relationships of directoryobject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2bdbf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2bdbf-106">Permissions</span></span>
<span data-ttu-id="2bdbf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bdbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bdbf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2bdbf-109">Permission type</span></span>      | <span data-ttu-id="2bdbf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2bdbf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2bdbf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2bdbf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2bdbf-112">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2bdbf-112">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2bdbf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2bdbf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bdbf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2bdbf-114">Not supported.</span></span>    |
|<span data-ttu-id="2bdbf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2bdbf-115">Application</span></span> | <span data-ttu-id="2bdbf-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bdbf-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2bdbf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2bdbf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2bdbf-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2bdbf-118">Optional query parameters</span></span>
<span data-ttu-id="2bdbf-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2bdbf-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2bdbf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2bdbf-120">Request headers</span></span>
| <span data-ttu-id="2bdbf-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2bdbf-121">Name</span></span>       | <span data-ttu-id="2bdbf-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bdbf-122">Type</span></span> | <span data-ttu-id="2bdbf-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bdbf-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2bdbf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2bdbf-124">Authorization</span></span>  | <span data-ttu-id="2bdbf-125">string</span><span class="sxs-lookup"><span data-stu-id="2bdbf-125">string</span></span>  | <span data-ttu-id="2bdbf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bdbf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2bdbf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2bdbf-128">Request body</span></span>
<span data-ttu-id="2bdbf-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2bdbf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bdbf-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bdbf-130">Response</span></span>

<span data-ttu-id="2bdbf-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2bdbf-131">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2bdbf-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2bdbf-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2bdbf-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2bdbf-133">Request</span></span>
<span data-ttu-id="2bdbf-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2bdbf-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2bdbf-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2bdbf-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/{id}
```
# <a name="c"></a>[<span data-ttu-id="2bdbf-136">C#</span><span class="sxs-lookup"><span data-stu-id="2bdbf-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2bdbf-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2bdbf-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2bdbf-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2bdbf-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2bdbf-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bdbf-139">Response</span></span>
<span data-ttu-id="2bdbf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2bdbf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
