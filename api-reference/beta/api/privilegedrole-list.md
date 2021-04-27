---
title: Listar privilegedRoles
description: Recupere uma lista de objetos privilegedRole.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: e785505a3b6a86b82a1631422e0e8861e68551d0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055257"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="811e0-103">Listar privilegedRoles</span><span class="sxs-lookup"><span data-stu-id="811e0-103">List privilegedRoles</span></span>

<span data-ttu-id="811e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="811e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="811e0-105">Recupere uma lista de [objetos privilegedRole.](../resources/privilegedrole.md)</span><span class="sxs-lookup"><span data-stu-id="811e0-105">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="811e0-106">Para filtrar os resultados da consulta, use as expressões ``$filter`` padrão do OData nos URIs.</span><span class="sxs-lookup"><span data-stu-id="811e0-106">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="811e0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="811e0-107">Permissions</span></span>
<span data-ttu-id="811e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="811e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="811e0-110">O solicitante precisa ter uma das seguintes funções: Administrador de Função _Privilegiada,_ _Administrador Global,_ Administrador de Segurança _ou_ Leitor de _Segurança._</span><span class="sxs-lookup"><span data-stu-id="811e0-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="811e0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="811e0-111">Permission type</span></span>      | <span data-ttu-id="811e0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="811e0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="811e0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="811e0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="811e0-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="811e0-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="811e0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="811e0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="811e0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="811e0-116">Not supported.</span></span>    |
|<span data-ttu-id="811e0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="811e0-117">Application</span></span> | <span data-ttu-id="811e0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="811e0-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="811e0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="811e0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="811e0-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="811e0-120">Optional query parameters</span></span>
<span data-ttu-id="811e0-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="811e0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="811e0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="811e0-122">Request headers</span></span>
| <span data-ttu-id="811e0-123">Nome</span><span class="sxs-lookup"><span data-stu-id="811e0-123">Name</span></span>      |<span data-ttu-id="811e0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="811e0-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="811e0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="811e0-125">Authorization</span></span>  | <span data-ttu-id="811e0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="811e0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="811e0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="811e0-128">Request body</span></span>
<span data-ttu-id="811e0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="811e0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="811e0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="811e0-130">Response</span></span>

<span data-ttu-id="811e0-131">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [privilegedRole](../resources/privilegedrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="811e0-131">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="811e0-132">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="811e0-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="811e0-133">Caso contrário, o código de status HTTP 403 Forbidden será retornado.</span><span class="sxs-lookup"><span data-stu-id="811e0-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="811e0-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="811e0-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="811e0-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="811e0-135">Request</span></span>
<span data-ttu-id="811e0-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="811e0-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="811e0-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="811e0-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles
```
# <a name="c"></a>[<span data-ttu-id="811e0-138">C#</span><span class="sxs-lookup"><span data-stu-id="811e0-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="811e0-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="811e0-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="811e0-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="811e0-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="811e0-141">Java</span><span class="sxs-lookup"><span data-stu-id="811e0-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="811e0-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="811e0-142">Response</span></span>
<span data-ttu-id="811e0-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="811e0-143">Here is an example of the response.</span></span> <span data-ttu-id="811e0-144">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="811e0-144">Note: The response object shown here might be shortened for readability.</span></span>
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
