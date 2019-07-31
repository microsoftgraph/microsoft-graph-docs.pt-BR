---
title: Get privilegedRole
description: 'Recupere as propriedades e os relacionamentos do objeto privilegedRole. '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 29bcd565c9dba3dc8bf1216d5c12c3b52695527c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978810"
---
# <a name="get-privilegedrole"></a><span data-ttu-id="106e6-103">Get privilegedRole</span><span class="sxs-lookup"><span data-stu-id="106e6-103">Get privilegedRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="106e6-104">Recupere as propriedades e os relacionamentos do objeto [privilegedRole](../resources/privilegedrole.md) .</span><span class="sxs-lookup"><span data-stu-id="106e6-104">Retrieve the properties and relationships of [privilegedRole](../resources/privilegedrole.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="106e6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="106e6-105">Permissions</span></span>
<span data-ttu-id="106e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="106e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="106e6-108">O solicitante precisa ter uma das seguintes funções: administrador de _função privilegiada_, _administrador global_, _administrador de segurança_ou _leitor de segurança_.</span><span class="sxs-lookup"><span data-stu-id="106e6-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="106e6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="106e6-109">Permission type</span></span>      | <span data-ttu-id="106e6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="106e6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="106e6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="106e6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="106e6-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="106e6-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="106e6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="106e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="106e6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="106e6-114">Not supported.</span></span>    |
|<span data-ttu-id="106e6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="106e6-115">Application</span></span> | <span data-ttu-id="106e6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="106e6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="106e6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="106e6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}
GET /privilegedRoleAssignments/{id}/roleInfo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="106e6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="106e6-118">Optional query parameters</span></span>
<span data-ttu-id="106e6-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="106e6-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="106e6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="106e6-120">Request headers</span></span>
| <span data-ttu-id="106e6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="106e6-121">Name</span></span>      |<span data-ttu-id="106e6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="106e6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="106e6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="106e6-123">Authorization</span></span>  | <span data-ttu-id="106e6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="106e6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="106e6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="106e6-126">Request body</span></span>
<span data-ttu-id="106e6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="106e6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="106e6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="106e6-128">Response</span></span>

<span data-ttu-id="106e6-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [privilegedRole](../resources/privilegedrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="106e6-129">If successful, this method returns a `200 OK` response code and [privilegedRole](../resources/privilegedrole.md) object in the response body.</span></span>

<span data-ttu-id="106e6-130">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="106e6-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="106e6-131">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="106e6-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="106e6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="106e6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="106e6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="106e6-133">Request</span></span>
<span data-ttu-id="106e6-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="106e6-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="106e6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="106e6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrole"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="106e6-136">C#</span><span class="sxs-lookup"><span data-stu-id="106e6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="106e6-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="106e6-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="106e6-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="106e6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="106e6-139">Java</span><span class="sxs-lookup"><span data-stu-id="106e6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="106e6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="106e6-140">Response</span></span>
<span data-ttu-id="106e6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="106e6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
