---
title: Create privilegedRoleAssignment
description: Use esta API para criar um novo privilegedRoleAssignment.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: f053dcbf93c4a933b4a4de4ea096621e7cb720e4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034970"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="42855-103">Create privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="42855-103">Create privilegedRoleAssignment</span></span>

<span data-ttu-id="42855-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42855-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42855-105">Use esta API para criar um novo  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="42855-105">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="42855-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="42855-106">Permissions</span></span>
<span data-ttu-id="42855-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42855-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="42855-109">O solicitante precisa ter função de _administrador de função privilegiada_ .</span><span class="sxs-lookup"><span data-stu-id="42855-109">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="42855-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42855-110">Permission type</span></span>      | <span data-ttu-id="42855-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42855-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42855-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42855-112">Delegated (work or school account)</span></span> | <span data-ttu-id="42855-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="42855-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="42855-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42855-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42855-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42855-115">Not supported.</span></span>    |
|<span data-ttu-id="42855-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42855-116">Application</span></span> | <span data-ttu-id="42855-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42855-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42855-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42855-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="42855-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42855-119">Request headers</span></span>
| <span data-ttu-id="42855-120">Nome</span><span class="sxs-lookup"><span data-stu-id="42855-120">Name</span></span>       | <span data-ttu-id="42855-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="42855-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="42855-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="42855-122">Authorization</span></span>  | <span data-ttu-id="42855-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42855-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42855-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42855-125">Request body</span></span>
<span data-ttu-id="42855-126">No corpo da solicitação, forneça uma representação JSON do objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="42855-126">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="42855-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="42855-127">Response</span></span>

<span data-ttu-id="42855-128">Se bem-sucedido, este método retorna o `201 Created` código de resposta e o objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42855-128">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="42855-129">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="42855-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="42855-130">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="42855-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="42855-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42855-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42855-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42855-132">Request</span></span>
<span data-ttu-id="42855-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42855-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42855-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="42855-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="42855-135">C#</span><span class="sxs-lookup"><span data-stu-id="42855-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedroleassignment-from-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42855-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42855-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedroleassignment-from-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42855-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42855-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedroleassignment-from-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="42855-138">No corpo da solicitação, forneça uma representação JSON do objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="42855-138">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="42855-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="42855-139">Response</span></span>
<span data-ttu-id="42855-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42855-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


