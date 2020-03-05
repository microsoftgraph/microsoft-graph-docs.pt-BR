---
title: 'servicePrincipalName: listar proprietários'
description: Recupere uma lista de proprietários do servicePrincipalName.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: c27e2e5ba109a63d4aad56ed753f53f6d4747318
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453377"
---
# <a name="serviceprincipals-list-owners"></a><span data-ttu-id="90df0-103">servicePrincipalName: listar proprietários</span><span class="sxs-lookup"><span data-stu-id="90df0-103">servicePrincipals: List owners</span></span>

<span data-ttu-id="90df0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="90df0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90df0-105">Recupere uma lista de proprietários do servicePrincipalName.</span><span class="sxs-lookup"><span data-stu-id="90df0-105">Retrieve a list of owners of the servicePrincipal.</span></span>

## <a name="permissions"></a><span data-ttu-id="90df0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="90df0-106">Permissions</span></span>
<span data-ttu-id="90df0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90df0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90df0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90df0-109">Permission type</span></span>      | <span data-ttu-id="90df0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90df0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90df0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90df0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="90df0-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="90df0-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="90df0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90df0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90df0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90df0-114">Not supported.</span></span>    |
|<span data-ttu-id="90df0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90df0-115">Application</span></span> | <span data-ttu-id="90df0-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90df0-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="90df0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90df0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="90df0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="90df0-118">Optional query parameters</span></span>
<span data-ttu-id="90df0-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="90df0-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="90df0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90df0-120">Request headers</span></span>
| <span data-ttu-id="90df0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="90df0-121">Name</span></span>       | <span data-ttu-id="90df0-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="90df0-122">Type</span></span> | <span data-ttu-id="90df0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="90df0-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="90df0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="90df0-124">Authorization</span></span>  | <span data-ttu-id="90df0-125">string</span><span class="sxs-lookup"><span data-stu-id="90df0-125">string</span></span>  | <span data-ttu-id="90df0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90df0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90df0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90df0-128">Request body</span></span>
<span data-ttu-id="90df0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90df0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90df0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="90df0-130">Response</span></span>

<span data-ttu-id="90df0-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90df0-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="90df0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90df0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90df0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90df0-133">Request</span></span>
<span data-ttu-id="90df0-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90df0-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="90df0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="90df0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="90df0-136">C#</span><span class="sxs-lookup"><span data-stu-id="90df0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90df0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90df0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90df0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90df0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="90df0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="90df0-139">Response</span></span>
<span data-ttu-id="90df0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90df0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
