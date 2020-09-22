---
title: Get privilegedRole
description: 'Recupere as propriedades e os relacionamentos do objeto privilegedRole. '
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: a3dcdff7395d3ec531dec9fd38686430c707995a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035173"
---
# <a name="get-privilegedrole"></a><span data-ttu-id="e01b5-103">Get privilegedRole</span><span class="sxs-lookup"><span data-stu-id="e01b5-103">Get privilegedRole</span></span>

<span data-ttu-id="e01b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e01b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e01b5-105">Recupere as propriedades e os relacionamentos do objeto [privilegedRole](../resources/privilegedrole.md) .</span><span class="sxs-lookup"><span data-stu-id="e01b5-105">Retrieve the properties and relationships of [privilegedRole](../resources/privilegedrole.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e01b5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e01b5-106">Permissions</span></span>
<span data-ttu-id="e01b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e01b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e01b5-109">O solicitante precisa ter uma das seguintes funções: administrador de _função privilegiada_, _administrador global_, _administrador de segurança_ou _leitor de segurança_.</span><span class="sxs-lookup"><span data-stu-id="e01b5-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="e01b5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e01b5-110">Permission type</span></span>      | <span data-ttu-id="e01b5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e01b5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e01b5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e01b5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e01b5-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e01b5-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e01b5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e01b5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e01b5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e01b5-115">Not supported.</span></span>    |
|<span data-ttu-id="e01b5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e01b5-116">Application</span></span> | <span data-ttu-id="e01b5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e01b5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e01b5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e01b5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}
GET /privilegedRoleAssignments/{id}/roleInfo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e01b5-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e01b5-119">Optional query parameters</span></span>
<span data-ttu-id="e01b5-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e01b5-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e01b5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e01b5-121">Request headers</span></span>
| <span data-ttu-id="e01b5-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e01b5-122">Name</span></span>      |<span data-ttu-id="e01b5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e01b5-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e01b5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e01b5-124">Authorization</span></span>  | <span data-ttu-id="e01b5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e01b5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e01b5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e01b5-127">Request body</span></span>
<span data-ttu-id="e01b5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e01b5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e01b5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e01b5-129">Response</span></span>

<span data-ttu-id="e01b5-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [privilegedRole](../resources/privilegedrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e01b5-130">If successful, this method returns a `200 OK` response code and [privilegedRole](../resources/privilegedrole.md) object in the response body.</span></span>

<span data-ttu-id="e01b5-131">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="e01b5-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="e01b5-132">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="e01b5-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="e01b5-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e01b5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e01b5-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e01b5-134">Request</span></span>
<span data-ttu-id="e01b5-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e01b5-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e01b5-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e01b5-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}
```
# <a name="c"></a>[<span data-ttu-id="e01b5-137">C#</span><span class="sxs-lookup"><span data-stu-id="e01b5-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e01b5-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e01b5-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e01b5-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e01b5-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e01b5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e01b5-140">Response</span></span>
<span data-ttu-id="e01b5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e01b5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


