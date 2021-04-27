---
title: 'orgContact: listar directReports'
description: Obter os relatórios diretos do contato.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8e0af76933aee154f16e735d82a7d744444f54c3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055530"
---
# <a name="orgcontact-list-directreports"></a><span data-ttu-id="15359-103">orgContact: listar directReports</span><span class="sxs-lookup"><span data-stu-id="15359-103">orgContact: List directReports</span></span>

<span data-ttu-id="15359-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15359-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15359-105">Obter os relatórios diretos do contato.</span><span class="sxs-lookup"><span data-stu-id="15359-105">Get the contact's direct reports.</span></span>

## <a name="permissions"></a><span data-ttu-id="15359-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="15359-106">Permissions</span></span>
<span data-ttu-id="15359-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15359-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15359-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15359-109">Permission type</span></span>      | <span data-ttu-id="15359-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15359-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15359-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15359-111">Delegated (work or school account)</span></span> | <span data-ttu-id="15359-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="15359-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="15359-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15359-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15359-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15359-114">Not supported.</span></span>    |
|<span data-ttu-id="15359-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15359-115">Application</span></span> | <span data-ttu-id="15359-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15359-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="15359-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15359-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="15359-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="15359-118">Optional query parameters</span></span>
<span data-ttu-id="15359-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="15359-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15359-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15359-120">Request headers</span></span>
| <span data-ttu-id="15359-121">Nome</span><span class="sxs-lookup"><span data-stu-id="15359-121">Name</span></span>       | <span data-ttu-id="15359-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="15359-122">Type</span></span> | <span data-ttu-id="15359-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="15359-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="15359-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="15359-124">Authorization</span></span>  | <span data-ttu-id="15359-125">string</span><span class="sxs-lookup"><span data-stu-id="15359-125">string</span></span>  | <span data-ttu-id="15359-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15359-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15359-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15359-128">Request body</span></span>
<span data-ttu-id="15359-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="15359-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15359-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="15359-130">Response</span></span>

<span data-ttu-id="15359-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15359-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="15359-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15359-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15359-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15359-133">Request</span></span>
<span data-ttu-id="15359-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15359-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="15359-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="15359-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contacts_get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/{id}/directReports
```
# <a name="c"></a>[<span data-ttu-id="15359-136">C#</span><span class="sxs-lookup"><span data-stu-id="15359-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contacts-get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="15359-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15359-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contacts-get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15359-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15359-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contacts-get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="15359-139">Java</span><span class="sxs-lookup"><span data-stu-id="15359-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contacts-get-directreports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="15359-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="15359-140">Response</span></span>
<span data-ttu-id="15359-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15359-141">Here is an example of the response.</span></span> <span data-ttu-id="15359-142">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="15359-142">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
