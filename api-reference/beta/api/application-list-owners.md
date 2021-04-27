---
title: Listar proprietários
description: Recupere uma lista de proprietários (objetos directoryObject) para um aplicativo.
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 69f6fe740b0e0377f73eedbef681589da2ffe56e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048117"
---
# <a name="list-owners"></a><span data-ttu-id="d140d-103">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="d140d-103">List owners</span></span>

<span data-ttu-id="d140d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d140d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d140d-105">Recupere uma lista de proprietários de um aplicativo que são [objetos directoryObject.](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="d140d-105">Retrieve a list of owners for an application that are [directoryObject](../resources/directoryobject.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d140d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d140d-106">Permissions</span></span>
<span data-ttu-id="d140d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d140d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d140d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d140d-109">Permission type</span></span>      | <span data-ttu-id="d140d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d140d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d140d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d140d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d140d-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d140d-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d140d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d140d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d140d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d140d-114">Not supported.</span></span>    |
|<span data-ttu-id="d140d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d140d-115">Application</span></span> | <span data-ttu-id="d140d-116">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d140d-116">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="d140d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d140d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d140d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d140d-118">Optional query parameters</span></span>
<span data-ttu-id="d140d-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d140d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d140d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d140d-120">Request headers</span></span>
| <span data-ttu-id="d140d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d140d-121">Name</span></span>           | <span data-ttu-id="d140d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d140d-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="d140d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d140d-123">Authorization</span></span>  | <span data-ttu-id="d140d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d140d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d140d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d140d-126">Request body</span></span>
<span data-ttu-id="d140d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d140d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d140d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d140d-128">Response</span></span>

<span data-ttu-id="d140d-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d140d-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d140d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d140d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d140d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d140d-131">Request</span></span>
<span data-ttu-id="d140d-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d140d-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d140d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d140d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="d140d-134">C#</span><span class="sxs-lookup"><span data-stu-id="d140d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d140d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d140d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d140d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d140d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d140d-137">Java</span><span class="sxs-lookup"><span data-stu-id="d140d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d140d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d140d-138">Response</span></span>
<span data-ttu-id="d140d-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d140d-139">Here is an example of the response.</span></span> <span data-ttu-id="d140d-140">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d140d-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

