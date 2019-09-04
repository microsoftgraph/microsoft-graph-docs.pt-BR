---
title: 'servicePrincipalName: listar ownedObjects'
description: Recupere uma lista de objetos pertencentes ao servicePrincipalName.  Isso pode incluir aplicativos ou grupos.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 53bb8f5cb14dd33b62e53983e16e660fca14387b
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724586"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="f6e42-104">servicePrincipalName: listar ownedObjects</span><span class="sxs-lookup"><span data-stu-id="f6e42-104">servicePrincipals: List ownedObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6e42-105">Recupere uma lista de objetos pertencentes ao servicePrincipalName.</span><span class="sxs-lookup"><span data-stu-id="f6e42-105">Retrieve a list of objects owned by the servicePrincipal.</span></span>  <span data-ttu-id="f6e42-106">Isso pode incluir aplicativos ou grupos.</span><span class="sxs-lookup"><span data-stu-id="f6e42-106">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6e42-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f6e42-107">Permissions</span></span>
<span data-ttu-id="f6e42-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6e42-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6e42-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6e42-110">Permission type</span></span>      | <span data-ttu-id="f6e42-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f6e42-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6e42-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6e42-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f6e42-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f6e42-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f6e42-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6e42-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6e42-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6e42-115">Not supported.</span></span>    |
|<span data-ttu-id="f6e42-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6e42-116">Application</span></span> | <span data-ttu-id="f6e42-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6e42-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6e42-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6e42-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f6e42-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f6e42-119">Optional query parameters</span></span>
<span data-ttu-id="f6e42-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f6e42-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6e42-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6e42-121">Request headers</span></span>
| <span data-ttu-id="f6e42-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f6e42-122">Name</span></span>       | <span data-ttu-id="f6e42-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6e42-123">Type</span></span> | <span data-ttu-id="f6e42-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6e42-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f6e42-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6e42-125">Authorization</span></span>  | <span data-ttu-id="f6e42-126">string</span><span class="sxs-lookup"><span data-stu-id="f6e42-126">string</span></span>  | <span data-ttu-id="f6e42-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6e42-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6e42-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6e42-129">Request body</span></span>
<span data-ttu-id="f6e42-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f6e42-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6e42-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6e42-131">Response</span></span>

<span data-ttu-id="f6e42-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6e42-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f6e42-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6e42-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6e42-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6e42-134">Request</span></span>
<span data-ttu-id="f6e42-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6e42-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f6e42-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6e42-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/ownedObjects
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f6e42-137">C#</span><span class="sxs-lookup"><span data-stu-id="f6e42-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ownedobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6e42-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6e42-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ownedobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f6e42-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f6e42-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ownedobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f6e42-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6e42-140">Response</span></span>
<span data-ttu-id="f6e42-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f6e42-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
