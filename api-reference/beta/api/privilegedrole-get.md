---
title: Get privilegedRole
description: 'Recupere as propriedades e os relacionamentos do objeto privilegedRole. '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: a366130529de2c06273f34e8fc336c7ad433a8f8
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412814"
---
# <a name="get-privilegedrole"></a><span data-ttu-id="1be5c-103">Get privilegedRole</span><span class="sxs-lookup"><span data-stu-id="1be5c-103">Get privilegedRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1be5c-104">Recupere as propriedades e os relacionamentos do objeto [privilegedRole](../resources/privilegedrole.md) .</span><span class="sxs-lookup"><span data-stu-id="1be5c-104">Retrieve the properties and relationships of [privilegedRole](../resources/privilegedrole.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="1be5c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1be5c-105">Permissions</span></span>
<span data-ttu-id="1be5c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1be5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1be5c-108">O solicitante precisa ter uma das seguintes funções: administrador de _função privilegiada_, _administrador global_, _administrador de segurança_ou _leitor de segurança_.</span><span class="sxs-lookup"><span data-stu-id="1be5c-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="1be5c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1be5c-109">Permission type</span></span>      | <span data-ttu-id="1be5c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1be5c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1be5c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1be5c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1be5c-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1be5c-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1be5c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1be5c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1be5c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1be5c-114">Not supported.</span></span>    |
|<span data-ttu-id="1be5c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1be5c-115">Application</span></span> | <span data-ttu-id="1be5c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1be5c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1be5c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1be5c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}
GET /privilegedRoleAssignments/{id}/roleInfo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1be5c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1be5c-118">Optional query parameters</span></span>
<span data-ttu-id="1be5c-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1be5c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1be5c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1be5c-120">Request headers</span></span>
| <span data-ttu-id="1be5c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1be5c-121">Name</span></span>      |<span data-ttu-id="1be5c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1be5c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1be5c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1be5c-123">Authorization</span></span>  | <span data-ttu-id="1be5c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1be5c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1be5c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1be5c-126">Request body</span></span>
<span data-ttu-id="1be5c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1be5c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1be5c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1be5c-128">Response</span></span>

<span data-ttu-id="1be5c-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [privilegedRole](../resources/privilegedrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1be5c-129">If successful, this method returns a `200 OK` response code and [privilegedRole](../resources/privilegedrole.md) object in the response body.</span></span>

<span data-ttu-id="1be5c-130">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="1be5c-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="1be5c-131">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="1be5c-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="1be5c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1be5c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1be5c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1be5c-133">Request</span></span>
<span data-ttu-id="1be5c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1be5c-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1be5c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1be5c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrole"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1be5c-136">C#</span><span class="sxs-lookup"><span data-stu-id="1be5c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1be5c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1be5c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1be5c-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1be5c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1be5c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1be5c-139">Response</span></span>
<span data-ttu-id="1be5c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1be5c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
