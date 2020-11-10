---
title: Listar privilegedRoles
description: Recupere uma lista de objetos privilegedRole.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 5bf6ba52e0c3c3cc2f729e86cb3a47de18de7f64
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970406"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="4c926-103">Listar privilegedRoles</span><span class="sxs-lookup"><span data-stu-id="4c926-103">List privilegedRoles</span></span>

<span data-ttu-id="4c926-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c926-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c926-105">Recupere uma lista de objetos [privilegedRole](../resources/privilegedrole.md) .</span><span class="sxs-lookup"><span data-stu-id="4c926-105">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="4c926-106">Para filtrar os resultados da consulta, use as expressões ``$filter`` padrão do OData nos URIs.</span><span class="sxs-lookup"><span data-stu-id="4c926-106">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="4c926-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c926-107">Permissions</span></span>
<span data-ttu-id="4c926-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c926-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4c926-110">O solicitante precisa ter uma das seguintes funções: administrador de _função privilegiada_ , _administrador global_ , _administrador de segurança_ ou _leitor de segurança_.</span><span class="sxs-lookup"><span data-stu-id="4c926-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_ , _Global Administrator_ , _Security Administrator_ , or _Security Reader_.</span></span>
 

|<span data-ttu-id="4c926-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c926-111">Permission type</span></span>      | <span data-ttu-id="4c926-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c926-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c926-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c926-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4c926-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4c926-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4c926-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c926-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c926-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c926-116">Not supported.</span></span>    |
|<span data-ttu-id="4c926-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c926-117">Application</span></span> | <span data-ttu-id="4c926-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c926-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c926-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c926-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4c926-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4c926-120">Optional query parameters</span></span>
<span data-ttu-id="4c926-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4c926-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c926-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c926-122">Request headers</span></span>
| <span data-ttu-id="4c926-123">Nome</span><span class="sxs-lookup"><span data-stu-id="4c926-123">Name</span></span>      |<span data-ttu-id="4c926-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c926-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4c926-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c926-125">Authorization</span></span>  | <span data-ttu-id="4c926-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c926-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c926-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c926-128">Request body</span></span>
<span data-ttu-id="4c926-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4c926-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c926-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c926-130">Response</span></span>

<span data-ttu-id="4c926-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [privilegedRole](../resources/privilegedrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c926-131">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="4c926-132">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="4c926-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="4c926-133">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="4c926-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="4c926-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c926-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c926-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c926-135">Request</span></span>
<span data-ttu-id="4c926-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c926-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4c926-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c926-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles
```
# <a name="c"></a>[<span data-ttu-id="4c926-138">C#</span><span class="sxs-lookup"><span data-stu-id="4c926-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c926-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c926-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c926-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c926-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c926-141">Java</span><span class="sxs-lookup"><span data-stu-id="4c926-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4c926-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c926-142">Response</span></span>
<span data-ttu-id="4c926-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c926-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
