---
title: Create privilegedRoleAssignment
description: Use esta API para criar um novo privilegedRoleAssignment.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 72e30c3ea64f52657d1c70c31cea0a74c46c131a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978781"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="543a3-103">Create privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="543a3-103">Create privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="543a3-104">Use esta API para criar um novo [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="543a3-104">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="543a3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="543a3-105">Permissions</span></span>
<span data-ttu-id="543a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="543a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="543a3-108">O solicitante precisa ter função de _administrador de função privilegiada_ .</span><span class="sxs-lookup"><span data-stu-id="543a3-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="543a3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="543a3-109">Permission type</span></span>      | <span data-ttu-id="543a3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="543a3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="543a3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="543a3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="543a3-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="543a3-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="543a3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="543a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="543a3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="543a3-114">Not supported.</span></span>    |
|<span data-ttu-id="543a3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="543a3-115">Application</span></span> | <span data-ttu-id="543a3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="543a3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="543a3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="543a3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="543a3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="543a3-118">Request headers</span></span>
| <span data-ttu-id="543a3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="543a3-119">Name</span></span>       | <span data-ttu-id="543a3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="543a3-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="543a3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="543a3-121">Authorization</span></span>  | <span data-ttu-id="543a3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="543a3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="543a3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="543a3-124">Request body</span></span>
<span data-ttu-id="543a3-125">No corpo da solicitação, forneça uma representação JSON do objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="543a3-125">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="543a3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="543a3-126">Response</span></span>

<span data-ttu-id="543a3-127">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="543a3-127">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="543a3-128">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="543a3-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="543a3-129">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="543a3-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="543a3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="543a3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="543a3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="543a3-131">Request</span></span>
<span data-ttu-id="543a3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="543a3-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="543a3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="543a3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_privilegedroleassignment_from_privilegedroleassignments"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments
Content-type: application/json
Content-length: 164

{
  "userId": "userId-value",
  "roleId": "roleId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="543a3-134">C#</span><span class="sxs-lookup"><span data-stu-id="543a3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedroleassignment-from-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="543a3-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="543a3-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedroleassignment-from-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="543a3-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="543a3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedroleassignment-from-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="543a3-137">Java</span><span class="sxs-lookup"><span data-stu-id="543a3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-privilegedroleassignment-from-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="543a3-138">No corpo da solicitação, forneça uma representação JSON do objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="543a3-138">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="543a3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="543a3-139">Response</span></span>
<span data-ttu-id="543a3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="543a3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
