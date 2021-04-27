---
title: Create privilegedRoleAssignment
description: Use essa API para criar um novo privilegedRoleAssignment.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: ae11f0c21a4dcb314d12f4b74e570ea4cafc03a8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052898"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="b6bbf-103">Create privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b6bbf-103">Create privilegedRoleAssignment</span></span>

<span data-ttu-id="b6bbf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6bbf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6bbf-105">Use essa API para criar um  [novo privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b6bbf-105">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="b6bbf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6bbf-106">Permissions</span></span>
<span data-ttu-id="b6bbf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6bbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b6bbf-109">O solicitante precisa ter função _de Administrador de Função_ Privilegiada.</span><span class="sxs-lookup"><span data-stu-id="b6bbf-109">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="b6bbf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6bbf-110">Permission type</span></span>      | <span data-ttu-id="b6bbf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6bbf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6bbf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6bbf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b6bbf-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b6bbf-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b6bbf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6bbf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6bbf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6bbf-115">Not supported.</span></span>    |
|<span data-ttu-id="b6bbf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6bbf-116">Application</span></span> | <span data-ttu-id="b6bbf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6bbf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6bbf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6bbf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="b6bbf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6bbf-119">Request headers</span></span>
| <span data-ttu-id="b6bbf-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b6bbf-120">Name</span></span>       | <span data-ttu-id="b6bbf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6bbf-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b6bbf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6bbf-122">Authorization</span></span>  | <span data-ttu-id="b6bbf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6bbf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6bbf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6bbf-125">Request body</span></span>
<span data-ttu-id="b6bbf-126">No corpo da solicitação, fornece uma representação JSON do [objeto privilegedRoleAssignment.](../resources/privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b6bbf-126">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b6bbf-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6bbf-127">Response</span></span>

<span data-ttu-id="b6bbf-128">Se tiver êxito, este método retornará `201 Created` o código de resposta e o objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6bbf-128">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="b6bbf-129">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="b6bbf-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="b6bbf-130">Caso contrário, o código de status HTTP 403 Forbidden será retornado.</span><span class="sxs-lookup"><span data-stu-id="b6bbf-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="b6bbf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6bbf-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6bbf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6bbf-132">Request</span></span>
<span data-ttu-id="b6bbf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6bbf-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b6bbf-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6bbf-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b6bbf-135">C#</span><span class="sxs-lookup"><span data-stu-id="b6bbf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedroleassignment-from-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6bbf-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6bbf-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedroleassignment-from-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6bbf-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6bbf-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedroleassignment-from-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6bbf-138">Java</span><span class="sxs-lookup"><span data-stu-id="b6bbf-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-privilegedroleassignment-from-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b6bbf-139">No corpo da solicitação, fornece uma representação JSON do [objeto privilegedRoleAssignment.](../resources/privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b6bbf-139">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b6bbf-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6bbf-140">Response</span></span>
<span data-ttu-id="b6bbf-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6bbf-141">Here is an example of the response.</span></span> <span data-ttu-id="b6bbf-142">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b6bbf-142">Note: The response object shown here might be shortened for readability.</span></span>
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


