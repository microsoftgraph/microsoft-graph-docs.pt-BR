---
title: Listar proprietários
description: Recupere uma lista de proprietários (objetos directoryobject) para um aplicativo.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f91a7926c5635a1f66622b6f3dd7e375d42c3f7d
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37999106"
---
# <a name="list-owners"></a><span data-ttu-id="0fd92-103">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="0fd92-103">List owners</span></span>

<span data-ttu-id="0fd92-104">Recupere uma lista de proprietários para um aplicativo que são objetos [directoryobject](../resources/directoryobject.md) .</span><span class="sxs-lookup"><span data-stu-id="0fd92-104">Retrieve a list of owners for an application that are [directoryObject](../resources/directoryobject.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fd92-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0fd92-105">Permissions</span></span>
<span data-ttu-id="0fd92-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fd92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fd92-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fd92-108">Permission type</span></span>      | <span data-ttu-id="0fd92-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0fd92-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fd92-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fd92-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0fd92-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0fd92-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0fd92-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fd92-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fd92-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fd92-113">Not supported.</span></span>    |
|<span data-ttu-id="0fd92-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fd92-114">Application</span></span> | <span data-ttu-id="0fd92-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fd92-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fd92-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fd92-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0fd92-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0fd92-117">Optional query parameters</span></span>
<span data-ttu-id="0fd92-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0fd92-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0fd92-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fd92-119">Request headers</span></span>
| <span data-ttu-id="0fd92-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0fd92-120">Name</span></span>       | <span data-ttu-id="0fd92-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0fd92-121">Type</span></span> | <span data-ttu-id="0fd92-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fd92-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0fd92-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fd92-123">Authorization</span></span>  | <span data-ttu-id="0fd92-124">string</span><span class="sxs-lookup"><span data-stu-id="0fd92-124">string</span></span>  | <span data-ttu-id="0fd92-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fd92-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0fd92-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fd92-127">Request body</span></span>
<span data-ttu-id="0fd92-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0fd92-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fd92-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fd92-129">Response</span></span>

<span data-ttu-id="0fd92-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fd92-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0fd92-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fd92-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0fd92-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fd92-132">Request</span></span>
<span data-ttu-id="0fd92-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fd92-133">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0fd92-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fd92-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}/owners
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0fd92-135">C#</span><span class="sxs-lookup"><span data-stu-id="0fd92-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0fd92-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fd92-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0fd92-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fd92-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0fd92-138">Java</span><span class="sxs-lookup"><span data-stu-id="0fd92-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0fd92-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fd92-139">Response</span></span>
<span data-ttu-id="0fd92-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fd92-140">Here is an example of the response.</span></span> 

><span data-ttu-id="0fd92-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0fd92-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
