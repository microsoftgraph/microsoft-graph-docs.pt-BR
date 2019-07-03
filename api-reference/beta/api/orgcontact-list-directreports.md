---
title: 'orgContact: list directReports'
description: Obter os subordinados diretos do contato.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c6d5de4540444b8f0e9f80670e1fc2753c67f7f7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445377"
---
# <a name="orgcontact-list-directreports"></a><span data-ttu-id="7a610-103">orgContact: list directReports</span><span class="sxs-lookup"><span data-stu-id="7a610-103">orgContact: List directReports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a610-104">Obter os subordinados diretos do contato.</span><span class="sxs-lookup"><span data-stu-id="7a610-104">Get the contact's direct reports.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a610-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a610-105">Permissions</span></span>
<span data-ttu-id="7a610-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a610-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a610-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a610-108">Permission type</span></span>      | <span data-ttu-id="7a610-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a610-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a610-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a610-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7a610-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7a610-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7a610-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a610-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a610-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a610-113">Not supported.</span></span>    |
|<span data-ttu-id="7a610-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a610-114">Application</span></span> | <span data-ttu-id="7a610-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a610-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a610-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a610-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7a610-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7a610-117">Optional query parameters</span></span>
<span data-ttu-id="7a610-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7a610-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a610-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a610-119">Request headers</span></span>
| <span data-ttu-id="7a610-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7a610-120">Name</span></span>       | <span data-ttu-id="7a610-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a610-121">Type</span></span> | <span data-ttu-id="7a610-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a610-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7a610-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a610-123">Authorization</span></span>  | <span data-ttu-id="7a610-124">string</span><span class="sxs-lookup"><span data-stu-id="7a610-124">string</span></span>  | <span data-ttu-id="7a610-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a610-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a610-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a610-127">Request body</span></span>
<span data-ttu-id="7a610-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a610-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a610-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a610-129">Response</span></span>

<span data-ttu-id="7a610-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a610-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7a610-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a610-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a610-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a610-132">Request</span></span>
<span data-ttu-id="7a610-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a610-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7a610-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a610-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/beta/contacts/{id}/directReports
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7a610-135">C#</span><span class="sxs-lookup"><span data-stu-id="7a610-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a610-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="7a610-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7a610-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7a610-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7a610-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a610-138">Response</span></span>
<span data-ttu-id="7a610-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a610-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
