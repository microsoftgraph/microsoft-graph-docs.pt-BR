---
title: Listar privilegedRoles
description: Recupere uma lista de objetos privilegedRole.
localization_priority: Normal
ms.openlocfilehash: 020a67e2347a91e665ca1832b3ad45467f8d8de9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445034"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="c2168-103">Listar privilegedRoles</span><span class="sxs-lookup"><span data-stu-id="c2168-103">List privilegedRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2168-104">Recupere uma lista de objetos [privilegedRole](../resources/privilegedrole.md) .</span><span class="sxs-lookup"><span data-stu-id="c2168-104">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="c2168-105">Para filtrar os resultados da consulta, use as expressões ``$filter`` padrão do OData nos URIs.</span><span class="sxs-lookup"><span data-stu-id="c2168-105">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="c2168-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2168-106">Permissions</span></span>
<span data-ttu-id="c2168-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2168-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c2168-109">O solicitante precisa ter uma das seguintes funções: administrador de _função privilegiada_, _administrador global_, _administrador de segurança_ou _leitor de segurança_.</span><span class="sxs-lookup"><span data-stu-id="c2168-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="c2168-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2168-110">Permission type</span></span>      | <span data-ttu-id="c2168-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2168-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2168-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2168-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c2168-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c2168-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c2168-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2168-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2168-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2168-115">Not supported.</span></span>    |
|<span data-ttu-id="c2168-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2168-116">Application</span></span> | <span data-ttu-id="c2168-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2168-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2168-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2168-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c2168-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c2168-119">Optional query parameters</span></span>
<span data-ttu-id="c2168-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c2168-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2168-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2168-121">Request headers</span></span>
| <span data-ttu-id="c2168-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c2168-122">Name</span></span>      |<span data-ttu-id="c2168-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2168-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c2168-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2168-124">Authorization</span></span>  | <span data-ttu-id="c2168-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2168-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2168-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2168-127">Request body</span></span>
<span data-ttu-id="c2168-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2168-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2168-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2168-129">Response</span></span>

<span data-ttu-id="c2168-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [privilegedRole](../resources/privilegedrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2168-130">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="c2168-131">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="c2168-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c2168-132">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="c2168-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="c2168-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2168-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2168-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2168-134">Request</span></span>
<span data-ttu-id="c2168-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2168-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c2168-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2168-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2168-137">C#</span><span class="sxs-lookup"><span data-stu-id="c2168-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2168-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2168-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2168-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c2168-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c2168-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2168-140">Response</span></span>
<span data-ttu-id="c2168-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2168-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 83

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
